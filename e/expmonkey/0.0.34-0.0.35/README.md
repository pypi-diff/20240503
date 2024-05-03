# Comparing `tmp/expmonkey-0.0.34.tar.gz` & `tmp/expmonkey-0.0.35.tar.gz`

## Comparing `expmonkey-0.0.34.tar` & `expmonkey-0.0.35.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 expmonkey-0.0.34/.flake8
--rw-r--r--   0        0        0    32647 2020-02-02 00:00:00.000000 expmonkey-0.0.34/expmonkey/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 expmonkey-0.0.34/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 expmonkey-0.0.34/LICENSE
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 expmonkey-0.0.34/README.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 expmonkey-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 expmonkey-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 expmonkey-0.0.35/.flake8
+-rw-r--r--   0        0        0    32863 2020-02-02 00:00:00.000000 expmonkey-0.0.35/expmonkey/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 expmonkey-0.0.35/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 expmonkey-0.0.35/LICENSE
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 expmonkey-0.0.35/README.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 expmonkey-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 expmonkey-0.0.35/PKG-INFO
```

### Comparing `expmonkey-0.0.34/expmonkey/__init__.py` & `expmonkey-0.0.35/expmonkey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     sys.stderr.write(msg)
     sys.stderr.write('\n')
     sys.stderr.flush()
     sys.exit(1)
 
 
 def _get_basedir(path=os.getcwd()):
-    path = os.path.abspath(path)
+    path = os.path.realpath(path)
     while True:
         if os.path.exists(os.path.join(path, '.em')):
             return path
         if path == os.path.dirname(path):
             _die('Project not found, you may want to start with "em init"')
         path = os.path.dirname(path)
 
 
 def _get_parent_git_path(path=os.getcwd()):
-    path = os.path.abspath(path)
+    path = os.path.realpath(path)
     relpath = './'
     while True:
         if os.path.exists(os.path.join(path, '.git')):
             return relpath
         if path == os.path.dirname(path):
             return None
         path = os.path.dirname(path)
@@ -90,15 +90,15 @@
 
     def list_worktrees(self):
         worktrees = []
         prev_path = None
         prev_head = None
         for line in self.check_output('git', 'worktree', 'list', '--porcelain').splitlines():
             if line.startswith('worktree'):
