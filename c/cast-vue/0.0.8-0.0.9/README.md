# Comparing `tmp/cast_vue-0.0.8.tar.gz` & `tmp/cast_vue-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cast_vue-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cast_vue-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cast_vue-0.0.8.tar` & `cast_vue-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0       90 2023-05-01 09:20:55.972830 cast_vue-0.0.8/.flake8
--rw-r--r--   0        0        0     2776 2023-05-30 04:53:45.246928 cast_vue-0.0.8/.gitignore
--rw-r--r--   0        0        0     1280 2023-05-01 09:18:51.481763 cast_vue-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2023-05-31 13:30:36.999455 cast_vue-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0     1505 2023-04-25 12:38:56.294777 cast_vue-0.0.8/LICENSE
--rw-r--r--   0        0        0     1504 2023-06-03 08:07:22.211561 cast_vue-0.0.8/README.md
--rw-r--r--   0        0        0       58 2023-08-24 17:24:18.237748 cast_vue-0.0.8/cast_vue/__init__.py
--rw-r--r--   0        0        0       90 2023-05-26 06:40:41.842414 cast_vue-0.0.8/cast_vue/apps.py
--rw-r--r--   0        0        0   102504 2023-08-24 17:23:07.951259 cast_vue-0.0.8/cast_vue/static/cast_vue/main-a0a35c93.js
--rw-r--r--   0        0        0     3861 2023-08-24 17:23:07.951183 cast_vue-0.0.8/cast_vue/static/cast_vue/main-da561700.css
--rw-r--r--   0        0        0      267 2023-08-24 17:23:28.223832 cast_vue-0.0.8/cast_vue/static/cast_vue/manifest.json
--rw-r--r--   0        0        0     4820 2023-05-21 12:56:52.164564 cast_vue-0.0.8/cast_vue/static/src/css/cast_vue/pygments.css
--rw-r--r--   0        0        0      243 2023-05-31 05:05:23.594201 cast_vue-0.0.8/cast_vue/static/src/css/cast_vue/styles.css
--rw-r--r--   0        0        0      952 2023-06-01 08:12:11.618518 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/App.vue
--rw-r--r--   0        0        0     2438 2023-06-03 10:38:33.762232 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/CommentForm.vue
--rw-r--r--   0        0        0     2498 2023-06-03 13:46:34.583934 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/CommentItem.vue
--rw-r--r--   0        0        0     3916 2023-06-05 09:32:00.446845 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/CommentList.vue
--rw-r--r--   0        0        0     3837 2023-08-24 15:28:59.917024 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/FilterForm.vue
--rw-r--r--   0        0        0     4893 2023-08-24 14:42:16.759342 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/LoadPostList.vue
--rw-r--r--   0        0        0     1179 2023-05-27 04:42:17.583182 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PaginationButtons.vue
--rw-r--r--   0        0        0      858 2023-06-04 17:58:26.383558 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PodlovePlayer.vue
--rw-r--r--   0        0        0     2358 2023-06-04 17:22:18.487455 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PostDetail.vue
--rw-r--r--   0        0        0     6364 2023-06-04 17:43:26.510191 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PostItem.vue
--rw-r--r--   0        0        0      728 2023-05-21 06:25:57.294899 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PostList.vue
--rw-r--r--   0        0        0     2222 2023-08-24 15:30:06.340438 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/types.ts
--rw-r--r--   0        0        0     1339 2023-06-03 13:34:23.511493 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/config.ts
--rw-r--r--   0        0        0      276 2023-04-29 13:53:07.766990 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/env.d.ts
--rw-r--r--   0        0        0      688 2023-05-21 19:57:32.000318 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/helpers/url.ts
--rw-r--r--   0        0        0      991 2023-06-01 08:14:04.995128 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/main.ts
--rw-r--r--   0        0        0     1353 2023-06-03 13:34:23.511613 cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/stores/dataStore.ts
--rw-r--r--   0        0        0     1543 2023-06-01 11:40:39.091796 cast_vue-0.0.8/cast_vue/static/src/tests/CommentItem.test.ts
--rw-r--r--   0        0        0     1217 2023-05-31 08:22:38.413871 cast_vue-0.0.8/cast_vue/static/src/tests/CommentList.test.ts
--rw-r--r--   0        0        0      120 2023-05-30 09:03:36.329437 cast_vue-0.0.8/cast_vue/static/src/tests/calculator.test.ts
--rw-r--r--   0        0        0      199 2023-04-28 20:44:53.445873 cast_vue-0.0.8/cast_vue/templates/cast/vue/400.html
--rw-r--r--   0        0        0      181 2023-04-28 20:44:53.446033 cast_vue-0.0.8/cast_vue/templates/cast/vue/403.html
--rw-r--r--   0        0        0      200 2023-04-28 20:44:53.446164 cast_vue-0.0.8/cast_vue/templates/cast/vue/403_csrf.html
--rw-r--r--   0        0        0      198 2023-04-28 20:44:53.446291 cast_vue-0.0.8/cast_vue/templates/cast/vue/404.html
--rw-r--r--   0        0        0      319 2023-04-28 20:44:53.446418 cast_vue-0.0.8/cast_vue/templates/cast/vue/500.html
--rw-r--r--   0        0        0      770 2023-04-28 20:44:53.446553 cast_vue-0.0.8/cast_vue/templates/cast/vue/_filter_form.html
--rw-r--r--   0        0        0      184 2023-04-28 20:44:53.446700 cast_vue-0.0.8/cast_vue/templates/cast/vue/_list_of_posts_and_paging_controls.html
--rw-r--r--   0        0        0     1653 2023-06-03 15:08:18.582073 cast_vue-0.0.8/cast_vue/templates/cast/vue/base.html
--rw-r--r--   0        0        0      196 2023-05-15 16:15:28.834058 cast_vue-0.0.8/cast_vue/templates/cast/vue/blog_list_of_posts.html
--rw-r--r--   0        0        0     1221 2023-04-29 06:25:35.455745 cast_vue-0.0.8/cast_vue/templates/cast/vue/blog_list_of_posts_old.html
--rw-r--r--   0        0        0      213 2023-04-28 20:44:53.447104 cast_vue-0.0.8/cast_vue/templates/cast/vue/episode.html
--rw-r--r--   0        0        0      807 2023-05-18 06:51:31.049924 cast_vue-0.0.8/cast_vue/templates/cast/vue/gallery.html
--rw-r--r--   0        0        0     2367 2023-04-28 20:44:53.447241 cast_vue-0.0.8/cast_vue/templates/cast/vue/pagination.html
--rw-r--r--   0        0        0      374 2023-06-03 13:34:23.511684 cast_vue-0.0.8/cast_vue/templates/cast/vue/post.html
--rw-r--r--   0        0        0      789 2023-06-01 09:37:52.057981 cast_vue-0.0.8/cast_vue/templates/cast/vue/post_body.html
--rw-r--r--   0        0        0      437 2023-05-26 06:05:17.654395 cast_vue-0.0.8/jest.config.js
--rwxr-xr-x   0        0        0      664 2023-04-27 12:47:56.103508 cast_vue-0.0.8/manage.py
--rw-r--r--   0        0        0    97175 2023-08-24 17:20:47.767263 cast_vue-0.0.8/package-lock.json
--rw-r--r--   0        0        0      489 2023-08-24 17:20:47.748185 cast_vue-0.0.8/package.json
--rw-r--r--   0        0        0      629 2023-05-31 13:39:14.362674 cast_vue-0.0.8/print_source.py
--rw-r--r--   0        0        0     2295 2023-04-27 11:19:43.197149 cast_vue-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      595 2023-05-31 07:40:49.752443 cast_vue-0.0.8/tsconfig.json
--rw-r--r--   0        0        0     1053 2023-05-31 07:39:24.021058 cast_vue-0.0.8/vite.config.ts
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 cast_vue-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-05-01 09:20:55.972830 cast_vue-0.0.9/.flake8
+-rw-r--r--   0        0        0     2776 2023-05-30 04:53:45.246928 cast_vue-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1280 2023-05-01 09:18:51.481763 cast_vue-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2023-05-31 13:30:36.999455 cast_vue-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0     1505 2023-04-25 12:38:56.294777 cast_vue-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1504 2023-06-03 08:07:22.211561 cast_vue-0.0.9/README.md
+-rw-r--r--   0        0        0       58 2023-09-03 08:01:36.875210 cast_vue-0.0.9/cast_vue/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-26 06:40:41.842414 cast_vue-0.0.9/cast_vue/apps.py
+-rw-r--r--   0        0        0   102504 2023-08-24 17:23:07.951259 cast_vue-0.0.9/cast_vue/static/cast_vue/main-a0a35c93.js
+-rw-r--r--   0        0        0     3861 2023-08-24 17:23:07.951183 cast_vue-0.0.9/cast_vue/static/cast_vue/main-da561700.css
+-rw-r--r--   0        0        0      267 2023-08-24 17:23:28.223832 cast_vue-0.0.9/cast_vue/static/cast_vue/manifest.json
+-rw-r--r--   0        0        0     4820 2023-05-21 12:56:52.164564 cast_vue-0.0.9/cast_vue/static/src/css/cast_vue/pygments.css
+-rw-r--r--   0        0        0      243 2023-05-31 05:05:23.594201 cast_vue-0.0.9/cast_vue/static/src/css/cast_vue/styles.css
+-rw-r--r--   0        0        0      952 2023-06-01 08:12:11.618518 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/App.vue
+-rw-r--r--   0        0        0     2438 2023-06-03 10:38:33.762232 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/CommentForm.vue
+-rw-r--r--   0        0        0     2498 2023-06-03 13:46:34.583934 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/CommentItem.vue
+-rw-r--r--   0        0        0     3916 2023-06-05 09:32:00.446845 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/CommentList.vue
+-rw-r--r--   0        0        0     3837 2023-08-24 15:28:59.917024 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/FilterForm.vue
+-rw-r--r--   0        0        0     5002 2023-09-03 08:00:04.663976 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/LoadPostList.vue
+-rw-r--r--   0        0        0     1179 2023-05-27 04:42:17.583182 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PaginationButtons.vue
+-rw-r--r--   0        0        0      858 2023-06-04 17:58:26.383558 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PodlovePlayer.vue
+-rw-r--r--   0        0        0     2358 2023-06-04 17:22:18.487455 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PostDetail.vue
+-rw-r--r--   0        0        0     6364 2023-06-04 17:43:26.510191 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PostItem.vue
+-rw-r--r--   0        0        0      728 2023-05-21 06:25:57.294899 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PostList.vue
+-rw-r--r--   0        0        0     1697 2023-09-03 08:03:46.770346 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/SelectTheme.vue
+-rw-r--r--   0        0        0     2304 2023-09-03 08:01:14.991569 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/types.ts
+-rw-r--r--   0        0        0     1485 2023-09-03 07:59:54.616579 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/config.ts
+-rw-r--r--   0        0        0      276 2023-04-29 13:53:07.766990 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/env.d.ts
+-rw-r--r--   0        0        0      688 2023-05-21 19:57:32.000318 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/helpers/url.ts
+-rw-r--r--   0        0        0      991 2023-06-01 08:14:04.995128 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/main.ts
+-rw-r--r--   0        0        0     1353 2023-06-03 13:34:23.511613 cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/stores/dataStore.ts
+-rw-r--r--   0        0        0     1543 2023-06-01 11:40:39.091796 cast_vue-0.0.9/cast_vue/static/src/tests/CommentItem.test.ts
+-rw-r--r--   0        0        0     1217 2023-05-31 08:22:38.413871 cast_vue-0.0.9/cast_vue/static/src/tests/CommentList.test.ts
+-rw-r--r--   0        0        0      120 2023-05-30 09:03:36.329437 cast_vue-0.0.9/cast_vue/static/src/tests/calculator.test.ts
+-rw-r--r--   0        0        0      199 2023-04-28 20:44:53.445873 cast_vue-0.0.9/cast_vue/templates/cast/vue/400.html
+-rw-r--r--   0        0        0      181 2023-04-28 20:44:53.446033 cast_vue-0.0.9/cast_vue/templates/cast/vue/403.html
+-rw-r--r--   0        0        0      200 2023-04-28 20:44:53.446164 cast_vue-0.0.9/cast_vue/templates/cast/vue/403_csrf.html
+-rw-r--r--   0        0        0      198 2023-04-28 20:44:53.446291 cast_vue-0.0.9/cast_vue/templates/cast/vue/404.html
+-rw-r--r--   0        0        0      319 2023-04-28 20:44:53.446418 cast_vue-0.0.9/cast_vue/templates/cast/vue/500.html
+-rw-r--r--   0        0        0      770 2023-04-28 20:44:53.446553 cast_vue-0.0.9/cast_vue/templates/cast/vue/_filter_form.html
+-rw-r--r--   0        0        0      184 2023-04-28 20:44:53.446700 cast_vue-0.0.9/cast_vue/templates/cast/vue/_list_of_posts_and_paging_controls.html
+-rw-r--r--   0        0        0     1930 2023-09-03 07:33:46.845509 cast_vue-0.0.9/cast_vue/templates/cast/vue/base.html
+-rw-r--r--   0        0        0      196 2023-05-15 16:15:28.834058 cast_vue-0.0.9/cast_vue/templates/cast/vue/blog_list_of_posts.html
+-rw-r--r--   0        0        0     1221 2023-04-29 06:25:35.455745 cast_vue-0.0.9/cast_vue/templates/cast/vue/blog_list_of_posts_old.html
+-rw-r--r--   0        0        0      213 2023-04-28 20:44:53.447104 cast_vue-0.0.9/cast_vue/templates/cast/vue/episode.html
+-rw-r--r--   0        0        0      807 2023-05-18 06:51:31.049924 cast_vue-0.0.9/cast_vue/templates/cast/vue/gallery.html
+-rw-r--r--   0        0        0     2367 2023-04-28 20:44:53.447241 cast_vue-0.0.9/cast_vue/templates/cast/vue/pagination.html
+-rw-r--r--   0        0        0      374 2023-06-03 13:34:23.511684 cast_vue-0.0.9/cast_vue/templates/cast/vue/post.html
+-rw-r--r--   0        0        0      789 2023-06-01 09:37:52.057981 cast_vue-0.0.9/cast_vue/templates/cast/vue/post_body.html
+-rw-r--r--   0        0        0      437 2023-05-26 06:05:17.654395 cast_vue-0.0.9/jest.config.js
+-rwxr-xr-x   0        0        0      664 2023-04-27 12:47:56.103508 cast_vue-0.0.9/manage.py
+-rw-r--r--   0        0        0    97175 2023-08-24 17:20:47.767263 cast_vue-0.0.9/package-lock.json
+-rw-r--r--   0        0        0      489 2023-08-24 17:20:47.748185 cast_vue-0.0.9/package.json
+-rw-r--r--   0        0        0      629 2023-05-31 13:39:14.362674 cast_vue-0.0.9/print_source.py
+-rw-r--r--   0        0        0     2295 2023-04-27 11:19:43.197149 cast_vue-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-05-31 07:40:49.752443 cast_vue-0.0.9/tsconfig.json
+-rw-r--r--   0        0        0     1053 2023-05-31 07:39:24.021058 cast_vue-0.0.9/vite.config.ts
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 cast_vue-0.0.9/PKG-INFO
```

### Comparing `cast_vue-0.0.8/.gitignore` & `cast_vue-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/.pre-commit-config.yaml` & `cast_vue-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/LICENSE` & `cast_vue-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/README.md` & `cast_vue-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/cast_vue/main-a0a35c93.js` & `cast_vue-0.0.9/cast_vue/static/cast_vue/main-a0a35c93.js`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/cast_vue/main-da561700.css` & `cast_vue-0.0.9/cast_vue/static/cast_vue/main-da561700.css`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/css/cast_vue/pygments.css` & `cast_vue-0.0.9/cast_vue/static/src/css/cast_vue/pygments.css`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/App.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/App.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/CommentForm.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/CommentForm.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/CommentItem.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/CommentItem.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/CommentList.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/CommentList.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/FilterForm.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/FilterForm.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/LoadPostList.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/LoadPostList.vue`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <template>
     <div>
         <p v-if="isLoading">Loading data...</p>
         <div v-else>
