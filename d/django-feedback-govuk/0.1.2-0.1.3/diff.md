# Comparing `tmp/django_feedback_govuk-0.1.2.tar.gz` & `tmp/django_feedback_govuk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feedback_govuk-0.1.2.tar", max compression
+gzip compressed data, was "django_feedback_govuk-0.1.3.tar", max compression
```

## Comparing `django_feedback_govuk-0.1.2.tar` & `django_feedback_govuk-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,32 @@
--rw-r--r--   0        0        0     1091 2023-03-14 11:04:30.618076 django_feedback_govuk-0.1.2/LICENSE
--rw-r--r--   0        0        0     2786 2023-04-11 10:12:43.934435 django_feedback_govuk-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.2/django_feedback_govuk/__init__.py
--rw-r--r--   0        0        0       95 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.2/django_feedback_govuk/admin.py
--rw-r--r--   0        0        0     1652 2023-04-11 10:35:22.354859 django_feedback_govuk-0.1.2/django_feedback_govuk/forms.py
--rw-r--r--   0        0        0     1840 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.2/django_feedback_govuk/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.2/django_feedback_govuk/migrations/__init__.py
--rw-r--r--   0        0        0      920 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.2/django_feedback_govuk/models.py
--rw-r--r--   0        0        0      789 2023-04-11 10:31:05.018794 django_feedback_govuk-0.1.2/django_feedback_govuk/notify.py
--rw-r--r--   0        0        0     2061 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.2/django_feedback_govuk/settings.py
--rw-r--r--   0        0        0     3357 2023-03-14 16:49:16.438614 django_feedback_govuk-0.1.2/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
--rw-r--r--   0        0        0     2339 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
--rw-r--r--   0        0        0      180 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
--rw-r--r--   0        0        0     1399 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
--rw-r--r--   0        0        0      351 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
--rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
--rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
--rw-r--r--   0        0        0       48 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
--rw-r--r--   0        0        0     1898 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
--rw-r--r--   0        0        0     1737 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
--rw-r--r--   0        0        0        0 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/templatetags/__init__.py
--rw-r--r--   0        0        0     1605 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.2/django_feedback_govuk/templatetags/feedback_tags.py
--rw-r--r--   0        0        0      471 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/urls.py
--rw-r--r--   0        0        0     1826 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.2/django_feedback_govuk/views.py
--rw-r--r--   0        0        0     1789 2023-04-11 10:35:52.255772 django_feedback_govuk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.2/setup.py
--rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-14 11:04:30.618076 django_feedback_govuk-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2786 2023-04-11 10:12:43.934435 django_feedback_govuk-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/admin.py
+-rw-r--r--   0        0        0     1652 2023-04-11 10:35:22.354859 django_feedback_govuk-0.1.3/django_feedback_govuk/forms.py
+-rw-r--r--   0        0        0     1840 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/migrations/__init__.py
+-rw-r--r--   0        0        0      920 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/models.py
+-rw-r--r--   0        0        0      789 2023-04-11 10:31:05.018794 django_feedback_govuk-0.1.3/django_feedback_govuk/notify.py
+-rw-r--r--   0        0        0     2061 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/settings.py
+-rw-r--r--   0        0        0     3357 2023-03-14 16:49:16.438614 django_feedback_govuk-0.1.3/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
+-rw-r--r--   0        0        0     2339 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
+-rw-r--r--   0        0        0      180 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
+-rw-r--r--   0        0        0     1399 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
+-rw-r--r--   0        0        0      351 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
+-rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
+-rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
+-rw-r--r--   0        0        0       48 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
+-rw-r--r--   0        0        0     1898 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
+-rw-r--r--   0        0        0     1737 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
+-rw-r--r--   0        0        0        0 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templatetags/__init__.py
+-rw-r--r--   0        0        0     1605 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/templatetags/feedback_tags.py
+-rw-r--r--   0        0        0        0 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/factories.py
+-rw-r--r--   0        0        0     1870 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/settings.py
+-rw-r--r--   0        0        0      558 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/test_views.py
+-rw-r--r--   0        0        0      153 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/urls.py
+-rw-r--r--   0        0        0      471 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/urls.py
+-rw-r--r--   0        0        0     1826 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/views.py
+-rw-r--r--   0        0        0     1877 2023-04-19 11:46:43.895872 django_feedback_govuk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.3/setup.py
+-rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.3/PKG-INFO
```

### Comparing `django_feedback_govuk-0.1.2/LICENSE` & `django_feedback_govuk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/README.md` & `django_feedback_govuk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/forms.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/forms.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/migrations/0001_initial.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/models.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/models.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/notify.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/notify.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/settings.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/static/django_feedback_govuk/star-rating.css` & `django_feedback_govuk-0.1.3/django_feedback_govuk/static/django_feedback_govuk/star-rating.css`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html` & `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html` & `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html` & `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html` & `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/templatetags/feedback_tags.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/templatetags/feedback_tags.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/django_feedback_govuk/views.py` & `django_feedback_govuk-0.1.3/django_feedback_govuk/views.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.2/pyproject.toml` & `django_feedback_govuk-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-feedback-govuk"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Django app to gather and send internal Government staff feedback"
 authors = ["jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>", "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_feedback_govuk"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -17,27 +17,32 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Django = "^3.2"
+Django = ">=3.2,<4.3"
 crispy-forms-gds = "^0.2.4"
 notifications-python-client = "^8.0.0"
 django-crispy-forms = "^1.9"
 
+[tool.poetry.group.testing.dependencies]
+pytest = "^7.2.2"
+pytest-django = "^4.5.2"
+coverage = "^7.2.1"
+tox = "^4.4.12"
+factory-boy = "^3.2.1"
+
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 djlint = "^1.19.16"
-pytest = "^7.2.2"
-pytest-django = "^4.5.2"
-coverage = "^7.2.1"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "7.0"
```

