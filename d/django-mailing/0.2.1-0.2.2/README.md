# Comparing `tmp/django-mailing-0.2.1.tar.gz` & `tmp/django_mailing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mailing-0.2.1.tar", last modified: Fri Mar  1 14:45:21 2024, max compression
+gzip compressed data, was "django_mailing-0.2.2.tar", last modified: Fri May  3 13:23:43 2024, max compression
```

## Comparing `django-mailing-0.2.1.tar` & `django_mailing-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.733506 django-mailing-0.2.1/
--rwxr-xr-x   0 jparadis   (501) staff       (20)      178 2023-05-05 14:19:38.000000 django-mailing-0.2.1/AUTHORS.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)       41 2023-05-05 14:19:38.000000 django-mailing-0.2.1/CHANGES.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1113 2023-05-05 14:19:38.000000 django-mailing-0.2.1/LICENSE.txt
--rwxr-xr-x   0 jparadis   (501) staff       (20)      134 2023-05-05 14:19:38.000000 django-mailing-0.2.1/MANIFEST.in
--rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-03-01 14:45:21.732695 django-mailing-0.2.1/PKG-INFO
--rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django-mailing-0.2.1/README.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.731915 django-mailing-0.2.1/django_mailing.egg-info/
--rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-03-01 14:45:21.000000 django-mailing-0.2.1/django_mailing.egg-info/PKG-INFO
--rw-r--r--   0 jparadis   (501) staff       (20)      687 2024-03-01 14:45:21.000000 django-mailing-0.2.1/django_mailing.egg-info/SOURCES.txt
--rw-r--r--   0 jparadis   (501) staff       (20)        1 2024-03-01 14:45:21.000000 django-mailing-0.2.1/django_mailing.egg-info/dependency_links.txt
--rw-r--r--   0 jparadis   (501) staff       (20)       49 2024-03-01 14:45:21.000000 django-mailing-0.2.1/django_mailing.egg-info/requires.txt
--rw-r--r--   0 jparadis   (501) staff       (20)        8 2024-03-01 14:45:21.000000 django-mailing-0.2.1/django_mailing.egg-info/top_level.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.720930 django-mailing-0.2.1/docs/
--rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django-mailing-0.2.1/docs/usage.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.726400 django-mailing-0.2.1/mailing/
--rwxr-xr-x   0 jparadis   (501) staff       (20)      525 2024-03-01 14:22:59.000000 django-mailing-0.2.1/mailing/__init__.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     5030 2023-05-05 15:32:40.000000 django-mailing-0.2.1/mailing/mail.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)        0 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/models.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     2263 2023-05-05 15:32:40.000000 django-mailing-0.2.1/mailing/shortcuts.py
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1870 2024-02-29 16:08:00.000000 django-mailing-0.2.1/mailing/tasks.py
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.712046 django-mailing-0.2.1/mailing/templates/
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.727850 django-mailing-0.2.1/mailing/templates/mailing/
--rwxr-xr-x   0 jparadis   (501) staff       (20)     3245 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/templates/mailing/base.html
--rwxr-xr-x   0 jparadis   (501) staff       (20)      150 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/templates/mailing/base.txt
-drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-03-01 14:45:21.730962 django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/
--rw-r--r--   0 jparadis   (501) staff       (20)     2555 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/README.markdown
--rw-r--r--   0 jparadis   (501) staff       (20)      352 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/contributors.txt
--rw-r--r--   0 jparadis   (501) staff       (20)    12246 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/email.html
--rw-r--r--   0 jparadis   (501) staff       (20)     6542 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/email_lite.html
--rwxr-xr-x   0 jparadis   (501) staff       (20)       26 2023-05-05 14:19:38.000000 django-mailing-0.2.1/mailing/views.py
--rw-r--r--   0 jparadis   (501) staff       (20)       38 2024-03-01 14:45:21.733655 django-mailing-0.2.1/setup.cfg
--rwxr-xr-x   0 jparadis   (501) staff       (20)     1099 2023-05-05 14:19:38.000000 django-mailing-0.2.1/setup.py
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.735675 django_mailing-0.2.2/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      178 2023-05-05 14:19:38.000000 django_mailing-0.2.2/AUTHORS.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)       41 2023-05-05 14:19:38.000000 django_mailing-0.2.2/CHANGES.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1113 2023-05-05 14:19:38.000000 django_mailing-0.2.2/LICENSE.txt
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      134 2023-05-05 14:19:38.000000 django_mailing-0.2.2/MANIFEST.in
+-rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-03 13:23:43.735099 django_mailing-0.2.2/PKG-INFO
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.2/README.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.734588 django_mailing-0.2.2/django_mailing.egg-info/
+-rw-r--r--   0 jparadis   (501) staff       (20)     8957 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/PKG-INFO
+-rw-r--r--   0 jparadis   (501) staff       (20)      687 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/SOURCES.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)        1 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/dependency_links.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)       49 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/requires.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)        8 2024-05-03 13:23:43.000000 django_mailing-0.2.2/django_mailing.egg-info/top_level.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.727230 django_mailing-0.2.2/docs/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     8415 2023-05-05 14:19:38.000000 django_mailing-0.2.2/docs/usage.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.730758 django_mailing-0.2.2/mailing/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      525 2024-05-03 13:09:42.000000 django_mailing-0.2.2/mailing/__init__.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     5074 2024-05-03 13:12:14.000000 django_mailing-0.2.2/mailing/mail.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)        0 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/models.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     2307 2024-05-03 13:13:32.000000 django_mailing-0.2.2/mailing/shortcuts.py
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1938 2024-05-03 13:13:16.000000 django_mailing-0.2.2/mailing/tasks.py
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.721063 django_mailing-0.2.2/mailing/templates/
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.731653 django_mailing-0.2.2/mailing/templates/mailing/
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     3245 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/base.html
+-rwxr-xr-x   0 jparadis   (501) staff       (20)      150 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/base.txt
+drwxr-xr-x   0 jparadis   (501) staff       (20)        0 2024-05-03 13:23:43.733917 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/
+-rw-r--r--   0 jparadis   (501) staff       (20)     2555 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/README.markdown
+-rw-r--r--   0 jparadis   (501) staff       (20)      352 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/contributors.txt
+-rw-r--r--   0 jparadis   (501) staff       (20)    12246 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email.html
+-rw-r--r--   0 jparadis   (501) staff       (20)     6542 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email_lite.html
+-rwxr-xr-x   0 jparadis   (501) staff       (20)       26 2023-05-05 14:19:38.000000 django_mailing-0.2.2/mailing/views.py
+-rw-r--r--   0 jparadis   (501) staff       (20)       38 2024-05-03 13:23:43.735773 django_mailing-0.2.2/setup.cfg
+-rwxr-xr-x   0 jparadis   (501) staff       (20)     1099 2023-05-05 14:19:38.000000 django_mailing-0.2.2/setup.py
```

### Comparing `django-mailing-0.2.1/LICENSE.txt` & `django_mailing-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/PKG-INFO` & `django_mailing-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailing
-Version: 0.2.1
+Version: 0.2.2
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-mailing-0.2.1/README.txt` & `django_mailing-0.2.2/README.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/django_mailing.egg-info/PKG-INFO` & `django_mailing-0.2.2/django_mailing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailing
-Version: 0.2.1
+Version: 0.2.2
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-mailing-0.2.1/django_mailing.egg-info/SOURCES.txt` & `django_mailing-0.2.2/django_mailing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/docs/usage.txt` & `django_mailing-0.2.2/docs/usage.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/mailing/__init__.py` & `django_mailing-0.2.2/mailing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Versioning
 # --------------------------------
 #VERSION = (0, 1, 0, "beta", 11) # following PEP 386