+            <select-theme></select-theme>
             <filter-form
                 @submit-filter-form="handleSubmitFilterForm"
                 :form="form"
                 :facetCounts="facetCounts"
             ></filter-form>
             <br />
             <pagination-buttons :currentPage="currentPage" :totalPages="totalPages" @change-page="changePage">
@@ -19,24 +20,26 @@
 import config from '../config';
 import { FacetCounts, PostsFromApi } from './types';
 import { ref, onMounted, computed, Ref } from 'vue';
 import { LocationQueryRaw, useRoute, useRouter } from 'vue-router';
 import FilterForm from './FilterForm.vue';
 import PostList from './PostList.vue';
 import PaginationButtons from './PaginationButtons.vue';
+import SelectTheme from './SelectTheme.vue';
 import { useDataStore } from '../stores/dataStore';
 import { setUrlSearchParams, getUrlSearchParams } from '../helpers/url';
 import { Form } from './types';
 
 
 export default {
     components: {
         FilterForm,
         PostList,
-        PaginationButtons
+        PaginationButtons,
+        SelectTheme,
     },
     setup() {
         const route = useRoute();
         const router = useRouter();
         const isLoading = ref(true);
         const blog = ref({});
         const postsFromApi = ref({} as PostsFromApi);
```

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PaginationButtons.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PaginationButtons.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PodlovePlayer.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PodlovePlayer.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PostDetail.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PostDetail.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PostItem.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PostItem.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/PostList.vue` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/PostList.vue`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/components/types.ts` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/components/types.ts`

 * *Files 3% similar despite different names*

```diff
@@ -116,7 +116,14 @@
 }
 
 export interface FacetCounts {
   date_facets: [Facet];
   category_facets: [Facet];
   tag_facets: [Facet];
 }
+
+
+export interface Theme {
+  slug: string;
+  name: string;
+  selected: boolean;
+}
```

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/config.ts` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/config.ts`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
   paginationPageSize = "5",
   wagtailApiPagesUrl = "/",
   apiFacetCountsUrl = "/",
   postCommentUrl = "/",
   vueRouteName = "PostList",
   postSlug = "",
   pageType = "",
+  apiThemeListUrl = "/",
+  apiThemeUpdateUrl = "/",
 } = document.getElementById("vue-configuration")?.dataset ?? {};
 
 let parsedBlogId = null;
 
 if (blogId) {
   parsedBlogId = parseInt(blogId);
   if (isNaN(parsedBlogId)) {
@@ -41,13 +43,15 @@
   blogUrl,
   csrfToken,
   blogId: parsedBlogId,
   paginationPageSize: parsedPaginationPageSize,
   wagtailApiPagesUrl,
   apiFacetCountsUrl: parsedApiFacetCountsUrl,
   postCommentUrl: parsedPostCommentUrl,
+  apiThemeListUrl: new URL(apiThemeListUrl),
+  apiThemeUpdateUrl: new URL(apiThemeUpdateUrl),
   blogDetailUrl,
   postListUrl,
   vueRouteName,
   postSlug,
   pageType,
 };
```

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/helpers/url.ts` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/helpers/url.ts`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/main.ts` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/main.ts`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/js/cast_vue/stores/dataStore.ts` & `cast_vue-0.0.9/cast_vue/static/src/js/cast_vue/stores/dataStore.ts`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/tests/CommentItem.test.ts` & `cast_vue-0.0.9/cast_vue/static/src/tests/CommentItem.test.ts`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/static/src/tests/CommentList.test.ts` & `cast_vue-0.0.9/cast_vue/static/src/tests/CommentList.test.ts`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/templates/cast/vue/_filter_form.html` & `cast_vue-0.0.9/cast_vue/templates/cast/vue/_filter_form.html`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/templates/cast/vue/base.html` & `cast_vue-0.0.9/cast_vue/templates/cast/vue/base.html`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,17 @@
               data-pagination-page-size="{{ blog.pagination_page_size }}" {# Used for pagination #}
             {# Used for fetching posts #}
               data-wagtail-api-pages-url="{{ request.scheme }}://{{ request.get_host }}{{ blog.wagtail_api_pages_url }}"
             {# Used for fetching facet counts #}
               data-api-facet-counts-url="{{ request.scheme }}://{{ request.get_host }}{{ blog.facet_counts_api_url }}"
             {# Used for posting comments #}
               data-post-comment-url="{{ request.scheme }}://{{ request.get_host }}{{ blog.comment_post_url }}"
+            {# Used for theme selection #}
+              data-api-theme-list-url="{{ request.scheme }}://{{ request.get_host }}{{ blog.theme_list_api_url }}"
+              data-api-theme-update-url="{{ request.scheme }}://{{ request.get_host }}{{ blog.theme_update_api_url }}"
             {% endblock vuejs-data %}
     >
     </script>
     <script src={% static 'js/cast/web-player/embed.4.js' %}></script>
   </head>
   <body>
     {% block main %}
```

#### html2text {}

```diff
@@ -5,11 +5,15 @@
 data-blog-id="{{ blog.pk }}" {# Used for blog api detail url and posts endpoint
 child_of=blog.pk #} data-pagination-page-size="{{ blog.pagination_page_size }}"
 {# Used for pagination #} {# Used for fetching posts #} data-wagtail-api-pages-
 url="{{ request.scheme }}://{{ request.get_host }}{{ blog.wagtail_api_pages_url
 }}" {# Used for fetching facet counts #} data-api-facet-counts-url="{
 { request.scheme }}://{{ request.get_host }}{{ blog.facet_counts_api_url }}" {#
 Used for posting comments #} data-post-comment-url="{{ request.scheme }}://{
-{ request.get_host }}{{ blog.comment_post_url }}" {% endblock vuejs-data %} >
+{ request.get_host }}{{ blog.comment_post_url }}" {# Used for theme selection
+#} data-api-theme-list-url="{{ request.scheme }}://{{ request.get_host }}{
+{ blog.theme_list_api_url }}" data-api-theme-update-url="{{ request.scheme }}:/
+/{{ request.get_host }}{{ blog.theme_update_api_url }}" {% endblock vuejs-data
+%} >
 }>
 {% block main %}
 {% endblock main %}
```

### Comparing `cast_vue-0.0.8/cast_vue/templates/cast/vue/blog_list_of_posts_old.html` & `cast_vue-0.0.9/cast_vue/templates/cast/vue/blog_list_of_posts_old.html`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/templates/cast/vue/gallery.html` & `cast_vue-0.0.9/cast_vue/templates/cast/vue/gallery.html`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/templates/cast/vue/pagination.html` & `cast_vue-0.0.9/cast_vue/templates/cast/vue/pagination.html`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/cast_vue/templates/cast/vue/post_body.html` & `cast_vue-0.0.9/cast_vue/templates/cast/vue/post_body.html`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/manage.py` & `cast_vue-0.0.9/manage.py`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/package-lock.json` & `cast_vue-0.0.9/package-lock.json`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/print_source.py` & `cast_vue-0.0.9/print_source.py`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/pyproject.toml` & `cast_vue-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/tsconfig.json` & `cast_vue-0.0.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/vite.config.ts` & `cast_vue-0.0.9/vite.config.ts`

 * *Files identical despite different names*

### Comparing `cast_vue-0.0.8/PKG-INFO` & `cast_vue-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cast-vue
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vue theme for django-cast.
 Keywords: blog,podcast,video,audio
 Author-email: Jochen Wersdörfer <jochen-castvue@wersdoerfer.de>
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