-                prev_path = line.split()[1]
+                prev_path = os.path.realpath(line.split()[1])
             if line.startswith('HEAD'):
                 prev_head = line.split()[1]
             if line.startswith('branch'):
                 branch = line.split()[1]
                 if branch.startswith('refs/heads/'):
                     branch = branch[len('refs/heads/'):]
                     worktrees.append({
@@ -265,19 +265,19 @@
     subprocess.check_output(['git', 'checkout', '-b', '__empty', '--quiet'], cwd=tmp_path)
     subprocess.check_output(['git', 'commit', '--allow-empty', '-m', 'Empty'], cwd=tmp_path)
     os.rename(tmp_path, path)
 
 
 def _get_branch(path=os.getcwd()):
     basedir = _get_basedir()
-    branch = os.path.relpath(path, basedir)
-    if not branch.strip('./'):
+    branch = os.path.relpath(path, basedir).strip('.').strip('/')
+    repo = _get_repo()
+    if branch not in repo.list_local_branches():
         return None
-    repo = _get_repo(path)
-    return repo.get_current_branch()
+    return branch
 
 
 def get_branch():
     env_override = os.getenv('EXPMONKEY_BRANCH')
     if env_override:
         return env_override
     branch = _get_branch()
@@ -294,15 +294,15 @@
 
 
 def _list_checked_out_branches():
     repo = _get_repo()
     basedir = _get_basedir()
     worktrees = repo.list_worktrees()
 
-    basedir = os.path.abspath(basedir)
+    basedir = os.path.realpath(basedir)
     branches = []
     for worktree in worktrees:
         if os.path.join(basedir, worktree['branch']) == worktree['path']:
             branches.append(worktree['branch'])
     return branches
 
 
@@ -311,15 +311,15 @@
 
 
 def _check_branch(branch, in_worktree=None, in_branch=None):
     repo = _get_repo()
     basedir = _get_basedir()
     worktrees = repo.list_worktrees()
 
-    basedir = os.path.abspath(basedir)
+    basedir = os.path.realpath(basedir)
     found_in_worktree = False
     for worktree in worktrees:
         if worktree['branch'] == branch:
             if os.path.join(basedir, worktree['branch']) == worktree['path']:
                 found_in_worktree = True
 
     if in_worktree is True and not found_in_worktree:
@@ -354,45 +354,52 @@
                  'branch "{}" not the same with branch in directory "{}"'.format(branch, current_branch))
 
     elif in_worktree is False:
         if _is_git_repo(os.path.join(basedir, branch)):
             _die('Directory "{}" already exists'.format(os.path.join(basedir, branch)))
 
 
-init_script = '''
-function em() {
+def print_init_script():
+    bash_argcomplete_script = argcomplete.shellcode(["em", "expmonkey"], shell='bash')
+    zsh_argcomplete_script = argcomplete.shellcode(["em", "expmonkey"], shell='zsh')
+
+    init_script = '''
+function expmonkey() {
     _EM_OUTPUT_NEW_PWD=$(mktemp)
 
-    _EM_OUTPUT_NEW_PWD=$_EM_OUTPUT_NEW_PWD expmonkey $@
+    _EM_OUTPUT_NEW_PWD=$_EM_OUTPUT_NEW_PWD command expmonkey $@
     if [[ $? -eq 0 ]]; then
         _EM_NEW_PWD=$(cat $_EM_OUTPUT_NEW_PWD)
         if [[ $_EM_NEW_PWD != "" && $_EM_NEW_PWD != $PWD ]]; then
             cd $_EM_NEW_PWD
         fi
     fi
 
     rm -rf $_EM_OUTPUT_NEW_PWD
 }
 
+if ! command -v em > /dev/null; then
+    function em() {
+        expmonkey $@
+    }
+fi
+
+
 if [[ -n "$BASH" || $0 == "-bash" ]]; then
-    eval "$(register-python-argcomplete em)"
-    eval "$(register-python-argcomplete expmonkey)"
+    ''' + bash_argcomplete_script + '''
 fi
+
 if [[ -n "$ZSH" || -n "$ZSH_NAME" || $0 == "-zsh" || $0 == "zsh" ]]; then
     autoload -U bashcompinit
     bashcompinit
-    eval "$(register-python-argcomplete em)"
-    eval "$(register-python-argcomplete expmonkey)"
+    ''' + zsh_argcomplete_script + '''
 fi
 
 export EXPMONKEY_INITED=1
-'''
-
-
-def print_init_script():
+    '''
     print(init_script)
 
 
 main_help = '''
 Expmonkey
 
 A lightweight experiment management tool based on git worktree
@@ -553,15 +560,15 @@
     args = parser.parse_args()
     args.func(args)
 
 
 def cli():
     if not os.getenv('EXPMONKEY_INITED'):
         print(colored.stylize('''Expmonkey autocompletion is not enabled
-Please add "source em-init.sh" to your ~/.bashrc or ~/.zshrc
+Please add 'eval "$(em-init-script)"' to your ~/.bashrc or ~/.zshrc
 You may want to install fzf for better experience''', colored.fg('red')))
         raise RuntimeError('Expmonkey is not inited')
     main()
 
 
 def clone(args):
     repo = args.repo
@@ -587,15 +594,15 @@
         git_path = _get_parent_git_path()
         if git_path is None:
             _die('No git repo found, please specify repo path')
         repo = git_path
     if _is_git_repo(repo):
         os.makedirs('.em', exist_ok=True)
         with open('.em/repo', 'w') as f:
-            f.write(os.path.abspath(repo))
+            f.write(os.path.realpath(repo))
     else:
         os.makedirs('.em/repo.tmp', exist_ok=True)
         _clone_repository(repo, '.em/repo', tempfile.mkdtemp(dir='.em/repo.tmp'))
 
     print('Successfully inited repo: {}'.format(repo))
```

### Comparing `expmonkey-0.0.34/.gitignore` & `expmonkey-0.0.35/.gitignore`

 * *Files identical despite different names*

### Comparing `expmonkey-0.0.34/LICENSE` & `expmonkey-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `expmonkey-0.0.34/README.md` & `expmonkey-0.0.35/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 1. Conjure the Python package:
 ```shell
 pip3 install expmonkey
 ```
 
 2. (Optional) Weave `em-init-script` into your shell's tapestry for autocompletion and arcane abilities:
 ```bash
-echo 'source <(em-init-script)' >> ~/.bashrc
+echo 'eval "$(em-init-script)"' >> ~/.bashrc
 ```
 
 3. (Optional) Summon `fzf` for a mystical user experience:
 ``` bash
 git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
 ~/.fzf/install
 ```
@@ -145,8 +145,8 @@
 Witness the divergence between realms:
 ``` shell
 em diff <branch1> <branch2>
 ```
 
 ## 📜 License
 
-This project is a tome of knowledge, open to all seekers under the [MIT License](LICENSE).
+This project is a tome of knowledge, open to all seekers under the [MIT License](LICENSE).
```

### Comparing `expmonkey-0.0.34/pyproject.toml` & `expmonkey-0.0.35/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "expmonkey"
-version = "0.0.34"
+version = "0.0.35"
 authors = [
     { name = "liuyibo", email = "liuyibo1994@qq.com" },
 ]
 maintainers = [
     { name = "liuyibo", email = "liuyibo1994@qq.com" },
 ]
 description="A git worktree-based CLI tool for efficient management and navigation of multiple isolated experiments in parallel development workflows"
@@ -30,15 +30,14 @@
 keywords = ["experiment management", "git worktree", "research workflow", "development tools", "version control", "branch management", "command-line interface", "parallel development", "code branching", "workspace management", "git enhancements", "scientific experiments", "machine learning experiments", "project organization", "code experiments", "git branches"]
 
 [project.urls]
 Homepage = "https://github.com/liuyibo/expmonkey"
 Issues = "https://github.com/liuyibo/expmonkey/issues"
 
 [project.scripts]
-em = "expmonkey:cli"
 expmonkey = "expmonkey:cli"
 em-init-script = "expmonkey:print_init_script"
 
 [tool.hatch.build.targets.wheel]
 include = [
   "/expmonkey/*.py",
-]
+]
```

### Comparing `expmonkey-0.0.34/PKG-INFO` & `expmonkey-0.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: expmonkey
-Version: 0.0.34
+Version: 0.0.35
 Summary: A git worktree-based CLI tool for efficient management and navigation of multiple isolated experiments in parallel development workflows
 Project-URL: Homepage, https://github.com/liuyibo/expmonkey
 Project-URL: Issues, https://github.com/liuyibo/expmonkey/issues
 Author-email: liuyibo <liuyibo1994@qq.com>
 Maintainer-email: liuyibo <liuyibo1994@qq.com>
 License-File: LICENSE
 Keywords: branch management,code branching,code experiments,command-line interface,development tools,experiment management,git branches,git enhancements,git worktree,machine learning experiments,parallel development,project organization,research workflow,scientific experiments,version control,workspace management
@@ -54,15 +54,15 @@
 1. Conjure the Python package:
 ```shell
 pip3 install expmonkey
 ```
 
 2. (Optional) Weave `em-init-script` into your shell's tapestry for autocompletion and arcane abilities:
 ```bash
-echo 'source <(em-init-script)' >> ~/.bashrc
+echo 'eval "$(em-init-script)"' >> ~/.bashrc
 ```
 
 3. (Optional) Summon `fzf` for a mystical user experience:
 ``` bash
 git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
 ~/.fzf/install
 ```
@@ -166,8 +166,8 @@
 Witness the divergence between realms:
 ``` shell
 em diff <branch1> <branch2>
 ```
 
 ## 📜 License
 
-This project is a tome of knowledge, open to all seekers under the [MIT License](LICENSE).
+This project is a tome of knowledge, open to all seekers under the [MIT License](LICENSE).
```