-VERSION = (0, 2, 1, "f") # following PEP 386
+VERSION = (0, 2, 2, "f") # following PEP 386
 DEV_N = None
 
 def get_version():
     version = "%s.%s" % (VERSION[0], VERSION[1])
     if VERSION[2]:
         version = "%s.%s" % (version, VERSION[2])
     if VERSION[3] != "f":
```

### Comparing `django-mailing-0.2.1/mailing/mail.py` & `django_mailing-0.2.2/mailing/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
         self.value = value
     def __str__(self):
         return repr(self.value if value else '')
 
 def send_email_default(*args, **kwargs):
     send_email(args[3],args[0],args[1], from_email=args[2], category='django core email')
 
-def send_email(recipients, subject, text_content=None, html_content=None, from_email=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None):
+def send_email(recipients, subject, text_content=None, html_content=None, from_email=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None, reply_to=None):
     """
     Will send a multi-format email to recipients. Email may be queued through celery
     """
     from django.conf import settings
     if not bypass_queue and hasattr(settings, 'MAILING_USE_CELERY') and settings.MAILING_USE_CELERY:
         from celery.execute import send_task
-        return send_task('mailing.queue_send_email',[recipients, subject, text_content, html_content, from_email, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files])
+        return send_task('mailing.queue_send_email',[recipients, subject, text_content, html_content, from_email, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files, reply_to])
     else:
 
         header_category_value = '%s%s' % (settings.MAILING_HEADER_CATEGORY_PREFIX if hasattr(settings, 'MAILING_HEADER_CATEGORY_PREFIX') else '', category)
         # Check for sendgrid support and add category header
         # --------------------------------
         if hasattr(settings, 'MAILING_USE_SENDGRID'):
             send_grid_support = settings.MAILING_USE_SENDGRID