### Comparing `django_feedback_govuk-0.1.2/setup.py` & `django_feedback_govuk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['django_feedback_govuk',
  'django_feedback_govuk.migrations',
- 'django_feedback_govuk.templatetags']
+ 'django_feedback_govuk.templatetags',
+ 'django_feedback_govuk.tests']
 
 package_data = \
 {'': ['*'],
  'django_feedback_govuk': ['static/django_feedback_govuk/*',
                            'templates/django_feedback_govuk/includes/*',
                            'templates/django_feedback_govuk/partials/*',
                            'templates/django_feedback_govuk/templates/*',
                            'templates/django_feedback_govuk/widgets/star_rating/*']}
 
 install_requires = \
-['Django>=3.2,<4.0',
+['Django>=3.2,<4.3',
  'crispy-forms-gds>=0.2.4,<0.3.0',
  'django-crispy-forms>=1.9,<2.0',
  'notifications-python-client>=8.0.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'django-feedback-govuk',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A Django app to gather and send internal Government staff feedback',
     'long_description': '# django-feedback\n\nA Django app to gather and send internal Government staff feedback, e.g. for open beta periods\n\n## Installation\n\n```\npip install django-feedback-govuk\n```\n\n1. Add `django-feedback` to your INSTALLED_APPS settings:\n\n```py\nINSTALLED_APPS = [\n    ...\n    \'crispy_forms\',\n    \'crispy_forms_gds\',\n    \'django_feedback_govuk\',\n]\n```\n\n2. Create a new email template in the GovUk Notify service, making sure to create a ((feedback_url)) field.\n\n> Note that ((feedback_url)) will be a link to the listing view, not an individual piece of feedback.\n\nYou\'ll need an API key and template ID from the gov.uk Notify service.\n\n3. Add the following settings to the file:\n\n```py\n# Crispy forms\nCRISPY_ALLOWED_TEMPLATE_PACKS = ["gds"]\nCRISPY_TEMPLATE_PACK = "gds"\n\n# Gov Notify\nGOVUK_NOTIFY_API_KEY="<your-api-key>"\n\n# Django Feedback GovUK\nDJANGO_FEEDBACK_GOVUK = {\n    "SERVICE_NAME": "<your-service>",\n    "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",\n    "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": ["email@example.com"],\n    "COPY": {\n        #...add any copy tags to override here\n    }\n}\n\nThe copy dict contains string IDs for all user-facing copy, defaulting to the following (override\njust the fields you want to, using the `{{ service_name }}` variable if necessary for _title and _body strings):\n\n```py\n{\n    "SUBMIT_TITLE": "Give feedback on {{ service_name }}",\n    "CONFIRM_TITLE": "Feedback submitted",\n    "CONFIRM_BODY": "Thank you for submitting your feedback.",\n    "FIELD_SATISFACTION_LEGEND": "Overall, how did you feel about the service you received today?",\n    "FIELD_COMMENT_LEGEND": "How could we improve this service?",\n    "FIELD_COMMENT_HINT": "Do not include any personal or financial information, for example your National Insurance or credit card numbers.",\n}\n```\n\nThe email addresses are for every recipient that should get an email when feedback is submitted.\n\n3. Build your own templates\n\nOverride the built-in templates by making new templates in your app under the\n`django_feedback_govuk/templates` path. You\'ll need templates for `submit.html`, `confirm.html`\nand `listing.html`, each of which should load its respective template tag from `feedback_submit`,\n`feedback_confirm` and `feedback_listing`.\n\nFor example:\n\n```py\n{# /your-project/templates/django_feedback_govuk/templates/submit.html #}\n{% extends "base.html" %}\n{% load feedback_tags %}\n{% block content %}\n    {% feedback_submit %}\n{% endblock content %}\n```\n\n> If you\'d like to use the templatetags without causing page loads to new views\n\n4. Add the URLs to your project\n\n```py\nfrom django_feedback_govuk import urls as feedback_urls\n\n\nurlpatterns = [\n    ...\n    path("feedback/", include(feedback_urls)),\n    ...\n]\n```\n\n5. Set up user permissions\n',
     'author': 'jafacakes2011',
     'author_email': 'cameron.lamb@digitial.trade.gov.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `django_feedback_govuk-0.1.2/PKG-INFO` & `django_feedback_govuk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feedback-govuk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django app to gather and send internal Government staff feedback
 License: MIT
 Author: jafacakes2011
 Author-email: cameron.lamb@digitial.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Django (>=3.2,<4.0)
+Requires-Dist: Django (>=3.2,<4.3)
 Requires-Dist: crispy-forms-gds (>=0.2.4,<0.3.0)
 Requires-Dist: django-crispy-forms (>=1.9,<2.0)
 Requires-Dist: notifications-python-client (>=8.0.0,<9.0.0)
 Description-Content-Type: text/markdown
 
 # django-feedback
```

