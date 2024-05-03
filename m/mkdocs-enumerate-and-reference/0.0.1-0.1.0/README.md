# Comparing `tmp/mkdocs_enumerate_and_reference-0.0.1.tar.gz` & `tmp/mkdocs_enumerate_and_reference-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_enumerate_and_reference-0.0.1.tar", max compression
+gzip compressed data, was "mkdocs_enumerate_and_reference-0.1.0.tar", max compression
```

## Comparing `mkdocs_enumerate_and_reference-0.0.1.tar` & `mkdocs_enumerate_and_reference-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0       83 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/__init__.py
--rw-r--r--   0        0        0     2011 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/enumerate.py
--rw-r--r--   0        0        0     3968 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/plugin.py
--rw-r--r--   0        0        0     1239 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/reference.py
--rw-r--r--   0        0        0      696 2024-01-03 18:38:37.544862 mkdocs_enumerate_and_reference-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 mkdocs_enumerate_and_reference-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-03 18:02:55.372146 mkdocs_enumerate_and_reference-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1902 2024-05-03 18:02:55.372146 mkdocs_enumerate_and_reference-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/__init__.py
+-rw-r--r--   0        0        0     2153 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/enumerate.py
+-rw-r--r--   0        0        0     4075 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/plugin.py
+-rw-r--r--   0        0        0     1239 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/reference.py
+-rw-r--r--   0        0        0      908 2024-05-03 18:02:55.376146 mkdocs_enumerate_and_reference-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 mkdocs_enumerate_and_reference-0.1.0/PKG-INFO
```

### Comparing `mkdocs_enumerate_and_reference-0.0.1/LICENSE.txt` & `mkdocs_enumerate_and_reference-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/enumerate.py` & `mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/enumerate.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     anc_numbers.append(item.number)
     cnumber = ".".join(anc_numbers)
     item.cnumber = cnumber
     return cnumber
 
 
 def enumerate_navigation(nav, cumulative: bool=True):
-    for item in nav.items:
+    for i, item in enumerate(nav.items):
+        item.number = str(i+1)
+        if item.title is not None:
+            item.title = ". ".join([item.number, item.title])
         enumerate_children(item, cumulative)
 
 
 def enumerate_children(item, cumulative: bool):
     if item.children is not None: 
         for i, child in enumerate(item.children):
             number = str(i+1)
```

### Comparing `mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/plugin.py` & `mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         for page in nav.pages:
             source = read_source(page)
             tag_ids = re.findall(r'@tag\((.+?)\)', source)
             self.config.tags_paths.update({k: page.url for k in tag_ids})
             # next line is to prevent reading source twice
             # config.sources.update({page.file.src_path: source})
     
-    def on_page_markdown(self, markdown, page,  **kwargs):
+    def on_page_markdown(self, markdown, page, config  **kwargs):
         if self.config.number_headings.enabled:
             activated, lowest_level = self.get_number_headings_params(page.meta)
             if activated:
                 markdown = add_section_numbers(markdown, lowest_level=lowest_level)
 
         cnumber = page.cnumber if hasattr(page, "cnumber") else None
         markdown = refactor_admonitions(markdown, cnumber)
@@ -91,7 +91,11 @@
     """
     if tag_id in tags_paths:
         rel_path = relpath(tags_paths[tag_id], url)
         r = f"{rel_path}/#{tag_id}"
         return f"{rel_path}/#{tag_id}"
     else:
         return tag_id
+
+if __name__ == "__main__":
+    from mkdocs.commands.serve import serve
+    serve("docs/mkdocs.yml")
```

### Comparing `mkdocs_enumerate_and_reference-0.0.1/mkdocs_enumerate_and_reference/reference.py` & `mkdocs_enumerate_and_reference-0.1.0/mkdocs_enumerate_and_reference/reference.py`

 * *Files identical despite different names*