@@ -79,15 +79,15 @@
         if text_content or html_content:
             if use_base_template:
                 prev_language = translation.get_language()
                 language and translation.activate(language)
                 text_content = render_to_string('mailing/base.txt', {'mailing_text_body': text_content, 'mailing_subject': subject, 'settings': settings}) if text_content else None
                 html_content = render_to_string('mailing/base.html', {'mailing_html_body': html_content, 'mailing_subject': subject, 'settings': settings}) if html_content else None
                 translation.activate(prev_language)
-            msg = EmailMultiAlternatives(subject, text_content if text_content else html_content, from_email if from_email else settings.DEFAULT_FROM_EMAIL, recipients_list, cc=cc, bcc=bcc, attachments=attachments, headers = headers)
+            msg = EmailMultiAlternatives(subject, text_content if text_content else html_content, from_email if from_email else settings.DEFAULT_FROM_EMAIL, recipients_list, cc=cc, bcc=bcc, attachments=attachments, headers = headers, reply_to=reply_to)
             if html_content and text_content:
                 msg.attach_alternative(html_content, "text/html")
             elif html_content: # Only HTML
                 msg.content_subtype = "html"
 
             # Attach files through attach_files helper
             # --------------------------------
```

### Comparing `django-mailing-0.2.1/mailing/shortcuts.py` & `django_mailing-0.2.2/mailing/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from django.conf import settings
 from django.template.loader import render_to_string
 from django.template import TemplateDoesNotExist
 from django.utils import translation
 
 from mailing.mail import send_email
 
-def render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None):
+def render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None, reply_to=None):
     if not bypass_queue and hasattr(settings, 'MAILING_USE_CELERY') and settings.MAILING_USE_CELERY:
         from celery.execute import send_task
-        return send_task('mailing.queue_render_send_email',[recipients, template, data, from_email, subject, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files])
+        return send_task('mailing.queue_render_send_email',[recipients, template, data, from_email, subject, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files, reply_to])
     else:
         # Set language
         # --------------------------------
         prev_language = translation.get_language()
         language and translation.activate(language)
         if subject:
             my_subject = subject
@@ -35,9 +35,9 @@
 
         try:
             html_content = render_to_string('%s.html' % template, data)
         except TemplateDoesNotExist:
             html_content = None
 
         translation.activate(prev_language)
-        send_email(recipients, my_subject, text_content, html_content, from_email, use_base_template, category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files)
+        send_email(recipients, my_subject, text_content, html_content, from_email, use_base_template, category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to)
```

### Comparing `django-mailing-0.2.1/mailing/tasks.py` & `django_mailing-0.2.2/mailing/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 
 from celery.utils.log import get_task_logger
 
 logger = get_task_logger(__name__)
 
 @shared_task(name="mailing.queue_send_email")
-def queue_send_email(recipients, subject, text_content=None, html_content=None, from_email=settings.DEFAULT_FROM_EMAIL, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None): 
+def queue_send_email(recipients, subject, text_content=None, html_content=None, from_email=settings.DEFAULT_FROM_EMAIL, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None, reply_to=None): 
     
     logger.debug('Sending %s to %s' % (subject, ','.join(recipients), ))
 
-    send_email(recipients=recipients, subject=subject, text_content=text_content, html_content=html_content, from_email=from_email, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files)
+    send_email(recipients=recipients, subject=subject, text_content=text_content, html_content=html_content, from_email=from_email, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to)
 
     return True
 
 @shared_task(name="mailing.queue_render_send_email")
-def queue_render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None):
+def queue_render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None, reply_to=None):
     
     logger.debug('Rendering and sending %s to %s' % (template, ','.join(recipients), ))
 
-    render_send_email(recipients=recipients, template=template, data=data, from_email=from_email, subject=subject, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files)
+    render_send_email(recipients=recipients, template=template, data=data, from_email=from_email, subject=subject, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files, reply_to=reply_to)
 
     return True
```

### Comparing `django-mailing-0.2.1/mailing/templates/mailing/base.html` & `django_mailing-0.2.2/mailing/templates/mailing/base.html`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/README.markdown` & `django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/README.markdown`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/email.html` & `django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email.html`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/mailing/templates/mailing/email_boiletplate/email_lite.html` & `django_mailing-0.2.2/mailing/templates/mailing/email_boiletplate/email_lite.html`

 * *Files identical despite different names*

### Comparing `django-mailing-0.2.1/setup.py` & `django_mailing-0.2.2/setup.py`

 * *Files identical despite different names*

