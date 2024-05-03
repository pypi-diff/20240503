# Comparing `tmp/mdremotifier-0.2.0.tar.gz` & `tmp/mdremotifier-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/markdown-remotifier/dist/.tmp-zgnqdol1/mdremotifier-0.2.0.tar", last modified: Tue Apr 30 20:23:20 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/markdown-remotifier/dist/.tmp-p4y9whvo/mdremotifier-0.3.0.tar", last modified: Fri May  3 15:05:53 2024, max compression
```

## Comparing `mdremotifier-0.2.0.tar` & `mdremotifier-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 20:23:20.733309 mdremotifier-0.2.0/
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 20:23:20.514473 mdremotifier-0.2.0/.github/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    16973 2024-04-30 19:08:57.000000 mdremotifier-0.2.0/.github/README.remotified.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdremotifier-0.2.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    22528 2024-04-30 20:23:20.726439 mdremotifier-0.2.0/PKG-INFO
--r-xr-xr-x   0 realz     (1000) realz     (1000)    15860 2024-04-30 19:08:56.000000 mdremotifier-0.2.0/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 20:23:20.558418 mdremotifier-0.2.0/mdremotifier/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      396 2024-04-27 10:02:01.000000 mdremotifier-0.2.0/mdremotifier/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     7389 2024-04-27 11:38:45.000000 mdremotifier-0.2.0/mdremotifier/cli.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 20:23:20.706334 mdremotifier-0.2.0/mdremotifier.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    22528 2024-04-30 20:23:20.000000 mdremotifier-0.2.0/mdremotifier.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      327 2024-04-30 20:23:20.000000 mdremotifier-0.2.0/mdremotifier.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-30 20:23:20.000000 mdremotifier-0.2.0/mdremotifier.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       55 2024-04-30 20:23:20.000000 mdremotifier-0.2.0/mdremotifier.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1373 2024-04-30 20:23:20.000000 mdremotifier-0.2.0/mdremotifier.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       13 2024-04-30 20:23:20.000000 mdremotifier-0.2.0/mdremotifier.egg-info/top_level.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     3474 2024-04-30 17:53:03.000000 mdremotifier-0.2.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-30 20:23:20.733309 mdremotifier-0.2.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 15:05:53.071589 mdremotifier-0.3.0/
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 15:05:52.870756 mdremotifier-0.3.0/.github/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    15610 2024-05-03 15:05:15.000000 mdremotifier-0.3.0/.github/README.remotified.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdremotifier-0.3.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    22360 2024-05-03 15:05:53.060951 mdremotifier-0.3.0/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    14493 2024-05-03 15:05:15.000000 mdremotifier-0.3.0/README.md
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 15:05:52.917085 mdremotifier-0.3.0/mdremotifier/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      396 2024-04-27 10:02:01.000000 mdremotifier-0.3.0/mdremotifier/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     8393 2024-05-03 15:05:15.000000 mdremotifier-0.3.0/mdremotifier/cli.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 15:05:53.040411 mdremotifier-0.3.0/mdremotifier.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    22360 2024-05-03 15:05:52.000000 mdremotifier-0.3.0/mdremotifier.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      327 2024-05-03 15:05:52.000000 mdremotifier-0.3.0/mdremotifier.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-03 15:05:52.000000 mdremotifier-0.3.0/mdremotifier.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       55 2024-05-03 15:05:52.000000 mdremotifier-0.3.0/mdremotifier.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1824 2024-05-03 15:05:52.000000 mdremotifier-0.3.0/mdremotifier.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       13 2024-05-03 15:05:52.000000 mdremotifier-0.3.0/mdremotifier.egg-info/top_level.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4045 2024-05-03 15:05:15.000000 mdremotifier-0.3.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-03 15:05:53.073095 mdremotifier-0.3.0/setup.cfg
```

### Comparing `mdremotifier-0.2.0/.github/README.remotified.md` & `mdremotifier-0.3.0/.github/README.remotified.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdremotifier][22]</div>
+# <div align="center">![mdremotifier][1]</div>
 
 <div align="center">
 
-<h1>warning _THIS PROJECT IS ALPHA^ALPHA, NOT READY FOR USE</h1>
-
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -45,52 +43,52 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
-**CLI to replace `./image.png` to <raw.githubusercontent.com> remote URL in
+**CLI to replace `./image.png` to `raw.githubusercontent.com` remote URL in
 README.md**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img src="./.github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/0.3.0/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdremotifier does:
 
-Turn this ([./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md)):
+Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
 ```
 <!---->
 
 Into this
-([./mdremotifier/examples/EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md)):
+([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.remotified.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md).
 
@@ -108,20 +106,20 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.2.0
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md)):
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
@@ -139,29 +137,29 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m mdremotifier.cli --help`" />
-<!---->
+<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/0.3.0/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - mdremotifier's own `README`:
-  - Original: [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md).
-  - Remotified: [./.github/README.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/README.remotified.md).
-  - Generation script: [./scripts/generate-readme.sh](https://raw.githubusercontent.com/realazthat/mdremotifier/master/scripts/generate-readme.sh).
+  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md).
+  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/README.remotified.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/scripts/generate-readme.sh).
 - Example:
-  - Original: [./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md).
+  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md).
   - Remotified:
-    [./mdremotifier/examples/EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md).
+    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.remotified.md).
   - Generation script:
-    [./mdremotifier/examples/example.sh](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/example.sh).
+    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdremotifier
 - Projects using mdremotifier:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -184,25 +182,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdremotifier are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -210,62 +208,82 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ------------------------------------------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [bdashore3/remark-github-images][60]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
-| [laobie/WriteMarkdownLazily][54]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [crh19970307/mdul][55]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][56] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                     |
-| [jen6/imgo][57]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                     |
-| [chocoluffy/lazy-markdown][59]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [loheagn/gopic][61]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                     |
-| [Undertone0809/imarkdown][53]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                      |
-| [ravgeetdhillon/markdown-imgur-upload][58]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                      |
+| [bdashore3/remark-github-images][23]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
+| [laobie/WriteMarkdownLazily][24]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [crh19970307/mdul][25]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][26] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                     |
+| [jen6/imgo][27]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                     |
+| [chocoluffy/lazy-markdown][28]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [loheagn/gopic][29]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                     |
+| [Undertone0809/imarkdown][30]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                      |
+| [ravgeetdhillon/markdown-imgur-upload][31]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                      |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.python-version) (which is currently
     `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml).
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash`, `rsync` (for
-    tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act, animation).
+    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/pyproject.toml).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdremotifier-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -277,74 +295,38 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
-[2]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
-[3]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
-[4]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdremotifier/
-[6]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/master?style=plastic
-[7]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
-[8]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
-[9]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...master
-[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
-[12]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[13]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[14]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[16]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[17]: https://github.com/realazthat/mdremotifier/tree/master
-[18]: https://github.com/realazthat/mdremotifier/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
-[19]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
-[20]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md
-[22]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/logo-exported.svg
-[23]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]: https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]: https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]: https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
-[60]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[1]: https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/logo-exported.svg
+[2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[4]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.0/LICENSE.md
+[7]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdremotifier/
+[9]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdremotifier/tree/master
+[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
+[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/master?style=plastic
+[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...master
+[15]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
+[16]: https://github.com/realazthat/mdremotifier/tree/develop
+[17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
+[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[22]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
+[23]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
+[24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
+[25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
+[26]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
+[27]: https://github.com/jen6/imgo "Upload to Google Drive"
+[28]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
+[29]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[30]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
+[31]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
```

#### html2text {}

```diff
@@ -1,181 +1,161 @@
 #
-                              ![mdremotifier][22]
-     ************ wwaarrnniinngg __TTHHIISS PPRROOJJEECCTT IISS AALLPPHHAA^^AALLPPHHAA,, NNOOTT RREEAADDYY FFOORR UUSSEE ************
-          ![**Audience:** Developers][19] ![**Platform:** Linux][20]
+                              ![mdremotifier][1]
+           ![**Audience:** Developers][2] ![**Platform:** Linux][3]
  _?ð_?_?_?_FF_ee_aa_tt_uu_rr_ee_ss ? ?•?  _?ð_?_?_? _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ? ?•?  _?ð_?_?_?_UU_ss_aa_gg_ee ? ?•?  _?ð_?_?_?»_CC_LL_II ? ?•?  _?ð_?_?_?¡_EE_xx_aa_mm_pp_ll_ee_ss
                               ? ?•?  _?â_?_?_RR_ee_qq_uu_ii_rr_ee_mm_ee_nn_tt_ss
-  ![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5] [!
-    [Python Version][8]][5] **CLI to replace `./image.png` to remote URL in
-                                  README.md**
+   ![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8] [!
+           [Python Version][9]][8] **CLI to replace `./image.png` to
+             `raw.githubusercontent.com` remote URL in README.md**
 ---
 | | Status | Stable | Unstable | | | ----------------- | ----------------------
----- | ------------------------- | ------------------------- | ----------------
--- | | **[Master][17]** | [![Build and Test][1]][2] | [![since tagged][6]][10]
- | | ![last commit][7] | | **[Develop][18]** | [![Build and Test][11]][2] | [!
-  [since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+----- | ------------------------- | ------------------------- | ---------------
+--- | | **[Master][10]** | [![Build and Test][11]][12] | [![since tagged][13]]
+[14] | | ![last commit][15] | | **[Develop][16]** | [![Build and Test][17]][12]
+| [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 [Demo]## â What What mdremotifier does: Turn this ([./mdremotifier/examples/
-EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/
+EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/
 mdremotifier/examples/EXAMPLE.md)): ```md # Example markdown file A link to a
 local file [LICENSE.md](./LICENSE.md). ``` Into this ([./mdremotifier/examples/
-EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/
-mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md)): ```md #
+EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/
+mdremotifier/examples/EXAMPLE.remotified.md)): ```md # Example markdown file A
+link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/
+mdremotifier/master/LICENSE.md). ``` This is useful for uploading `README.md`
+files to third-party sites, like the npmjs.com registry, or pypi.org registry,
+because these registries will break the local images in your README when
+displayed on their sites. ## ð Features - ð·ðð¡ðð¼ï¸ Replace
+local URLs with raw.githubusercontent.com URLs. ## ð  Installation ```bash #
+Install from pypi (https://pypi.org/project/mdremotifier/) pip install
+mdremotifier # Install from git (https://github.com/realazthat/mdremotifier)
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.0 ``` ##
+ð Usage Example README: ([./mdremotifier/examples/EXAMPLE.md](https://
+github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/
+EXAMPLE.md)): ```md # Example markdown file A link to a local file [LICENSE.md]
+(./LICENSE.md). ``` Generating the README: ```bash $ python -m mdremotifier.cli
+-i ./mdremotifier/examples/EXAMPLE.md --url-prefix https://
+raw.githubusercontent.com/realazthat/mdremotifier/master/ -o - 2>/dev/null #
 Example markdown file A link to a local file [LICENSE.md](https://
-raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md). ``` This
-is useful for uploading `README.md` files to third-party sites, like the
-npmjs.com registry, or pypi.org registry, because these registries will break
-the local images in your README when displayed on their sites. ## ð Features
-- ð·ðð¡ðð¼ï¸ Replace local URLs with raw.githubusercontent.com
-URLs. ## ð  Installation ```bash # Install from pypi (https://pypi.org/
-project/mdremotifier/) pip install mdremotifier # Install from git (https://
-github.com/realazthat/mdremotifier) pip install git+https://github.com/
-realazthat/mdremotifier.git@v0.2.0 ``` ## ð Usage Example README: ([./
-mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/
-mdremotifier/master/mdremotifier/examples/EXAMPLE.md)): ```md # Example
-markdown file A link to a local file [LICENSE.md](./LICENSE.md). ``` Generating
-the README: ```bash $ python -m mdremotifier.cli -i ./mdremotifier/examples/
-EXAMPLE.md --url-prefix https://raw.githubusercontent.com/realazthat/
-mdremotifier/master/ -o - 2>/dev/null # Example markdown file A link to a local
-file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/
-master/LICENSE.md). ``` ## ð» Command Line Options [Output of `python -
-m mdremotifier.cli --help`]## ð¡ Examples - mdremotifier's own `README`: -
-Original: [./README.md](https://raw.githubusercontent.com/realazthat/
-mdremotifier/master/README.md). - Remotified: [./.github/README.remotified.md]
-(https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/
-README.remotified.md). - Generation script: [./scripts/generate-readme.sh]
-(https://raw.githubusercontent.com/realazthat/mdremotifier/master/scripts/
-generate-readme.sh). - Example: - Original: [./mdremotifier/examples/
-EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/
+raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md). ``` ##
+ð» Command Line Options [Output of `python -m mdremotifier.cli --help`]##
+ð¡ Examples - mdremotifier's own `README`: - Original: [./README.md](https://
+github.com/realazthat/mdremotifier/blob/v0.3.0/README.md). - Remotified:
+[./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/
+blob/v0.3.0/.github/README.remotified.md). - Generation script: [./scripts/
+generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/
+scripts/generate-readme.sh). - Example: - Original: [./mdremotifier/examples/
+EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/
 mdremotifier/examples/EXAMPLE.md). - Remotified: [./mdremotifier/examples/
-EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/
-mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md). - Generation
-script: [./mdremotifier/examples/example.sh](https://raw.githubusercontent.com/
-realazthat/mdremotifier/master/mdremotifier/examples/example.sh). ## â
-Requirements - Linux-like environment - Why: Uses pexpect.spawn(). - Python
-3.8+ - Why: Some dev dependencies require Python 3.8+. ### Tested Platforms -
-WSL2 Ubuntu 20.04, Python `3.8.0`. - Ubuntu 20.04, Python `3.8.0, 3.9.0,
-3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions workflow ([build-and-
-test.yml](https://raw.githubusercontent.com/realazthat/mdremotifier/
-master/.github/workflows/build-and-test.yml)). ## ð¤ Versioning We use SemVer
-for versioning. For the versions available, see the tags on this repository. ##
-ð License This project is licensed under the MIT License - see the [./
-LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/
-LICENSE.md) file for details. ## ð Thanks Main libraries used in
-mdremotifier are: - Markdown AST: [mistletoe](https://github.com/miyuchina/
-mistletoe). - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/
-rich-argparse). ## ð¤ Related Projects Not complete, and not necessarily up
-to date. Make a PR ([contributions](#-contributions)) to insert/modify. |
-Project | Stars | Last Update | Language | Platform | Similarity X Obviousness
-| | ------------------------------------------------- | ----- | ------------ |
--------- | -------- | ------------------------ | | [bdashore3/remark-github-
-images][60] | 0 | `2022/12/29` | JS | CLI | â­â­â­â­â­ | | [laobie/
-WriteMarkdownLazily][54] | 36 | `2024/01/06` | Python | CLI | â­â­â­â­ | |
-[crh19970307/mdul][55] | 1 | `2020/02/01` | Python | CLI | â­â­â­â­ | |
-[SkyLee424/Go-MarkDown-Image-Transfer-Helper][56] | 0 | `2024/03/25` | Go | CLI
-| â­â­â­â­ | | [jen6/imgo][57] | 0 | `2020/03/18` | Pyhon | CLI |
-â­â­â­â­ | | [chocoluffy/lazy-markdown][59] | 0 | `2016/11/20` | Python |
-CLI | â­â­â­â­ | | [loheagn/gopic][61] | 0 | `2021/11/24` | Go | CLI |
-â­â­â­â­ | | [Undertone0809/imarkdown][53] | 57 | `2024/01/06` | Python |
-Python | â­â­â­ | | [ravgeetdhillon/markdown-imgur-upload][58] | 1 | `2022/
-03/26` | Python | CLI | â­â­â­ | ## ð«¡ Contributions ### Development
-environment: Linux-like - For running `pre.sh` (Linux-like environment). -
-Requires `pyenv`, or an exact matching version of python as in [.python-
-version](https://raw.githubusercontent.com/realazthat/mdremotifier/
-master/.python-version) (which is currently `3.8.0 `). - `jq`, ([installation]
+EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/
+mdremotifier/examples/EXAMPLE.remotified.md). - Generation script: [./
+mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/
+blob/v0.3.0/mdremotifier/examples/example.sh). ## â Requirements - Linux-like
+environment - Why: Uses pexpect.spawn(). - Python 3.8+ - Why: Some dev
+dependencies require Python 3.8+. ### Tested Platforms - WSL2 Ubuntu 20.04,
+Python `3.8.0`. - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`,
+tested in GitHub Actions workflow ([build-and-test.yml](https://github.com/
+realazthat/mdremotifier/blob/v0.3.0/.github/workflows/build-and-test.yml)). ##
+ð¤ Versioning We use SemVer for versioning. For the versions available, see
+the tags on this repository. ## ð License This project is licensed under the
+MIT License - see the [./LICENSE.md](https://github.com/realazthat/
+mdremotifier/blob/v0.3.0/LICENSE.md) file for details. ## ð Thanks Main
+libraries used in mdremotifier are: - Markdown AST: [mistletoe](https://
+github.com/miyuchina/mistletoe). - Colorful CLI help: [rich-argparse](https://
+github.com/hamdanal/rich-argparse). ## ð¤ Related Projects Not complete, and
+not necessarily up to date. Make a PR ([contributions](#-contributions)) to
+insert/modify. | Project | Stars | Last Update | Language | Platform |
+Similarity X Obviousness | | ------------------------------------------------
+- | ----- | ------------ | -------- | -------- | ------------------------ | |
+[bdashore3/remark-github-images][23] | 0 | `2022/12/29` | JS | CLI |
+â­â­â­â­â­ | | [laobie/WriteMarkdownLazily][24] | 36 | `2024/01/06` |
+Python | CLI | â­â­â­â­ | | [crh19970307/mdul][25] | 1 | `2020/02/01` |
+Python | CLI | â­â­â­â­ | | [SkyLee424/Go-MarkDown-Image-Transfer-Helper]
+[26] | 0 | `2024/03/25` | Go | CLI | â­â­â­â­ | | [jen6/imgo][27] | 0 |
+`2020/03/18` | Pyhon | CLI | â­â­â­â­ | | [chocoluffy/lazy-markdown][28] |
+0 | `2016/11/20` | Python | CLI | â­â­â­â­ | | [loheagn/gopic][29] | 0 |
+`2021/11/24` | Go | CLI | â­â­â­â­ | | [Undertone0809/imarkdown][30] | 57 |
+`2024/01/06` | Python | Python | â­â­â­ | | [ravgeetdhillon/markdown-imgur-
+upload][31] | 1 | `2022/03/26` | Python | CLI | â­â­â­ | ## ð«¡
+Contributions ### Development environment: Linux-like - For running `pre.sh`
+(Linux-like environment). - From [./.github/dependencies.yml](https://
+github.com/realazthat/mdremotifier/blob/v0.3.0/.github/dependencies.yml), which
+is used for the GH Action to do a fresh install of everything: ```yaml bash:
+scripts. findutils: scripts. grep: tests. xxd: tests. git: scripts, tests.
+xxhash: scripts (changeguard). rsync: out-of-directory test. expect: for
+`unbuffer`, useful to grab and compare ansi color symbols. jq: dependency for
+[yq](https://github.com/kislyuk/yq), which is used to generate the README; the
+README generator needs to use `tomlq` (which is a part of `yq`) to query
+`pyproject.toml`. ``` - Requires `pyenv`, or an exact matching version of
+python as in [.python-version](https://github.com/realazthat/mdremotifier/blob/
+v0.3.0/.python-version) (which is currently `3.8.0 `). - `jq`, ([installation]
 (https://jqlang.github.io/jq/)) required for [yq](https://github.com/kislyuk/
-yq), which is itself required for our [./README.md](https://
-raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) generation,
-which uses `tomlq` (from the [yq](https://github.com/kislyuk/yq) package) to
-include version strings from [./pyproject.toml](https://
-raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml). -
-`bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash`, `rsync` (for tests/
-workflows). - Requires nodejs (for act). - Requires Go (to run act). - docker
-(for act, animation). ### Commit Process 1. (Optionally) Fork the `develop`
-branch. 2. Stage your files: `git add path/to/file.py`. 3. `bash ./scripts/
-pre.sh`, this will format, lint, and test the code. 4. `git status` check if
-anything changed (generated [./README.md](https://raw.githubusercontent.com/
-realazthat/mdremotifier/master/README.md) for example), if so, `git add` the
-changes, and go back to the previous step. 5. `git commit -m "..."`. 6. Make a
-PR to `develop` (or push to develop if you have the rights). ## ðð
-Release Process These instructions are for maintainers of the project. 1. In
-the `develop` branch, run `bash ./scripts/pre.sh` to ensure everything is in
-order. 2. In the `develop` branch, bump the version in [./pyproject.toml]
-(https://raw.githubusercontent.com/realazthat/mdremotifier/master/
-pyproject.toml), following semantic versioning principles. Also modify the
-`last_unstable_release` and `last_stable_release` in the `[tool.mdremotifier-
-project-metadata]` table as appropriate. Run `bash ./scripts/pre.sh` to ensure
-everything is in order. 3. In the `develop` branch, commit these changes with a
-message like `"Prepare release X.Y.Z"`. (See the contributions section [above]
-(#commit-process)). 4. Merge the `develop` branch into the `master` branch:
-`git checkout master && git merge develop --no-ff`. 5. `master` branch: Tag the
-release: Create a git tag for the release with `git tag -a vX.Y.Z -m "Version
-X.Y.Z"`. 6. Publish to PyPI: Publish the release to PyPI with `bash ./scripts/
-deploy-to-pypi.sh`. 7. Push to GitHub: Push the commit and tags to GitHub with
-`git push && git push --tags`. 8. The `--no-ff` option adds a commit to the
-master branch for the merge, so refork the develop branch from the master
-branch: `git checkout develop && git merge master`. 9. Push the develop branch
-to GitHub: `git push origin develop`. [1]: https://img.shields.io/github/
-actions/workflow/status/realazthat/mdremotifier/build-and-
-test.yml?branch=master&style=plastic [2]: https://github.com/realazthat/
-mdremotifier/actions/workflows/build-and-test.yml [3]: https://img.shields.io/
-github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E [4]: https://
-img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E [5]: https://
-pypi.org/project/mdremotifier/ [6]: https://img.shields.io/github/commits-
-since/realazthat/mdremotifier/v0.2.0/master?style=plastic [7]: https://
-img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
-[8]: https://img.shields.io/pypi/pyversions/
-mdremotifier?style=plastic&color=0A1E1E [9]: https://img.shields.io/github/
-languages/top/realazthat/
-mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [10]: https://
-github.com/realazthat/mdremotifier/compare/v0.2.0...master [11]: https://
-img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-
-and-test.yml?branch=develop&style=plastic [12]: https://img.shields.io/github/
-commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic [13]: https:
-//github.com/realazthat/mdremotifier/compare/v0.2.0...develop [14]: https://
-img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/
-v0.2.0/develop?style=plastic [16]: https://github.com/realazthat/mdremotifier/
-compare/v0.2.0...develop [17]: https://github.com/realazthat/mdremotifier/tree/
-master [18]: https://github.com/realazthat/mdremotifier/tree/develop [19]:
+yq), which is itself required for our [./README.md](https://github.com/
+realazthat/mdremotifier/blob/v0.3.0/README.md) generation, which uses `tomlq`
+(from the [yq](https://github.com/kislyuk/yq) package) to include version
+strings from [./pyproject.toml](https://github.com/realazthat/mdremotifier/
+blob/v0.3.0/pyproject.toml). - act (to run the GH Action locally): - Requires
+nodejs. - Requires Go. - docker. - Generate animation: - docker ### Commit
+Process 1. (Optionally) Fork the `develop` branch. 2. Stage your files: `git
+add path/to/file.py`. 3. `bash ./scripts/pre.sh`, this will format, lint, and
+test the code. 4. `git status` check if anything changed (generated [./
+README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md)
+for example), if so, `git add` the changes, and go back to the previous step.
+5. `git commit -m "..."`. 6. Make a PR to `develop` (or push to develop if you
+have the rights). ## ðð Release Process These instructions are for
+maintainers of the project. 1. In the `develop` branch, run `bash ./scripts/
+pre.sh` to ensure everything is in order. 2. In the `develop` branch, bump the
+version in [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/
+v0.3.0/pyproject.toml), following semantic versioning principles. Also modify
+the `last_unstable_release` and `last_stable_release` in the `
+[tool.mdremotifier-project-metadata]` table as appropriate. Run `bash ./
+scripts/pre.sh` to ensure everything is in order. 3. In the `develop` branch,
+commit these changes with a message like `"Prepare release X.Y.Z"`. (See the
+contributions section [above](#commit-process)). 4. Merge the `develop` branch
+into the `master` branch: `git checkout master && git merge develop --no-ff`.
+5. `master` branch: Tag the release: Create a git tag for the release with `git
+tag -a vX.Y.Z -m "Version X.Y.Z"`. 6. Publish to PyPI: Publish the release to
+PyPI with `bash ./scripts/deploy-to-pypi.sh`. 7. Push to GitHub: Push the
+commit and tags to GitHub with `git push && git push --tags`. 8. The `--no-ff`
+option adds a commit to the master branch for the merge, so refork the develop
+branch from the master branch: `git checkout develop && git merge master`. 9.
+Push the develop branch to GitHub: `git push origin develop`. [1]: https://
+github.com/realazthat/mdremotifier/blob/v0.3.0/.github/logo-exported.svg [2]:
 https://img.shields.io/badge/Audience-Developers-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-[20]: https://img.shields.io/badge/Platform-Linux-
+[3]: https://img.shields.io/badge/Platform-Linux-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/
-LICENSE.md [22]: https://raw.githubusercontent.com/realazthat/mdremotifier/
-master/.github/logo-exported.svg [23]: https://docs.github.com/en/get-started/
-writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-
-to-a-code-snippet [24]: https://github.com/zakhenry/embedme [25]: https://
-github.com/electrovir/markdown-code-example-inserter [26]: https://github.com/
-dineshsonachalam/markdown-autodocs [27]: https://github.com/romnn/embedme [28]:
-https://github.com/drewavis/markdowninclude [29]: https://github.com/tokusumi/
-markdown-embed-code [30]: https://github.com/ARMmbed/snippet [31]: https://
-github.com/SimonCropp/MarkdownSnippets [32]: https://github.com/shiftkey/
-scribble [33]: https://github.com/shiftkey/scribble/blob/master/docs/features/
-code-snippets.md [34]: https://github.com/JulianCataldo/remark-embed [35]:
-https://github.com/calebpeterson/jest-transformer-test-md [36]: https://
-github.com/ildar-shaimordanov/git-markdown-snippet [37]: https://github.com/
-sammndhr/gridsome-remark-embed-snippet [38]: https://gridsome.org/ [39]: https:
-//github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby [41]: https://github.com/endocode/
-snippetextractor [42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc [44]: https://github.com/
-NativeScript/markdown-snippet-injector [45]: https://github.com/polywrap/doc-
-snippets [46]: https://github.com/andersfischernielsen/Simple-Embedded-
-Markdown-Code-Snippets [47]: https://github.com/xrd/oreilly-snippets [48]:
-https://github.com/DamonOehlman/injectcode [49]: https://github.com/fuxingloh/
-remark-code-import-replace [50]: https://github.com/teyc/markdown-snippet [51]:
-https://github.com/marc-bouvier-graveyard/baldir_markdown [52]: https://
-github.com/tjstankus/commitate [53]: https://github.com/Undertone0809/imarkdown
-"Doesn't yet have a CLI." [54]: https://github.com/laobie/WriteMarkdownLazily
-"Uploads to cloud." [55]: https://github.com/crh19970307/mdul "Uploads to
-sm.ms" [56]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper
-"Upload to Qiniu Cloud" [57]: https://github.com/jen6/imgo "Upload to Google
-Drive" [58]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to
-imgur, a bit annoying because it requires you to put the images into a
-particular directory" [59]: https://github.com/chocoluffy/lazy-markdown
-"Uploads to LeanCloud, readme is a bit unclear" [60]: https://github.com/
-bdashore3/remark-github-images "Documentation is non-existent, but code looks
-very similar to mdremotifier" [61]: https://github.com/loheagn/gopic "Upload to
-cloud, not clear which cloud"
+[4]: https://img.shields.io/github/languages/top/realazthat/
+mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [5]: https://
+img.shields.io/github/license/realazthat/
+mdremotifier?style=plastic&color=0A1E1E [6]: https://github.com/realazthat/
+mdremotifier/blob/v0.3.0/LICENSE.md [7]: https://img.shields.io/pypi/v/
+mdremotifier?style=plastic&color=0A1E1E [8]: https://pypi.org/project/
+mdremotifier/ [9]: https://img.shields.io/pypi/pyversions/
+mdremotifier?style=plastic&color=0A1E1E [10]: https://github.com/realazthat/
+mdremotifier/tree/master [11]: https://img.shields.io/github/actions/workflow/
+status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-
+test.yml [13]: https://img.shields.io/github/commits-since/realazthat/
+mdremotifier/v0.3.0/master?style=plastic [14]: https://github.com/realazthat/
+mdremotifier/compare/v0.3.0...master [15]: https://img.shields.io/github/last-
+commit/realazthat/mdremotifier/master?style=plastic [16]: https://github.com/
+realazthat/mdremotifier/tree/develop [17]: https://img.shields.io/github/
+actions/workflow/status/realazthat/mdremotifier/build-and-
+test.yml?branch=develop&style=plastic [18]: https://img.shields.io/github/
+commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic [19]: https:
+//github.com/realazthat/mdremotifier/compare/v0.3.0...develop [20]: https://
+img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/
+develop?style=plastic [21]: https://github.com/realazthat/mdremotifier/compare/
+v0.3.0...develop [22]: https://img.shields.io/github/last-commit/realazthat/
+mdremotifier/develop?style=plastic [23]: https://github.com/bdashore3/remark-
+github-images "Documentation is non-existent, but code looks very similar to
+mdremotifier" [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to
+cloud." [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms" [26]:
+https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu
+Cloud" [27]: https://github.com/jen6/imgo "Upload to Google Drive" [28]: https:
+//github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit
+unclear" [29]: https://github.com/loheagn/gopic "Upload to cloud, not clear
+which cloud" [30]: https://github.com/Undertone0809/imarkdown "Doesn't yet have
+a CLI." [31]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload
+to imgur, a bit annoying because it requires you to put the images into a
+particular directory"
```

### Comparing `mdremotifier-0.2.0/LICENSE.md` & `mdremotifier-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdremotifier-0.2.0/PKG-INFO` & `mdremotifier-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdremotifier
-Version: 0.2.0
+Version: 0.3.0
 Summary: Remotify local links in README.md.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -62,54 +62,78 @@
 Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == "prod"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
 Requires-Dist: types-html5lib==1.1.11.20240228; extra == "prod"
 Requires-Dist: typing-extensions==4.11.0; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.3.0; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
+Requires-Dist: backports-tarfile==1.1.1; extra == "dev"
 Requires-Dist: beautifulsoup4==4.12.3; extra == "dev"
 Requires-Dist: bs4==0.0.2; extra == "dev"
+Requires-Dist: certifi==2024.2.2; extra == "dev"
+Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: changeguard==0.3.1; extra == "dev"
+Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
+Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: defusedxml==0.7.1; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
+Requires-Dist: docutils==0.20.1; extra == "dev"
 Requires-Dist: filelock==3.13.4; extra == "dev"
 Requires-Dist: identify==2.5.36; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: idna==3.7; extra == "dev"
 Requires-Dist: importlib-metadata==7.1.0; extra == "dev"
+Requires-Dist: importlib-resources==6.4.0; extra == "dev"
+Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: jaraco-classes==3.4.0; extra == "dev"
+Requires-Dist: jaraco-context==5.3.0; extra == "dev"
+Requires-Dist: jaraco-functools==4.0.1; extra == "dev"
+Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
+Requires-Dist: keyring==25.2.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
 Requires-Dist: mistletoe==1.3.0; extra == "dev"
+Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
+Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
 Requires-Dist: pexpect==4.9.0; extra == "dev"
+Requires-Dist: pkginfo==1.10.0; extra == "dev"
 Requires-Dist: platformdirs==4.2.1; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: ptyprocess==0.7.0; extra == "dev"
+Requires-Dist: pycparser==2.22; extra == "dev"
 Requires-Dist: pyflakes==3.2.0; extra == "dev"
 Requires-Dist: pygments==2.17.2; extra == "dev"
 Requires-Dist: pyright==1.1.352; extra == "dev"
 Requires-Dist: pyyaml==6.0.1; extra == "dev"
+Requires-Dist: readme-renderer==43.0; extra == "dev"
+Requires-Dist: requests==2.31.0; extra == "dev"
+Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
+Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
-Requires-Dist: snipinator==1.3.1; extra == "dev"
+Requires-Dist: secretstorage==3.3.3; extra == "dev"
+Requires-Dist: snipinator==1.4.0; extra == "dev"
 Requires-Dist: soupsieve==2.5; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
 Requires-Dist: types-html5lib==1.1.11.20240228; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
+Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.26.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
 Requires-Dist: yq==3.2.3; extra == "dev"
 Requires-Dist: zipp==3.18.1; extra == "dev"
 
 <!--
@@ -124,28 +148,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdremotifier][22]</div>
+# <div align="center">![mdremotifier][1]</div>
 
 <div align="center">
 
-<h1>warning _THIS PROJECT IS ALPHA^ALPHA, NOT READY FOR USE</h1>
-
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -159,52 +181,52 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
-**CLI to replace `./image.png` to <raw.githubusercontent.com> remote URL in
+**CLI to replace `./image.png` to `raw.githubusercontent.com` remote URL in
 README.md**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img src="./.github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/0.3.0/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdremotifier does:
 
-Turn this ([./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md)):
+Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
 ```
 <!---->
 
 Into this
-([./mdremotifier/examples/EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md)):
+([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.remotified.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md).
 
@@ -222,20 +244,20 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.2.0
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md)):
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
@@ -253,29 +275,29 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m mdremotifier.cli --help`" />
-<!---->
+<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/0.3.0/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - mdremotifier's own `README`:
-  - Original: [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md).
-  - Remotified: [./.github/README.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/README.remotified.md).
-  - Generation script: [./scripts/generate-readme.sh](https://raw.githubusercontent.com/realazthat/mdremotifier/master/scripts/generate-readme.sh).
+  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md).
+  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/README.remotified.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/scripts/generate-readme.sh).
 - Example:
-  - Original: [./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md).
+  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md).
   - Remotified:
-    [./mdremotifier/examples/EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md).
+    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.remotified.md).
   - Generation script:
-    [./mdremotifier/examples/example.sh](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/example.sh).
+    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdremotifier
 - Projects using mdremotifier:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -298,25 +320,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdremotifier are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -324,62 +346,82 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ------------------------------------------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [bdashore3/remark-github-images][60]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
-| [laobie/WriteMarkdownLazily][54]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [crh19970307/mdul][55]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][56] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                     |
-| [jen6/imgo][57]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                     |
-| [chocoluffy/lazy-markdown][59]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [loheagn/gopic][61]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                     |
-| [Undertone0809/imarkdown][53]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                      |
-| [ravgeetdhillon/markdown-imgur-upload][58]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                      |
+| [bdashore3/remark-github-images][23]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
+| [laobie/WriteMarkdownLazily][24]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [crh19970307/mdul][25]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][26] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                     |
+| [jen6/imgo][27]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                     |
+| [chocoluffy/lazy-markdown][28]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [loheagn/gopic][29]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                     |
+| [Undertone0809/imarkdown][30]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                      |
+| [ravgeetdhillon/markdown-imgur-upload][31]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                      |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.python-version) (which is currently
     `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml).
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash`, `rsync` (for
-    tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act, animation).
+    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/pyproject.toml).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdremotifier-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -391,74 +433,38 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
-[2]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
-[3]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
-[4]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdremotifier/
-[6]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/master?style=plastic
-[7]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
-[8]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
-[9]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...master
-[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
-[12]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[13]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[14]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[16]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[17]: https://github.com/realazthat/mdremotifier/tree/master
-[18]: https://github.com/realazthat/mdremotifier/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
-[19]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
-[20]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md
-[22]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/logo-exported.svg
-[23]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]: https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]: https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]: https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
-[60]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[1]: https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/logo-exported.svg
+[2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[4]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.0/LICENSE.md
+[7]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdremotifier/
+[9]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdremotifier/tree/master
+[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
+[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/master?style=plastic
+[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...master
+[15]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
+[16]: https://github.com/realazthat/mdremotifier/tree/develop
+[17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
+[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[22]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
+[23]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
+[24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
+[25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
+[26]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
+[27]: https://github.com/jen6/imgo "Upload to Google Drive"
+[28]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
+[29]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[30]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
+[31]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
```

### Comparing `mdremotifier-0.2.0/README.md` & `mdremotifier-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdremotifier][22]</div>
+# <div align="center">![mdremotifier][1]</div>
 
 <div align="center">
 
-<h1>warning _THIS PROJECT IS ALPHA^ALPHA, NOT READY FOR USE</h1>
-
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -45,30 +43,30 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
-**CLI to replace `./image.png` to <raw.githubusercontent.com> remote URL in
+**CLI to replace `./image.png` to `raw.githubusercontent.com` remote URL in
 README.md**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
 <img src="./.github/demo.gif" alt="Demo" width="100%">
 
 ## ❔ What
 
@@ -108,15 +106,15 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.2.0
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
 Example README: ([./mdremotifier/examples/EXAMPLE.md](./mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
@@ -210,43 +208,63 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ------------------------------------------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [bdashore3/remark-github-images][60]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐               |
-| [laobie/WriteMarkdownLazily][54]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                 |
-| [crh19970307/mdul][55]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                 |
-| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][56] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                 |
-| [jen6/imgo][57]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                 |
-| [chocoluffy/lazy-markdown][59]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                 |
-| [loheagn/gopic][61]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                 |
-| [Undertone0809/imarkdown][53]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                   |
-| [ravgeetdhillon/markdown-imgur-upload][58]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                   |
+| [bdashore3/remark-github-images][23]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐               |
+| [laobie/WriteMarkdownLazily][24]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                 |
+| [crh19970307/mdul][25]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                 |
+| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][26] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                 |
+| [jen6/imgo][27]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                 |
+| [chocoluffy/lazy-markdown][28]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                 |
+| [loheagn/gopic][29]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                 |
+| [Undertone0809/imarkdown][30]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                   |
+| [ravgeetdhillon/markdown-imgur-upload][31]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                   |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+    
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
     [.python-version](.python-version) (which is currently
     `3.8.0
 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
     [./README.md](./README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
     [./pyproject.toml](./pyproject.toml).
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash`, `rsync` (for
-    tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act, animation).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
@@ -278,103 +296,63 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
+[1]: ./.github/logo-exported.svg
 [2]:
-  https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
+  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [3]:
-  https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
+  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [4]:
-  https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdremotifier/
-[6]:
-  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/master?style=plastic
+  https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]:
+  https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
+[6]: ./LICENSE.md
 [7]:
-  https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
-[8]:
-  https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
+  https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdremotifier/
 [9]:
-  https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]:
-  https://github.com/realazthat/mdremotifier/compare/v0.2.0...master
+  https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdremotifier/tree/master
 [11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
+  https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
+  https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
 [13]:
-  https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
+  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/master?style=plastic
 [14]:
-  https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
+  https://github.com/realazthat/mdremotifier/compare/v0.3.0...master
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[16]:
-  https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[17]: https://github.com/realazthat/mdremotifier/tree/master
-[18]: https://github.com/realazthat/mdremotifier/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
+  https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
+[16]: https://github.com/realazthat/mdremotifier/tree/develop
+[17]:
+  https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
+[18]:
+  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
 [19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
+  https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
 [20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
+  https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[21]:
+  https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[22]:
+  https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
 [23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
-  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]:
+  https://github.com/bdashore3/remark-github-images
+  "Documentation is non-existent, but code looks very similar to mdremotifier"
+[24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
+[25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
+[26]:
   https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper
   "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]:
-  https://github.com/ravgeetdhillon/markdown-imgur-upload
-  "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]:
+[27]: https://github.com/jen6/imgo "Upload to Google Drive"
+[28]:
   https://github.com/chocoluffy/lazy-markdown
   "Uploads to LeanCloud, readme is a bit unclear"
-[60]:
-  https://github.com/bdashore3/remark-github-images
-  "Documentation is non-existent, but code looks very similar to mdremotifier"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[29]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[30]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
+[31]:
+  https://github.com/ravgeetdhillon/markdown-imgur-upload
+  "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
 #
-                              ![mdremotifier][22]
-     ************ wwaarrnniinngg __TTHHIISS PPRROOJJEECCTT IISS AALLPPHHAA^^AALLPPHHAA,, NNOOTT RREEAADDYY FFOORR UUSSEE ************
-          ![**Audience:** Developers][19] ![**Platform:** Linux][20]
+                              ![mdremotifier][1]
+           ![**Audience:** Developers][2] ![**Platform:** Linux][3]
  _?ð_?_?_?_FF_ee_aa_tt_uu_rr_ee_ss ? ?•?  _?ð_?_?_? _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ? ?•?  _?ð_?_?_?_UU_ss_aa_gg_ee ? ?•?  _?ð_?_?_?»_CC_LL_II ? ?•?  _?ð_?_?_?¡_EE_xx_aa_mm_pp_ll_ee_ss
                               ? ?•?  _?â_?_?_RR_ee_qq_uu_ii_rr_ee_mm_ee_nn_tt_ss
-  ![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5] [!
-    [Python Version][8]][5] **CLI to replace `./image.png` to remote URL in
-                                  README.md**
+   ![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8] [!
+           [Python Version][9]][8] **CLI to replace `./image.png` to
+             `raw.githubusercontent.com` remote URL in README.md**
 ---
 | | Status | Stable | Unstable | | | ----------------- | ----------------------
----- | ------------------------- | ------------------------- | ----------------
--- | | **[Master][17]** | [![Build and Test][1]][2] | [![since tagged][6]][10]
- | | ![last commit][7] | | **[Develop][18]** | [![Build and Test][11]][2] | [!
-  [since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+----- | ------------------------- | ------------------------- | ---------------
+--- | | **[Master][10]** | [![Build and Test][11]][12] | [![since tagged][13]]
+[14] | | ![last commit][15] | | **[Develop][16]** | [![Build and Test][17]][12]
+| [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 [Demo]## â What What mdremotifier does: Turn this ([./mdremotifier/examples/
 EXAMPLE.md](./mdremotifier/examples/EXAMPLE.md)): ```md # Example markdown file
 A link to a local file [LICENSE.md](./LICENSE.md). ``` Into this ([./
 mdremotifier/examples/EXAMPLE.remotified.md](./mdremotifier/examples/
 EXAMPLE.remotified.md)): ```md # Example markdown file A link to a local file
 [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/
 LICENSE.md). ``` This is useful for uploading `README.md` files to third-party
 sites, like the npmjs.com registry, or pypi.org registry, because these
 registries will break the local images in your README when displayed on their
 sites. ## ð Features - ð·ðð¡ðð¼ï¸ Replace local URLs with
 raw.githubusercontent.com URLs. ## ð  Installation ```bash # Install from
 pypi (https://pypi.org/project/mdremotifier/) pip install mdremotifier #
 Install from git (https://github.com/realazthat/mdremotifier) pip install
-git+https://github.com/realazthat/mdremotifier.git@v0.2.0 ``` ## ð Usage
+git+https://github.com/realazthat/mdremotifier.git@v0.3.0 ``` ## ð Usage
 Example README: ([./mdremotifier/examples/EXAMPLE.md](./mdremotifier/examples/
 EXAMPLE.md)): ```md # Example markdown file A link to a local file [LICENSE.md]
 (./LICENSE.md). ``` Generating the README: ```bash $ python -m mdremotifier.cli
 -i ./mdremotifier/examples/EXAMPLE.md --url-prefix https://
 raw.githubusercontent.com/realazthat/mdremotifier/master/ -o - 2>/dev/null #
 Example markdown file A link to a local file [LICENSE.md](https://
 raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md). ``` ##
@@ -53,112 +52,96 @@
 Thanks Main libraries used in mdremotifier are: - Markdown AST: [mistletoe]
 (https://github.com/miyuchina/mistletoe). - Colorful CLI help: [rich-argparse]
 (https://github.com/hamdanal/rich-argparse). ## ð¤ Related Projects Not
 complete, and not necessarily up to date. Make a PR ([contributions](#-
 contributions)) to insert/modify. | Project | Stars | Last Update | Language |
 Platform | Similarity X Obviousness | | ---------------------------------------
 ---------- | ----- | ------------ | -------- | -------- | ---------------------
---- | | [bdashore3/remark-github-images][60] | 0 | `2022/12/29` | JS | CLI |
-â­â­â­â­â­ | | [laobie/WriteMarkdownLazily][54] | 36 | `2024/01/06` |
-Python | CLI | â­â­â­â­ | | [crh19970307/mdul][55] | 1 | `2020/02/01` |
+--- | | [bdashore3/remark-github-images][23] | 0 | `2022/12/29` | JS | CLI |
+â­â­â­â­â­ | | [laobie/WriteMarkdownLazily][24] | 36 | `2024/01/06` |
+Python | CLI | â­â­â­â­ | | [crh19970307/mdul][25] | 1 | `2020/02/01` |
 Python | CLI | â­â­â­â­ | | [SkyLee424/Go-MarkDown-Image-Transfer-Helper]
-[56] | 0 | `2024/03/25` | Go | CLI | â­â­â­â­ | | [jen6/imgo][57] | 0 |
-`2020/03/18` | Pyhon | CLI | â­â­â­â­ | | [chocoluffy/lazy-markdown][59] |
-0 | `2016/11/20` | Python | CLI | â­â­â­â­ | | [loheagn/gopic][61] | 0 |
-`2021/11/24` | Go | CLI | â­â­â­â­ | | [Undertone0809/imarkdown][53] | 57 |
+[26] | 0 | `2024/03/25` | Go | CLI | â­â­â­â­ | | [jen6/imgo][27] | 0 |
+`2020/03/18` | Pyhon | CLI | â­â­â­â­ | | [chocoluffy/lazy-markdown][28] |
+0 | `2016/11/20` | Python | CLI | â­â­â­â­ | | [loheagn/gopic][29] | 0 |
+`2021/11/24` | Go | CLI | â­â­â­â­ | | [Undertone0809/imarkdown][30] | 57 |
 `2024/01/06` | Python | Python | â­â­â­ | | [ravgeetdhillon/markdown-imgur-
-upload][58] | 1 | `2022/03/26` | Python | CLI | â­â­â­ | ## ð«¡
+upload][31] | 1 | `2022/03/26` | Python | CLI | â­â­â­ | ## ð«¡
 Contributions ### Development environment: Linux-like - For running `pre.sh`
-(Linux-like environment). - Requires `pyenv`, or an exact matching version of
-python as in [.python-version](.python-version) (which is currently `3.8.0 `).
-- `jq`, ([installation](https://jqlang.github.io/jq/)) required for [yq](https:
-//github.com/kislyuk/yq), which is itself required for our [./README.md](./
-README.md) generation, which uses `tomlq` (from the [yq](https://github.com/
-kislyuk/yq) package) to include version strings from [./pyproject.toml](./
-pyproject.toml). - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash`, `rsync`
-(for tests/workflows). - Requires nodejs (for act). - Requires Go (to run act).
-- docker (for act, animation). ### Commit Process 1. (Optionally) Fork the
-`develop` branch. 2. Stage your files: `git add path/to/file.py`. 3. `bash ./
-scripts/pre.sh`, this will format, lint, and test the code. 4. `git status`
-check if anything changed (generated [./README.md](./README.md) for example),
-if so, `git add` the changes, and go back to the previous step. 5. `git commit
--m "..."`. 6. Make a PR to `develop` (or push to develop if you have the
-rights). ## ðð Release Process These instructions are for maintainers of
-the project. 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
-everything is in order. 2. In the `develop` branch, bump the version in [./
-pyproject.toml](./pyproject.toml), following semantic versioning principles.
-Also modify the `last_unstable_release` and `last_stable_release` in the `
-[tool.mdremotifier-project-metadata]` table as appropriate. Run `bash ./
-scripts/pre.sh` to ensure everything is in order. 3. In the `develop` branch,
-commit these changes with a message like `"Prepare release X.Y.Z"`. (See the
-contributions section [above](#commit-process)). 4. Merge the `develop` branch
-into the `master` branch: `git checkout master && git merge develop --no-ff`.
-5. `master` branch: Tag the release: Create a git tag for the release with `git
-tag -a vX.Y.Z -m "Version X.Y.Z"`. 6. Publish to PyPI: Publish the release to
-PyPI with `bash ./scripts/deploy-to-pypi.sh`. 7. Push to GitHub: Push the
-commit and tags to GitHub with `git push && git push --tags`. 8. The `--no-ff`
-option adds a commit to the master branch for the merge, so refork the develop
-branch from the master branch: `git checkout develop && git merge master`. 9.
-Push the develop branch to GitHub: `git push origin develop`. [1]: https://
-img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-
-and-test.yml?branch=master&style=plastic [2]: https://github.com/realazthat/
-mdremotifier/actions/workflows/build-and-test.yml [3]: https://img.shields.io/
-github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E [4]: https://
-img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E [5]: https://
-pypi.org/project/mdremotifier/ [6]: https://img.shields.io/github/commits-
-since/realazthat/mdremotifier/v0.2.0/master?style=plastic [7]: https://
-img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
-[8]: https://img.shields.io/pypi/pyversions/
-mdremotifier?style=plastic&color=0A1E1E [9]: https://img.shields.io/github/
-languages/top/realazthat/
-mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [10]: https://
-github.com/realazthat/mdremotifier/compare/v0.2.0...master [11]: https://
-img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-
-and-test.yml?branch=develop&style=plastic [12]: https://img.shields.io/github/
-commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic [13]: https:
-//github.com/realazthat/mdremotifier/compare/v0.2.0...develop [14]: https://
-img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/
-v0.2.0/develop?style=plastic [16]: https://github.com/realazthat/mdremotifier/
-compare/v0.2.0...develop [17]: https://github.com/realazthat/mdremotifier/tree/
-master [18]: https://github.com/realazthat/mdremotifier/tree/develop [19]:
+(Linux-like environment). - From [./.github/dependencies.yml](./.github/
+dependencies.yml), which is used for the GH Action to do a fresh install of
+everything: ```yaml bash: scripts. findutils: scripts. grep: tests. xxd: tests.
+git: scripts, tests. xxhash: scripts (changeguard). rsync: out-of-directory
+test. expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to
+generate the README; the README generator needs to use `tomlq` (which is a part
+of `yq`) to query `pyproject.toml`. ``` - Requires `pyenv`, or an exact
+matching version of python as in [.python-version](.python-version) (which is
+currently `3.8.0 `). - `jq`, ([installation](https://jqlang.github.io/jq/))
+required for [yq](https://github.com/kislyuk/yq), which is itself required for
+our [./README.md](./README.md) generation, which uses `tomlq` (from the [yq]
+(https://github.com/kislyuk/yq) package) to include version strings from [./
+pyproject.toml](./pyproject.toml). - act (to run the GH Action locally): -
+Requires nodejs. - Requires Go. - docker. - Generate animation: - docker ###
+Commit Process 1. (Optionally) Fork the `develop` branch. 2. Stage your files:
+`git add path/to/file.py`. 3. `bash ./scripts/pre.sh`, this will format, lint,
+and test the code. 4. `git status` check if anything changed (generated [./
+README.md](./README.md) for example), if so, `git add` the changes, and go back
+to the previous step. 5. `git commit -m "..."`. 6. Make a PR to `develop` (or
+push to develop if you have the rights). ## ðð Release Process These
+instructions are for maintainers of the project. 1. In the `develop` branch,
+run `bash ./scripts/pre.sh` to ensure everything is in order. 2. In the
+`develop` branch, bump the version in [./pyproject.toml](./pyproject.toml),
+following semantic versioning principles. Also modify the
+`last_unstable_release` and `last_stable_release` in the `[tool.mdremotifier-
+project-metadata]` table as appropriate. Run `bash ./scripts/pre.sh` to ensure
+everything is in order. 3. In the `develop` branch, commit these changes with a
+message like `"Prepare release X.Y.Z"`. (See the contributions section [above]
+(#commit-process)). 4. Merge the `develop` branch into the `master` branch:
+`git checkout master && git merge develop --no-ff`. 5. `master` branch: Tag the
+release: Create a git tag for the release with `git tag -a vX.Y.Z -m "Version
+X.Y.Z"`. 6. Publish to PyPI: Publish the release to PyPI with `bash ./scripts/
+deploy-to-pypi.sh`. 7. Push to GitHub: Push the commit and tags to GitHub with
+`git push && git push --tags`. 8. The `--no-ff` option adds a commit to the
+master branch for the merge, so refork the develop branch from the master
+branch: `git checkout develop && git merge master`. 9. Push the develop branch
+to GitHub: `git push origin develop`. [1]: ./.github/logo-exported.svg [2]:
 https://img.shields.io/badge/Audience-Developers-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-[20]: https://img.shields.io/badge/Platform-Linux-
+[3]: https://img.shields.io/badge/Platform-Linux-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md [22]: ./.github/logo-exported.svg [23]: https://
-docs.github.com/en/get-started/writing-on-github/working-with-advanced-
-formatting/creating-a-permanent-link-to-a-code-snippet [24]: https://
-github.com/zakhenry/embedme [25]: https://github.com/electrovir/markdown-code-
-example-inserter [26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme [28]: https://github.com/drewavis/
-markdowninclude [29]: https://github.com/tokusumi/markdown-embed-code [30]:
-https://github.com/ARMmbed/snippet [31]: https://github.com/SimonCropp/
-MarkdownSnippets [32]: https://github.com/shiftkey/scribble [33]: https://
-github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md [34]:
-https://github.com/JulianCataldo/remark-embed [35]: https://github.com/
-calebpeterson/jest-transformer-test-md [36]: https://github.com/ildar-
-shaimordanov/git-markdown-snippet [37]: https://github.com/sammndhr/gridsome-
-remark-embed-snippet [38]: https://gridsome.org/ [39]: https://github.com/
-gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet [40]: https://
-github.com/gatsbyjs/gatsby [41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises [43]: https://
-github.com/devincornell/pymddoc [44]: https://github.com/NativeScript/markdown-
-snippet-injector [45]: https://github.com/polywrap/doc-snippets [46]: https://
-github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets [47]:
-https://github.com/xrd/oreilly-snippets [48]: https://github.com/DamonOehlman/
-injectcode [49]: https://github.com/fuxingloh/remark-code-import-replace [50]:
-https://github.com/teyc/markdown-snippet [51]: https://github.com/marc-bouvier-
-graveyard/baldir_markdown [52]: https://github.com/tjstankus/commitate [53]:
-https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI." [54]:
-https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud." [55]: https:/
-/github.com/crh19970307/mdul "Uploads to sm.ms" [56]: https://github.com/
-SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud" [57]:
-https://github.com/jen6/imgo "Upload to Google Drive" [58]: https://github.com/
-ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because
-it requires you to put the images into a particular directory" [59]: https://
-github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit
-unclear" [60]: https://github.com/bdashore3/remark-github-images "Documentation
-is non-existent, but code looks very similar to mdremotifier" [61]: https://
-github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[4]: https://img.shields.io/github/languages/top/realazthat/
+mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [5]: https://
+img.shields.io/github/license/realazthat/
+mdremotifier?style=plastic&color=0A1E1E [6]: ./LICENSE.md [7]: https://
+img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E [8]: https://
+pypi.org/project/mdremotifier/ [9]: https://img.shields.io/pypi/pyversions/
+mdremotifier?style=plastic&color=0A1E1E [10]: https://github.com/realazthat/
+mdremotifier/tree/master [11]: https://img.shields.io/github/actions/workflow/
+status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-
+test.yml [13]: https://img.shields.io/github/commits-since/realazthat/
+mdremotifier/v0.3.0/master?style=plastic [14]: https://github.com/realazthat/
+mdremotifier/compare/v0.3.0...master [15]: https://img.shields.io/github/last-
+commit/realazthat/mdremotifier/master?style=plastic [16]: https://github.com/
+realazthat/mdremotifier/tree/develop [17]: https://img.shields.io/github/
+actions/workflow/status/realazthat/mdremotifier/build-and-
+test.yml?branch=develop&style=plastic [18]: https://img.shields.io/github/
+commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic [19]: https:
+//github.com/realazthat/mdremotifier/compare/v0.3.0...develop [20]: https://
+img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/
+develop?style=plastic [21]: https://github.com/realazthat/mdremotifier/compare/
+v0.3.0...develop [22]: https://img.shields.io/github/last-commit/realazthat/
+mdremotifier/develop?style=plastic [23]: https://github.com/bdashore3/remark-
+github-images "Documentation is non-existent, but code looks very similar to
+mdremotifier" [24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to
+cloud." [25]: https://github.com/crh19970307/mdul "Uploads to sm.ms" [26]:
+https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu
+Cloud" [27]: https://github.com/jen6/imgo "Upload to Google Drive" [28]: https:
+//github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit
+unclear" [29]: https://github.com/loheagn/gopic "Upload to cloud, not clear
+which cloud" [30]: https://github.com/Undertone0809/imarkdown "Doesn't yet have
+a CLI." [31]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload
+to imgur, a bit annoying because it requires you to put the images into a
+particular directory"
```

### Comparing `mdremotifier-0.2.0/mdremotifier/cli.py` & `mdremotifier-0.3.0/mdremotifier/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 """
 import argparse
 import logging
 import sys
 import warnings
 from pathlib import Path
 from shutil import get_terminal_size
-from typing import Dict, List, Optional
+from typing import List, Optional, Set
 from urllib.parse import ParseResult, urljoin, urlparse
 
 import colorama
 import mistletoe
 from bs4 import BeautifulSoup
 from mistletoe.markdown_renderer import (LinkReferenceDefinition,
                                          MarkdownRenderer)
-from mistletoe.span_token import HtmlSpan, Image, InlineCode, Link, SpanToken
+from mistletoe.span_token import (HtmlSpan, Image, InlineCode, Link, RawText,
+                                  SpanToken)
 from mistletoe.token import Token
 from rich.console import Console
 from rich_argparse import RichHelpFormatter
 
 from . import _build_version
 
 logger = logging.getLogger(__name__)
@@ -84,68 +85,77 @@
   path = Path(path_str)
   with path.open('w') as fout:
     fout.write(output)
 
 
 class _Updater:
 
-  def __init__(self, url_prefix: str, all_references: bool,
-               console: Console) -> None:
-    self._url_prefix = url_prefix
+  def __init__(self, link_url_prefix: str, img_url_prefix: str,
+               all_references: bool, console: Console) -> None:
+    self._link_url_prefix = link_url_prefix
+    self._img_url_prefix = img_url_prefix
     self._all_references = all_references
     self._console = console
-    self._label2token: Dict[str, Token] = {}
+    self._seen_labels: Set[str] = set()
 
   def _ShouldReplaceURL(self, url: str) -> bool:
     url_pr: ParseResult = urlparse(url)
     if url_pr.scheme != '':
       return False
     if url_pr.path == '':
       return False
     return True
 
-  def _ReplaceURL(self, url: str) -> str:
+  def _ReplaceURL(self, url: str, *, is_img: bool) -> str:
     """Replace the URL with a raw.githubusercontent.com URL if it is a relative
       path to a file in the repository."""
     if self._ShouldReplaceURL(url):
+      url_prefix = (self._img_url_prefix if is_img else self._link_url_prefix)
       # new_url = f'{self._url_prefix}{url_pr.path.lstrip("/")}'
-      new_url = urljoin(self._url_prefix, url)
+      new_url = urljoin(url_prefix, url)
       self._console.print(f'{url} -> {new_url}')
       return new_url
     return url
 
+  def _UpdateBS4Image(self, img: BeautifulSoup) -> bool:
+    if 'src' not in img.attrs:
+      return False
+    src0 = img.attrs['src']
+    if not isinstance(src0, str):
+      raise TypeError(f"Expected 'src' to be a string, but got {type(src0)}")
+    new_src = self._ReplaceURL(src0, is_img=True)
+    if new_src == src0:
+      return False
+    img.attrs['src'] = new_src
+    return True
+
   def _UpdateText(self, token: SpanToken):
     """Update the text contents of a span token and its children.
       `InlineCode` tokens are left unchanged."""
 
     if isinstance(token, Image):
       if token.label is not None:
-        self._label2token[token.label] = token
+        self._seen_labels.add(token.label)
       else:
-        token.src = self._ReplaceURL(token.src)
+        token.src = self._ReplaceURL(token.src, is_img=True)
     elif isinstance(token, Link):
       if token.label is not None:
-        self._label2token[token.label] = token
+        self._seen_labels.add(token.label)
       else:
-        token.target = self._ReplaceURL(token.target)
-    elif isinstance(token, HtmlSpan):
-      if token.content.startswith('<img '):
-        # parse the img html
-        img = BeautifulSoup(token.content, 'html.parser')
-        src0 = img['src']
-        if not isinstance(src0, str):
-          raise TypeError(
-              f"Expected 'src' to be a string, but got {type(src0)}")
-        new_src = self._ReplaceURL(src0)
-        if new_src != src0:
-          img['src'] = new_src
-          token.content = str(img)
+        token.target = self._ReplaceURL(token.target, is_img=False)
     elif isinstance(token, (LinkReferenceDefinition)):
-      if self._all_references or token.label in self._label2token:
-        token.dest = self._ReplaceURL(token.dest)
+      if self._all_references or token.label in self._seen_labels:
+        token.dest = self._ReplaceURL(token.dest, is_img=False)
+    elif isinstance(token, (RawText, HtmlSpan)):
+      soup = BeautifulSoup(token.content, 'html.parser')
+      updated = False
+      for img in soup.find_all('img'):
+        updated |= self._UpdateBS4Image(img)
+      if updated:
+        token.content = str(soup)
     else:
       pass
 
     if not isinstance(token, InlineCode) and hasattr(token, 'children'):
       children: List[Token] = token.children  # type: ignore
       for child in children:
         if not isinstance(child, SpanToken):
@@ -192,33 +202,46 @@
                    help='Output markdown file, use "-" for stdout.')
     p.add_argument(
         '--url-prefix',
         type=str,
         required=True,
         help='URL prefix to replace the local URLs with.'
         ' Should probably end in a slash.'
+        ' Example: "https://github.com/realazthat/mdremotifier/blob/master/".')
+    p.add_argument(
+        '--img-url-prefix',
+        type=str,
+        required=False,
+        default=None,
+        help='URL prefix to replace the local URLs with, specifically for images.'
+        ' Should probably end in a slash.'
         ' Example: "https://raw.githubusercontent.com/realazthat/mdremotifier/master/".'
-    )
+        ' Defaults to the value of --url-prefix.')
     p.add_argument(
         '--all-references',
         action='store',
         default=False,
         help=
         'Should all references be updated be externalized, or only those that are used by links and images?'
     )
     p.add_argument('--version',
                    action='version',
                    version=_build_version,
                    help='Show the version and exit.')
 
     args = p.parse_args()
+    url_prefix: str = args.url_prefix
+    img_url_prefix: str = url_prefix
+    if args.img_url_prefix is not None:
+      img_url_prefix = args.img_url_prefix
 
     with MarkdownRenderer() as renderer:
       doc = mistletoe.Document(_GetInput(args))
-      updater = _Updater(url_prefix=args.url_prefix,
+      updater = _Updater(link_url_prefix=url_prefix,
+                         img_url_prefix=img_url_prefix,
                          all_references=args.all_references,
                          console=console)
       updater.Update(doc)
       # Two passes, in case the linked reference came first.
       updater.Update(doc)
       _DumpOutput(args, renderer.render(doc))
```

### Comparing `mdremotifier-0.2.0/mdremotifier.egg-info/PKG-INFO` & `mdremotifier-0.3.0/mdremotifier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdremotifier
-Version: 0.2.0
+Version: 0.3.0
 Summary: Remotify local links in README.md.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -62,54 +62,78 @@
 Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == "prod"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
 Requires-Dist: types-html5lib==1.1.11.20240228; extra == "prod"
 Requires-Dist: typing-extensions==4.11.0; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.3.0; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
+Requires-Dist: backports-tarfile==1.1.1; extra == "dev"
 Requires-Dist: beautifulsoup4==4.12.3; extra == "dev"
 Requires-Dist: bs4==0.0.2; extra == "dev"
+Requires-Dist: certifi==2024.2.2; extra == "dev"
+Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: changeguard==0.3.1; extra == "dev"
+Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
+Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: defusedxml==0.7.1; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
+Requires-Dist: docutils==0.20.1; extra == "dev"
 Requires-Dist: filelock==3.13.4; extra == "dev"
 Requires-Dist: identify==2.5.36; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: idna==3.7; extra == "dev"
 Requires-Dist: importlib-metadata==7.1.0; extra == "dev"
+Requires-Dist: importlib-resources==6.4.0; extra == "dev"
+Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: jaraco-classes==3.4.0; extra == "dev"
+Requires-Dist: jaraco-context==5.3.0; extra == "dev"
+Requires-Dist: jaraco-functools==4.0.1; extra == "dev"
+Requires-Dist: jeepney==0.8.0; extra == "dev"
 Requires-Dist: jinja2==3.1.3; extra == "dev"
+Requires-Dist: keyring==25.2.0; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
 Requires-Dist: mistletoe==1.3.0; extra == "dev"
+Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
+Requires-Dist: nh3==0.2.17; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
 Requires-Dist: pexpect==4.9.0; extra == "dev"
+Requires-Dist: pkginfo==1.10.0; extra == "dev"
 Requires-Dist: platformdirs==4.2.1; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: ptyprocess==0.7.0; extra == "dev"
+Requires-Dist: pycparser==2.22; extra == "dev"
 Requires-Dist: pyflakes==3.2.0; extra == "dev"
 Requires-Dist: pygments==2.17.2; extra == "dev"
 Requires-Dist: pyright==1.1.352; extra == "dev"
 Requires-Dist: pyyaml==6.0.1; extra == "dev"
+Requires-Dist: readme-renderer==43.0; extra == "dev"
+Requires-Dist: requests==2.31.0; extra == "dev"
+Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
+Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
-Requires-Dist: snipinator==1.3.1; extra == "dev"
+Requires-Dist: secretstorage==3.3.3; extra == "dev"
+Requires-Dist: snipinator==1.4.0; extra == "dev"
 Requires-Dist: soupsieve==2.5; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
 Requires-Dist: types-html5lib==1.1.11.20240228; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
+Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.26.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
 Requires-Dist: yq==3.2.3; extra == "dev"
 Requires-Dist: zipp==3.18.1; extra == "dev"
 
 <!--
@@ -124,28 +148,26 @@
 
 
 
 
 
 -->
 
-# <div align="center">![mdremotifier][22]</div>
+# <div align="center">![mdremotifier][1]</div>
 
 <div align="center">
 
-<h1>warning _THIS PROJECT IS ALPHA^ALPHA, NOT READY FOR USE</h1>
-
 </div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][2] ![**Platform:** Linux][3]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="#-features">🎇Features</a>
     &nbsp;&bull;&nbsp;
@@ -159,52 +181,52 @@
     &nbsp;&bull;&nbsp;
     <a href="#-requirements">✅Requirements</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][4] [![GitHub License][5]][6] [![PyPI - Version][7]][8]
+[![Python Version][9]][8]
 
-**CLI to replace `./image.png` to <raw.githubusercontent.com> remote URL in
+**CLI to replace `./image.png` to `raw.githubusercontent.com` remote URL in
 README.md**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][10]**  | [![Build and Test][11]][12] | [![since tagged][13]][14] |                           | ![last commit][15] |
+| **[Develop][16]** | [![Build and Test][17]][12] | [![since tagged][18]][19] | [![since tagged][20]][21] | ![last commit][22] |
 
 </div>
 
-<img src="./.github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/mdremotifier/0.3.0/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What mdremotifier does:
 
-Turn this ([./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md)):
+Turn this ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
 ```
 <!---->
 
 Into this
-([./mdremotifier/examples/EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md)):
+([./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.remotified.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md).
 
@@ -222,20 +244,20 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdremotifier/)
 pip install mdremotifier
 
 # Install from git (https://github.com/realazthat/mdremotifier)
-pip install git+https://github.com/realazthat/mdremotifier.git@v0.2.0
+pip install git+https://github.com/realazthat/mdremotifier.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
-Example README: ([./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md)):
+Example README: ([./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md)):
 
 <!---->
 ```md
 # Example markdown file
 
 A link to a local file [LICENSE.md](./LICENSE.md).
 
@@ -253,29 +275,29 @@
 
 ```
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m mdremotifier.cli --help`" />
-<!---->
+<img alt="Output of `python -m mdremotifier.cli --help`" src="https://raw.githubusercontent.com/realazthat/mdremotifier/0.3.0/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - mdremotifier's own `README`:
-  - Original: [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md).
-  - Remotified: [./.github/README.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/README.remotified.md).
-  - Generation script: [./scripts/generate-readme.sh](https://raw.githubusercontent.com/realazthat/mdremotifier/master/scripts/generate-readme.sh).
+  - Original: [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md).
+  - Remotified: [./.github/README.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/README.remotified.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/scripts/generate-readme.sh).
 - Example:
-  - Original: [./mdremotifier/examples/EXAMPLE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.md).
+  - Original: [./mdremotifier/examples/EXAMPLE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.md).
   - Remotified:
-    [./mdremotifier/examples/EXAMPLE.remotified.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/EXAMPLE.remotified.md).
+    [./mdremotifier/examples/EXAMPLE.remotified.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/EXAMPLE.remotified.md).
   - Generation script:
-    [./mdremotifier/examples/example.sh](https://raw.githubusercontent.com/realazthat/mdremotifier/master/mdremotifier/examples/example.sh).
+    [./mdremotifier/examples/example.sh](https://github.com/realazthat/mdremotifier/blob/v0.3.0/mdremotifier/examples/example.sh).
 
 <!-- TODO: Rebuild this for mdremotifier
 - Projects using mdremotifier:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
     See
@@ -298,25 +320,25 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/workflows/build-and-test.yml)).
 
 ## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in mdremotifier are:
 
 - Markdown AST: [mistletoe](https://github.com/miyuchina/mistletoe).
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
@@ -324,62 +346,82 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                           | Stars | Last Update  | Language | Platform | Similarity X Obviousness |
 | ------------------------------------------------- | ----- | ------------ | -------- | -------- | ------------------------ |
-| [bdashore3/remark-github-images][60]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
-| [laobie/WriteMarkdownLazily][54]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [crh19970307/mdul][55]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][56] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                     |
-| [jen6/imgo][57]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                     |
-| [chocoluffy/lazy-markdown][59]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                     |
-| [loheagn/gopic][61]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                     |
-| [Undertone0809/imarkdown][53]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                      |
-| [ravgeetdhillon/markdown-imgur-upload][58]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                      |
+| [bdashore3/remark-github-images][23]              | 0     | `2022/12/29` | JS       | CLI      | ⭐⭐⭐⭐⭐                    |
+| [laobie/WriteMarkdownLazily][24]                  | 36    | `2024/01/06` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [crh19970307/mdul][25]                            | 1     | `2020/02/01` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [SkyLee424/Go-MarkDown-Image-Transfer-Helper][26] | 0     | `2024/03/25` | Go       | CLI      | ⭐⭐⭐⭐                     |
+| [jen6/imgo][27]                                   | 0     | `2020/03/18` | Pyhon    | CLI      | ⭐⭐⭐⭐                     |
+| [chocoluffy/lazy-markdown][28]                    | 0     | `2016/11/20` | Python   | CLI      | ⭐⭐⭐⭐                     |
+| [loheagn/gopic][29]                               | 0     | `2021/11/24` | Go       | CLI      | ⭐⭐⭐⭐                     |
+| [Undertone0809/imarkdown][30]                     | 57    | `2024/01/06` | Python   | Python   | ⭐⭐⭐                      |
+| [ravgeetdhillon/markdown-imgur-upload][31]        | 1     | `2022/03/26` | Python   | CLI      | ⭐⭐⭐                      |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](https://raw.githubusercontent.com/realazthat/mdremotifier/master/.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/mdremotifier/blob/v0.3.0/.python-version) (which is currently
     `3.8.0 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) generation, which uses `tomlq` (from the
+    [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md) generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    [./pyproject.toml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml).
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash`, `rsync` (for
-    tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act, animation).
+    [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/pyproject.toml).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](https://raw.githubusercontent.com/realazthat/mdremotifier/master/README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/mdremotifier/blob/v0.3.0/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](https://raw.githubusercontent.com/realazthat/mdremotifier/master/pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/mdremotifier/blob/v0.3.0/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.mdremotifier-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -391,74 +433,38 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
-[2]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
-[3]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
-[4]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/mdremotifier/
-[6]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/master?style=plastic
-[7]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
-[8]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
-[9]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...master
-[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
-[12]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[13]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[14]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.2.0/develop?style=plastic
-[16]: https://github.com/realazthat/mdremotifier/compare/v0.2.0...develop
-[17]: https://github.com/realazthat/mdremotifier/tree/master
-[18]: https://github.com/realazthat/mdremotifier/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
-[19]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
-[20]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/LICENSE.md
-[22]: https://raw.githubusercontent.com/realazthat/mdremotifier/master/.github/logo-exported.svg
-[23]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]: https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]: https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]: https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
-[54]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
-[55]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
-[56]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
-[57]: https://github.com/jen6/imgo "Upload to Google Drive"
-[58]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
-[59]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
-[60]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
-[61]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[1]: https://github.com/realazthat/mdremotifier/blob/v0.3.0/.github/logo-exported.svg
+[2]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[3]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[4]: https://img.shields.io/github/languages/top/realazthat/mdremotifier.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+[5]: https://img.shields.io/github/license/realazthat/mdremotifier?style=plastic&color=0A1E1E
+[6]: https://github.com/realazthat/mdremotifier/blob/v0.3.0/LICENSE.md
+[7]: https://img.shields.io/pypi/v/mdremotifier?style=plastic&color=0A1E1E
+[8]: https://pypi.org/project/mdremotifier/
+[9]: https://img.shields.io/pypi/pyversions/mdremotifier?style=plastic&color=0A1E1E
+[10]: https://github.com/realazthat/mdremotifier/tree/master
+[11]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=master&style=plastic
+[12]: https://github.com/realazthat/mdremotifier/actions/workflows/build-and-test.yml
+[13]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/master?style=plastic
+[14]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...master
+[15]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/master?style=plastic
+[16]: https://github.com/realazthat/mdremotifier/tree/develop
+[17]: https://img.shields.io/github/actions/workflow/status/realazthat/mdremotifier/build-and-test.yml?branch=develop&style=plastic
+[18]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[19]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[20]: https://img.shields.io/github/commits-since/realazthat/mdremotifier/v0.3.0/develop?style=plastic
+[21]: https://github.com/realazthat/mdremotifier/compare/v0.3.0...develop
+[22]: https://img.shields.io/github/last-commit/realazthat/mdremotifier/develop?style=plastic
+[23]: https://github.com/bdashore3/remark-github-images "Documentation is non-existent, but code looks very similar to mdremotifier"
+[24]: https://github.com/laobie/WriteMarkdownLazily "Uploads to cloud."
+[25]: https://github.com/crh19970307/mdul "Uploads to sm.ms"
+[26]: https://github.com/SkyLee424/Go-MarkDown-Image-Transfer-Helper "Upload to Qiniu Cloud"
+[27]: https://github.com/jen6/imgo "Upload to Google Drive"
+[28]: https://github.com/chocoluffy/lazy-markdown "Uploads to LeanCloud, readme is a bit unclear"
+[29]: https://github.com/loheagn/gopic "Upload to cloud, not clear which cloud"
+[30]: https://github.com/Undertone0809/imarkdown "Doesn't yet have a CLI."
+[31]: https://github.com/ravgeetdhillon/markdown-imgur-upload "Upload to imgur, a bit annoying because it requires you to put the images into a particular directory"
```

### Comparing `mdremotifier-0.2.0/mdremotifier.egg-info/requires.txt` & `mdremotifier-0.3.0/mdremotifier.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,54 +10,78 @@
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [dev]
 argcomplete==3.3.0
 autoflake==2.3.1
+backports-tarfile==1.1.1
 beautifulsoup4==4.12.3
 bs4==0.0.2
+certifi==2024.2.2
+cffi==1.16.0
 cfgv==3.4.0
 changeguard==0.3.1
+charset-normalizer==3.3.2
 colorama==0.4.6
+cryptography==42.0.5
 defusedxml==0.7.1
 distlib==0.3.8
+docutils==0.20.1
 filelock==3.13.4
 identify==2.5.36
-isort==5.13.2
+idna==3.7
 importlib-metadata==7.1.0
+importlib-resources==6.4.0
+isort==5.13.2
+jaraco-classes==3.4.0
+jaraco-context==5.3.0
+jaraco-functools==4.0.1
+jeepney==0.8.0
 jinja2==3.1.3
+keyring==25.2.0
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
 mistletoe==1.3.0
+more-itertools==10.2.0
 mypy==1.8.0
 mypy-extensions==1.0.0
+nh3==0.2.17
 nodeenv==1.8.0
 pathspec==0.12.1
 pexpect==4.9.0
+pkginfo==1.10.0
 platformdirs==4.2.1
 pre-commit==3.5.0
 ptyprocess==0.7.0
+pycparser==2.22
 pyflakes==3.2.0
 pygments==2.17.2
 pyright==1.1.352
 pyyaml==6.0.1
+readme-renderer==43.0
+requests==2.31.0
+requests-toolbelt==1.0.0
+rfc3986==2.0.0
 rich==13.7.1
 rich-argparse==1.4.0
-snipinator==1.3.1
+secretstorage==3.3.3
+snipinator==1.4.0
 soupsieve==2.5
 toml-sort==0.23.1
 tomli==2.0.1
 tomlkit==0.12.4
+twine==5.0.0
 types-beautifulsoup4==4.12.0.20240229
 types-colorama==0.4.15.20240311
 types-html5lib==1.1.11.20240228
 types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
+urllib3==2.2.1
 virtualenv==20.26.0
 xmltodict==0.13.0
 yapf==0.40.2
 yq==3.2.3
 zipp==3.18.1
 
 [prod]
```

### Comparing `mdremotifier-0.2.0/pyproject.toml` & `mdremotifier-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdremotifier"
-version = "0.2.0"
+version = "0.3.0"
 description = "Remotify local links in README.md."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = ".github/README.remotified.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -64,54 +64,78 @@
 ]
 # Set of dev dependencies, all pinned, so that they are known to work. To add a
 # new dependency here, add the unpinned package name here, and then run
 # `EXTRA=dev bash scripts/pin-extra-reqs.sh`.
 dev = [
   "argcomplete==3.3.0",
   "autoflake==2.3.1",
+  "backports-tarfile==1.1.1",
   "beautifulsoup4==4.12.3",
   "bs4==0.0.2",
+  "certifi==2024.2.2",
+  "cffi==1.16.0",
   "cfgv==3.4.0",
   "changeguard==0.3.1",
+  "charset-normalizer==3.3.2",
   "colorama==0.4.6",
+  "cryptography==42.0.5",
   "defusedxml==0.7.1",
   "distlib==0.3.8",
+  "docutils==0.20.1",
   "filelock==3.13.4",
   "identify==2.5.36",
-  "isort==5.13.2",
+  "idna==3.7",
   "importlib-metadata==7.1.0",
+  "importlib-resources==6.4.0",
+  "isort==5.13.2",
+  "jaraco-classes==3.4.0",
+  "jaraco-context==5.3.0",
+  "jaraco-functools==4.0.1",
+  "jeepney==0.8.0",
   "jinja2==3.1.3",
+  "keyring==25.2.0",
   "markdown-it-py==3.0.0",
   "markupsafe==2.1.5",
   "mdurl==0.1.2",
   "mistletoe==1.3.0",
+  "more-itertools==10.2.0",
   "mypy==1.8.0",
   "mypy-extensions==1.0.0",
+  "nh3==0.2.17",
   "nodeenv==1.8.0",
   "pathspec==0.12.1",
   "pexpect==4.9.0",
+  "pkginfo==1.10.0",
   "platformdirs==4.2.1",
   "pre-commit==3.5.0",
   "ptyprocess==0.7.0",
+  "pycparser==2.22",
   "pyflakes==3.2.0",
   "pygments==2.17.2",
   "pyright==1.1.352",
   "pyyaml==6.0.1",
+  "readme-renderer==43.0",
+  "requests==2.31.0",
+  "requests-toolbelt==1.0.0",
+  "rfc3986==2.0.0",
   "rich==13.7.1",
   "rich-argparse==1.4.0",
-  "snipinator==1.3.1",
+  "secretstorage==3.3.3",
+  "snipinator==1.4.0",
   "soupsieve==2.5",
   "toml-sort==0.23.1",
   "tomli==2.0.1",
   "tomlkit==0.12.4",
+  "twine==5.0.0",
   "types-beautifulsoup4==4.12.0.20240229",
   "types-colorama==0.4.15.20240311",
   "types-html5lib==1.1.11.20240228",
   "types-pyyaml==6.0.12.20240311",
   "typing-extensions==4.10.0",
+  "urllib3==2.2.1",
   "virtualenv==20.26.0",
   "xmltodict==0.13.0",
   "yapf==0.40.2",
   "yq==3.2.3",
   "zipp==3.18.1"
 ]
 
@@ -120,14 +144,14 @@
 
 [project.urls]
 Homepage = "https://github.com/realazthat/mdremotifier"
 Documentation = "https://github.com/realazthat/mdremotifier"
 Repository = "https://github.com/realazthat/mdremotifier"
 
 [tool.mdremotifier-project-metadata]
-last_unstable_release = "0.2.0"
-last_stable_release = "0.2.0"
+last_unstable_release = "0.3.0"
+last_stable_release = "0.3.0"
 
 [tool.setuptools]
 packages = ["mdremotifier"]
 
 [tool.tomlsort]
```

