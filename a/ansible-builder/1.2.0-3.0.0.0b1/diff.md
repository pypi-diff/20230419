# Comparing `tmp/ansible-builder-1.2.0.tar.gz` & `tmp/ansible-builder-3.0.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-builder-1.2.0.tar", last modified: Tue Nov  1 21:56:28 2022, max compression
+gzip compressed data, was "ansible-builder-3.0.0.0b1.tar", last modified: Wed Apr 19 15:45:27 2023, max compression
```

## Comparing `ansible-builder-1.2.0.tar` & `ansible-builder-3.0.0.0b1.tar`

### file list

```diff
@@ -1,200 +1,224 @@
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      210 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.cherry_picker.toml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      288 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.coveragerc
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       25 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.dockerignore
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.github/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2036 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       27 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      623 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/documentation_report.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      600 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       23 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/issue_labeler.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      113 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/patchback.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       37 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/pr_labeler_existing.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       90 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/pr_labeler_new.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.github/test-scripts/
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     4593 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/test-scripts/setup_pulp.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.github/workflows/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4836 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      763 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/workflows/triage_existing.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      734 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.github/workflows/triage_new.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      334 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.readthedocs.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      476 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.yamllint
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.zuul.d/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1764 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.zuul.d/jobs.yaml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.zuul.d/playbooks/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.zuul.d/playbooks/.zuul.ignore
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/.zuul.d/playbooks/ansible-builder-build-container-image/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      331 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.zuul.d/playbooks/ansible-builder-build-container-image/pre.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      444 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/.zuul.d/project.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1142 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/AUTHORS
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      306 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/CODEOWNERS
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1176 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    16034 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ChangeLog
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      887 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/Containerfile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9302 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/LICENSE.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3008 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/Makefile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2016 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/PKG-INFO
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1766 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/README.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      313 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/SECURITY.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      494 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/TODO.org
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.634431 ansible-builder-1.2.0/ansible_builder/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10699 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/cli.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      157 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/colors.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1044 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/constants.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      271 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/exceptions.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6673 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/introspect.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    17733 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/main.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4633 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/policies.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3084 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/requirements.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3751 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/steps.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10613 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/user_definition.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5263 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/ansible_builder/utils.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/ansible_builder.egg-info/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2016 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/PKG-INFO
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4475 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/SOURCES.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/dependency_links.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/entry_points.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/not-zip-safe
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       47 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/pbr.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       34 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/requires.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       16 2022-11-01 21:56:28.000000 ansible-builder-1.2.0/ansible_builder.egg-info/top_level.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      211 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/demo/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      257 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/demo/execution-environment.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       31 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/demo/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/demo/requirements.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/docs/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      612 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/Makefile
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/docs/_static/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/_static/.gitkeep
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/docs/_templates/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/_templates/.gitkeep
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2581 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/collection_metadata.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4796 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/conf.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7581 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/definition.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      543 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/glossary.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2082 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/index.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      861 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/installation.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      819 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/make.bat
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/requirements.in
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      491 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7677 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/docs/usage.rst
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.632431 ansible-builder-1.2.0/packaging/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/packaging/rpm/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      257 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/packaging/rpm/Dockerfile.epel-7-x86_64
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      167 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/packaging/rpm/Dockerfile.epel-8-x86_64
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      921 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/packaging/rpm/ansible-builder.spec.j2
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      457 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/packaging/rpm/docker-compose.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      464 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/pytest.ini
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       34 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      433 2022-11-01 21:56:28.638431 ansible-builder-1.2.0/setup.cfg
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      104 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/setup.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/test/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5587 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/conftest.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/test/data/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1857 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/README.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      420 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible-test.cfg
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/test/data/ansible.posix.at/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.635431 ansible-builder-1.2.0/test/data/ansible.posix.at/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      108 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible.posix.at/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible.posix.at/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/ansible.posix.at/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      577 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible.posix.at/project/ansible.posix.at.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      109 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible.posix.at/requirements.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      255 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible.posix.at/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.632431 ansible-builder-1.2.0/test/data/ansible_collections/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.632431 ansible-builder-1.2.0/test/data/ansible_collections/other/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/ansible_collections/other/reqfile/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       44 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/other/reqfile/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.632431 ansible-builder-1.2.0/test/data/ansible_collections/test/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/ansible_collections/test/bindep/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/bindep/MANIFEST.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/bindep/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/ansible_collections/test/metadata/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/metadata/MANIFEST.json
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/ansible_collections/test/metadata/meta/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       59 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/metadata/meta/execution-environment.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/metadata/my-requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/ansible_collections/test/reqfile/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/reqfile/MANIFEST.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/reqfile/extra_req.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/ansible_collections/test/reqfile/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/blank/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/blank/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       97 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/blank/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/blank/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/blank/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       99 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/blank/project/blank.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      237 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/blank/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/build_args/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      107 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/build_args/base-image.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/build_args/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/build_fail/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       78 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/build_fail/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/definition_files/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/definition_files/bad.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       12 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/definition_files/invalid.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/definition_files/no_galaxy.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/definition_files/no_python.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/foo/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       20 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/foo/requirements.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/needs_git/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/needs_git/execution-environment.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       82 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/needs_git/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/nested-galaxy.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/pip/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/pip/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       95 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pip/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       64 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pip/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/pip/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      131 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pip/project/pip.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pip/project/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pip/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.636431 ansible-builder-1.2.0/test/data/prepend_steps/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/prepend_steps/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/pytz/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/pytz/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       30 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pytz/env/extravars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       96 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pytz/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pytz/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/pytz/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      294 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pytz/project/pytz.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       35 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/pytz/requirements.yml
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)      699 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/subversion/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/subversion/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/subversion/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      102 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/subversion/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       50 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/subversion/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/subversion/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/subversion/project/subversion.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      241 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/subversion/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/v2/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5135 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/v2/RPM-GPG-KEY-redhat-release
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/v2/invalid-keyring
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/data/v2/sig_req/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      397 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/v2/sig_req/ee-good.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      289 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/data/v2/sig_req/ee-no-orig.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/integration/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/integration/conftest.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9983 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/integration/test_build.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5302 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/integration/test_create.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1425 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/integration/test_help.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2698 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/integration/test_introspect_cli.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/pulp_integration/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7877 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/pulp_integration/test_policies.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       72 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:56:28.637431 ansible-builder-1.2.0/test/unit/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8339 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_cli.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1212 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_introspect.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4898 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_main.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5909 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_policies.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1515 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_requirements.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2952 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_steps.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6668 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_user_definition.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2930 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/test/unit/test_utils.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1350 2022-11-01 21:53:34.000000 ansible-builder-1.2.0/tox.ini
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      210 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.cherry_picker.toml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      288 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.coveragerc
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       25 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.dockerignore
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2036 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       27 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      623 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/documentation_report.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      600 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       23 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/issue_labeler.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      113 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/patchback.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       37 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/pr_labeler_existing.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       90 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/pr_labeler_new.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/test-scripts/
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     4597 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/test-scripts/setup_pulp.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/.github/workflows/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4750 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/workflows/ci.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      763 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/workflows/triage_existing.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      734 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.github/workflows/triage_new.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      334 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.readthedocs.yaml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      547 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/.yamllint
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1229 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/AUTHORS
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      306 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/CODEOWNERS
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1176 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/CONTRIBUTING.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    17443 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ChangeLog
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      827 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/Containerfile
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     9302 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/LICENSE.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3008 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/Makefile
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2866 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/PKG-INFO
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1766 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/README.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      313 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/SECURITY.md
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      494 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/TODO.org
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/ansible_builder/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/__main__.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/__init__.py
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     6537 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/assemble
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     3474 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/check_ansible
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     1618 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/check_galaxy
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     1480 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/get-extras-packages
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)     3440 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/install-from-bindep
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    14022 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/_target_scripts/introspect.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     8136 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/cli.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      157 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/colors.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1198 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/constants.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    17011 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/containerfile.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    13396 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/ee_schema.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      407 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/exceptions.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     9107 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/main.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4633 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/policies.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     3084 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/requirements.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     8843 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/user_definition.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     6117 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/ansible_builder/utils.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2866 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5263 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        1 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/not-zip-safe
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       47 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/pbr.json
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       45 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/requires.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       16 2023-04-19 15:45:27.000000 ansible-builder-3.0.0.0b1/ansible_builder.egg-info/top_level.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      211 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/bindep.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/demo/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      257 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/execution-environment.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       31 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/requirements.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/demo/v3_demo/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1277 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/demo/v3_demo/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.465620 ansible-builder-3.0.0.0b1/docs/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      612 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/Makefile
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/docs/_static/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/_static/.gitkeep
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/docs/_templates/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/_templates/.gitkeep
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2581 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/collection_metadata.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5018 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/conf.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    10849 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/definition.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      543 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/glossary.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2082 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/index.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      861 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/installation.rst
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      819 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/make.bat
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       15 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/requirements.in
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      522 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     8293 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/docs/usage.rst
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/packaging/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/packaging/rpm/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      257 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/Dockerfile.epel-7-x86_64
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      167 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/Dockerfile.epel-8-x86_64
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      921 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/ansible-builder.spec.j2
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      457 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/packaging/rpm/docker-compose.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      464 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/pytest.ini
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       45 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1134 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/setup.cfg
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      133 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/setup.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5587 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/conftest.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1857 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/README.md
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      108 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/env/settings
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      577 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/project/ansible.posix.at.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      109 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/requirements.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      255 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/run.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_cfg_for_galaxy/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      420 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_cfg_for_galaxy/ansible-test.cfg
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_cfg_for_galaxy/requirements.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/other/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/other/reqfile/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       44 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/other/reqfile/requirements.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.457620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/bindep/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/bindep/MANIFEST.json
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       53 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/bindep/bindep.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        2 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/MANIFEST.json
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/meta/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       59 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/meta/execution-environment.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       13 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/metadata/my-requirements.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        2 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/MANIFEST.json
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       73 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/extra_req.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/ansible_collections/test/reqfile/requirements.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/blank/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/blank/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       97 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/env/settings
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       15 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/blank/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       99 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/project/blank.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      237 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/blank/run.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/build_args/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      107 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/build_args/base-image.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       73 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/build_args/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/build_fail/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       78 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/build_fail/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/definition_files/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      187 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/bad.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       12 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/invalid.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/no_galaxy.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/definition_files/no_python.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/needs_git/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/needs_git/execution-environment.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       82 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/needs_git/requirements.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.469620 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/foo/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       20 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/foo/requirements.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       60 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/nested_galaxy_file/nested-galaxy.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pip/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pip/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       95 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/env/settings
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       64 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pip/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      131 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/project/pip.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       26 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/project/requirements.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      239 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pip/run.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/prepend_steps/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       67 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/prepend_steps/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pytz/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pytz/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       30 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/env/extravars
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       96 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/env/settings
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       56 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/pytz/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      294 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/project/pytz.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       35 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/pytz/requirements.yml
+-rwxrwxr-x   0 shrews    (1000) shrews    (1000)      699 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/run.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/subversion/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       53 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/bindep.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/subversion/env/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      102 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/env/settings
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)       50 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/execution-environment.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/subversion/project/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      239 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/project/subversion.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      241 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/subversion/run.sh
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v2/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5135 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/RPM-GPG-KEY-redhat-release
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/invalid-keyring
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v2/sig_req/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      397 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/sig_req/ee-good.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      289 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v2/sig_req/ee-no-orig.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.461620 ansible-builder-3.0.0.0b1/test/data/v3/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      258 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/ee-missing-ansible.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      254 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/ee-missing-runner.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      235 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/check_ansible/ee-skip.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      685 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/ee.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/a.dat
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/text_files/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/data/text_files/a.txt
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/complete/files/random.cfg
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/data/v3/pre_and_post/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      427 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/pre_and_post/ee.yml
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/data/v3/pre_and_post/requirements.yml
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/integration/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/conftest.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    10171 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_build.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    11995 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_create.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1425 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_help.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2698 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/integration/test_introspect_cli.py
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.473620 ansible-builder-3.0.0.0b1/test/pulp_integration/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     7877 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/pulp_integration/test_policies.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1715 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/pulp_integration/test_v3.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)      114 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/requirements.txt
+drwxrwxr-x   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:45:27.477620 ansible-builder-3.0.0.0b1/test/unit/
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)        0 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/__init__.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    10219 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_cli.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4871 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_containerfile.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1228 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_introspect.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     4927 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_main.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     5909 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_policies.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1515 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_requirements.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)    11769 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_user_definition.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     2930 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/test/unit/test_utils.py
+-rw-rw-r--   0 shrews    (1000) shrews    (1000)     1474 2023-04-19 15:39:17.000000 ansible-builder-3.0.0.0b1/tox.ini
```

### Comparing `ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/documentation_report.yml` & `ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/documentation_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `ansible-builder-3.0.0.0b1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/.github/test-scripts/setup_pulp.sh` & `ansible-builder-3.0.0.0b1/.github/test-scripts/setup_pulp.sh`

 * *Files 1% similar despite different names*

```diff
@@ -107,11 +107,11 @@
 # See https://github.com/containers/skopeo/issues/942 for more info.
 ##############################################################################
 
 export XDG_RUNTIME_DIR=/tmp/pulptests
 mkdir $XDG_RUNTIME_DIR
 
 skopeo login --username admin --password password localhost:8080 --tls-verify=false
-skopeo copy docker://registry.access.redhat.com/ubi9/ubi-micro:latest docker://localhost:8080/testrepo/ubi-micro --dest-tls-verify=false
+skopeo copy docker://registry.access.redhat.com/ubi9/ubi-minimal:latest docker://localhost:8080/testrepo/ubi-minimal --dest-tls-verify=false
 
 podman login --username "$1" --password "$2" registry.redhat.io
 skopeo copy docker://registry.redhat.io/ansible-automation-platform-21/ansible-builder-rhel8:latest docker://localhost:8080/testrepo/ansible-builder-rhel8 --dest-tls-verify=false
```

### Comparing `ansible-builder-1.2.0/.github/workflows/ci.yml` & `ansible-builder-3.0.0.0b1/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -4,58 +4,60 @@
   pull_request:
   push:
 
 
 jobs:
   sanity:
     name: ${{ matrix.test.name }}
-    runs-on: ubuntu-20.04
-    container:
-      image: quay.io/ansible/ansible-builder-test-container:2.0.0
-      env:
-        PIP_CACHE_DIR: ${{ runner.temp }}/.cache/pip
-        TOXENV: ${{ matrix.test.tox_env }}
+    runs-on: ubuntu-22.04
+    env:
+      TOXENV: ${{ matrix.test.tox_env }}
 
     strategy:
       fail-fast: false
       matrix:
         test:
           - name: Lint
-            tox_env: linters
+            tox_env: linters-py310
 
           - name: Docs
             tox_env: docs
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
+      - name: Install tox
+        run: |
+          python3 -m pip install --upgrade pip
+          python3 -m pip install tox
+
       - name: Create tox environment
         run: tox --notest
 
       - name: Run tests
         run: tox
 
   secrets_preflight:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     name: Secrets pre-flight check
     env:
       secret_user: ${{ secrets.RH_REGISTRY_USER }}
       secret_pass: ${{ secrets.RH_REGISTRY_PASSWORD }}
     steps:
       - id: has_secrets
         if: ${{ env.secret_user != '' && env.secret_pass != '' }}
         run: |
-          echo "::set-output name=has_secrets::${{ true }}"
+          echo "has_secrets=${{ true }}" >> $GITHUB_OUTPUT
     outputs:
       has_secrets: ${{ steps.has_secrets.outputs.has_secrets }}
 
 
   pulp_integration:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     name: Pulp Integration - ${{ matrix.py_version.name }}
     # NB: running this job requires access to an RH registry token; PRs can't currently access the main repo secret,
     # so forks will need to define the secrets locally to run these tests pre-merge
     needs: secrets_preflight
     if: needs.secrets_preflight.outputs.has_secrets == 'true'
 
     env:
@@ -99,33 +101,32 @@
 
       - name: Run pulp integration tests
         run: |
           tox
 
 
   integration:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     name: Integration - ${{ matrix.py_version.name }}
 
     env:
       TOXENV: ${{ matrix.py_version.tox_env }}
 
     strategy:
       fail-fast: false
       matrix:
         py_version:
-          - name: '3.8'
-            tox_env: integration-py38
-
           - name: '3.9'
             tox_env: integration-py39
 
           - name: '3.10'
             tox_env: integration-py310
 
+          - name: '3.11'
+            tox_env: integration-py311
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Install Python ${{ matrix.py_version.name }}
         uses: actions/setup-python@v4
@@ -139,52 +140,59 @@
 
       - name: Create tox environment
         run: |
           tox --notest
 
       - name: Run integration tests
         run: |
-          docker build --rm=true -t quay.io/ansible/ansible-builder -f Containerfile .
-          podman build --rm=true -t quay.io/ansible/ansible-builder -f Containerfile .
           tox
 
       - name: Upload coverage report
-        run: |
-          curl --silent --show-error --output codecov https://ansible-ci-files.s3.us-east-1.amazonaws.com/codecov/linux/codecov
-          chmod +x codecov
-          ./codecov --file test/coverage/reports/coverage.xml --flags {{ matrix.py_version.tox_env }}
-
+        uses: codecov/codecov-action@v3
+        with:
+          files: test/coverage/reports/coverage.xml
+          flags: ${{ matrix.py_version.tox_env }}
 
   unit:
     name: Unit - ${{ matrix.py_version.name}}
-    runs-on: ubuntu-20.04
-    container:
-      image: quay.io/ansible/ansible-builder-test-container:2.0.0
-      env:
-        PIP_CACHE_DIR: ${{ runner.temp }}/.cache/pip
-        TOXENV: ${{ matrix.py_version.tox_env }}
+    runs-on: ubuntu-22.04
+    env:
+      TOXENV: ${{ matrix.py_version.tox_env }}
 
     strategy:
       fail-fast: false
       matrix:
         py_version:
-          - name: '3.8'
-            tox_env: unit-py38
-
           - name: '3.9'
             tox_env: unit-py39
 
           - name: '3.10'
             tox_env: unit-py310
 
+          - name: '3.11'
+            tox_env: unit-py311
+
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
+      - name: Install Python ${{ matrix.py_version.name }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.py_version.name }}
+
+      - name: Install tox
+        run: |
+          python3 -m pip install --upgrade pip
+          python3 -m pip install tox
+
       - name: Create tox environment
         run: tox --notest
 
       - name: Run tests
         run: tox
 
       - name: Upload coverage report
-        run: codecov --file test/coverage/reports/coverage.xml --flags {{ matrix.py_version.tox_env }}
+        uses: codecov/codecov-action@v3
+        with:
+          files: test/coverage/reports/coverage.xml
+          flags: ${{ matrix.py_version.tox_env }}
```

### Comparing `ansible-builder-1.2.0/.github/workflows/triage_existing.yml` & `ansible-builder-3.0.0.0b1/.github/workflows/triage_existing.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/.github/workflows/triage_new.yml` & `ansible-builder-3.0.0.0b1/.github/workflows/triage_new.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/AUTHORS` & `ansible-builder-3.0.0.0b1/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 Alan Rominger <arominge@redhat.com>
 AlanCoding <arominge@redhat.com>
 Alexander Sowitzki <asowitzk@redhat.com>
 Bianca Henderson <beeankha@gmail.com>
 Bianca Henderson <bstohrer@redhat.com>
 Bill Nottingham <notting@redhat.com>
 Dave Safanyuk <dsafanyuk@gmail.com>
+David Schmidt <51931019+schmidtd@users.noreply.github.com>
 David Shrewsbury <Shrews@users.noreply.github.com>
 David Shrewsbury <dshrewsb@redhat.com>
+Don Naro <dnaro@redhat.com>
 Elijah DeLee <kdelee@redhat.com>
 Ellen Marie Dash <me@duckie.co>
 Jake Jackson <jljacks93@gmail.com>
 James Tanner <tanner.jc@gmail.com>
 Matt Davis <6775756+nitzmahone@users.noreply.github.com>
 Matt Davis <mrd@redhat.com>
 Matthew Jones <bsdmatburt@gmail.com>
```

### Comparing `ansible-builder-1.2.0/CONTRIBUTING.md` & `ansible-builder-3.0.0.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/ChangeLog` & `ansible-builder-3.0.0.0b1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,50 @@
 CHANGES
 =======
 
-1.2.0
------
+3.0.0b1
+-------
 
-* [backport][release\_1.2] Update CI GH actions (#421)
+* Add Python 3.11 testing (#474)
+* Misc typo fixes (#471)
+* Prefer COPY over ADD (#466)
+* Remove set-output syntax in GH workflow (#459)
+* Do not build local builder image in CI (#469)
+* Change ansible\_core/ansible\_runner schema types (#464)
+* add container\_init customization (#18)
+* Add option for package manager (#17)
+* Add check for Ansible/Runner in final image
+* Bump schema to v3 (#15)
+* Remove py3.8 classifier
+* Carry over fix for v2 default images
+* Add check for ansible-galaxy before galaxy installs
+* Revise help for --squash option
+* Revise docs for --squash option
+* Add squash feature
+* Set user to root in base image
+* Add mypy to linters job and correct existing errors
+* Support directories being the src for additional\_build\_files
+* Support additional build files
+* [feature] allow custom commands before and after build phases (#7)
+* Enforce min python version and lint fixes
+* Move steps.py code to containerfile.py
+* Split Containerfile class
+* Fixes for integration tests
+* Use jsonschema for EE schema validation (#3)
+* Fix CI failures (#1)
+* wip
+* Clarify help (#456)
+* Make sure default images are used with v2 schema (#455)
+* Add license and classifiers metadata (#449)
+* Bump certifi from 2021.10.8 to 2022.12.7 in /docs (#441)
+* Check minimum Python version (#415)
+* Update yamllint config for new 1.29.0 version (#440)
+* Docs: Use the Ansible Sphinx theme (#439)
+* Remove Zuul remnants (#428)
+* Update CI GH actions (#420)
 * Container image signature validation (#371)
 * Fix secrets\_preflight check (#405)
 * only run pulp tests when registry secrets are available
 * setup\_pulp.sh now expects username as passed in secret
 * Have setup\_pulp.sh exit early if pwd is empty
 * Move test script, some cleanup
 * Add pulp\_integration framework
```

### Comparing `ansible-builder-1.2.0/LICENSE.md` & `ansible-builder-3.0.0.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/Makefile` & `ansible-builder-3.0.0.0b1/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/PKG-INFO` & `ansible-builder-3.0.0.0b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: ansible-builder
-Version: 1.2.0
-Summary: "A tool for building Ansible Execution Environments"
-Home-page: https://ansible-builder.readthedocs.io
-Author: Ansible, Inc.
-Author-email: info@ansible.com
-License-File: LICENSE.md
-
 [![CI](https://github.com/ansible/ansible-builder/actions/workflows/ci.yml/badge.svg?branch=devel)](https://github.com/ansible/ansible-builder/actions?query=branch%3Adevel)
 [![codecov](https://codecov.io/gh/ansible/ansible-builder/branch/devel/graph/badge.svg?token=4F6P3DBI40)](https://codecov.io/gh/ansible/ansible-builder)
 
 # Ansible Builder
 
 Ansible Builder is a tool that automates the process of building execution
 environments using the schemas and tooling defined in various Ansible
```

### Comparing `ansible-builder-1.2.0/ansible_builder/cli.py` & `ansible-builder-3.0.0.0b1/ansible_builder/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import argparse
 import logging
 import sys
-import yaml
 import os
 import pkg_resources
 
 from . import constants
 
 from .colors import MessageColors
 from .exceptions import DefinitionError
 from .main import AnsibleBuilder
 from .policies import PolicyChoices
-from .introspect import process, simple_combine, base_collections_path
-from .requirements import sanitize_requirements
-from .utils import configure_logger, write_file
+from ._target_scripts.introspect import create_introspect_parser, run_introspect
+from .utils import configure_logger
 
 
 logger = logging.getLogger(__name__)
 
 
 def run():
     args = parse_args()
@@ -34,37 +32,17 @@
                     ) + MessageColors.ENDC)
                 sys.exit(0)
         except DefinitionError as e:
             logger.error(e.args[0])
             sys.exit(1)
 
     elif args.action == 'introspect':
-        data = process(args.folder, user_pip=args.user_pip, user_bindep=args.user_bindep)
-        if args.sanitize:
-            logger.info('# Sanitized dependencies for %s', args.folder)
-            data_for_write = data
-            data['python'] = sanitize_requirements(data['python'])
-            data['system'] = simple_combine(data['system'])
-        else:
-            logger.info('# Dependency data for %s', args.folder)
-            data_for_write = data.copy()
-            data_for_write['python'] = simple_combine(data['python'])
-            data_for_write['system'] = simple_combine(data['system'])
-
-        print('---')
-        print(yaml.dump(data, default_flow_style=False))
-
-        if args.write_pip and data.get('python'):
-            write_file(args.write_pip, data_for_write.get('python') + [''])
-        if args.write_bindep and data.get('system'):
-            write_file(args.write_bindep, data_for_write.get('system') + [''])
+        run_introspect(args, logger)
 
-        sys.exit(0)
-
-    logger.error("An error has occured.")
+    logger.error("An error has occurred.")
     sys.exit(1)
 
 
 def get_version():
     return pkg_resources.get_distribution('ansible_builder').version
 
 
@@ -138,14 +116,21 @@
     )
 
     build_command_parser.add_argument(
         '--container-keyring',
         help='GPG keyring for container image validation.',
     )
 
+    build_command_parser.add_argument(
+        '--squash',
+        choices=['new', 'all', 'off'],
+        default='new',
+        help='Squash layers in the final image (choices: %(choices)s). Defaults to "%(default)s". (podman only)'
+    )
+
     for p in [create_command_parser, build_command_parser]:
 
         p.add_argument('-f', '--file',
                        default=constants.default_file,
                        dest='filename',
                        help='The definition of the execution environment (default: %(default)s)')
 
@@ -169,54 +154,15 @@
                        action="append",
                        help='A gpg status code to ignore during signature verification when installing with '
                        'ansible-galaxy. May be specified multiple times. See ansible-galaxy doc for more info.')
         p.add_argument('--galaxy-required-valid-signature-count',
                        help='The number of signatures that must successfully verify collections from '
                        'ansible-galaxy ~if there are any signatures provided~. See ansible-galaxy doc for more info.')
 
-    introspect_parser = parser.add_parser(
-        'introspect',
-        help='Introspects collections in folder.',
-        description=(
-            'Loops over collections in folder and returns data about dependencies. '
-            'This is used internally and exposed here for verification. '
-            'This is targeted toward collection authors and maintainers.'
-        )
-    )
-    introspect_parser.add_argument('--sanitize', action='store_true',
-                                   help=('Sanitize and de-duplicate requirements. '
-                                         'This is normally done separately from the introspect script, but this '
-                                         'option is given to more accurately test collection content.'))
-
-    introspect_parser.add_argument(
-        'folder', default=base_collections_path, nargs='?',
-        help=(
-            'Ansible collections path(s) to introspect. '
-            'This should have a folder named ansible_collections inside of it.'
-        )
-    )
-    # Combine user requirements and collection requirements into single file
-    # in the future, could look into passing multilple files to
-    # python-builder scripts to be fed multiple files as opposed to this
-    introspect_parser.add_argument(
-        '--user-pip', dest='user_pip',
-        help='An additional file to combine with collection pip requirements.'
-    )
-    introspect_parser.add_argument(
-        '--user-bindep', dest='user_bindep',
-        help='An additional file to combine with collection bindep requirements.'
-    )
-    introspect_parser.add_argument(
-        '--write-pip', dest='write_pip',
-        help='Write the combined bindep file to this location.'
-    )
-    introspect_parser.add_argument(
-        '--write-bindep', dest='write_bindep',
-        help='Write the combined bindep file to this location.'
-    )
+    introspect_parser = create_introspect_parser(parser)
 
     for n in [create_command_parser, build_command_parser, introspect_parser]:
 
         n.add_argument('-v', '--verbosity',
                        dest='verbosity',
                        type=int,
                        choices=[0, 1, 2, 3],
```

### Comparing `ansible-builder-1.2.0/ansible_builder/constants.py` & `ansible-builder-3.0.0.0b1/ansible_builder/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,11 +27,16 @@
     default_container_runtime = 'docker'
 
 default_keyring_name = 'keyring.gpg'
 default_policy_file_name = 'policy.json'
 
 # Files that need to be moved into the build context, and their naming inside the context
 CONTEXT_FILES = {
+    # HACK: hacking in prototype other kinds of deps for dynamic builder
+    'python_interpreter': '',
+    'ansible_core': '',
+    'ansible_runner': '',
+
     'galaxy': 'requirements.yml',
     'python': 'requirements.txt',
     'system': 'bindep.txt',
 }
```

### Comparing `ansible-builder-1.2.0/ansible_builder/main.py` & `ansible-builder-3.0.0.0b1/ansible_builder/containerfile.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,242 +1,25 @@
+import importlib.resources
 import logging
 import os
 
+from pathlib import Path
+
 from . import constants
-from .policies import PolicyChoices, IgnoreAll, ExactReference
-from .steps import (
-    AdditionalBuildSteps, BuildContextSteps, GalaxyInstallSteps, GalaxyCopySteps, AnsibleConfigSteps
-)
 from .user_definition import UserDefinition
-from .utils import run_command, copy_file
+from .utils import copy_directory, copy_file
 
 
 logger = logging.getLogger(__name__)
 
 
-class AnsibleBuilder:
-    def __init__(self,
-                 action=None,
-                 filename=constants.default_file,
-                 build_args=None,
-                 build_context=constants.default_build_context,
-                 tag=None,
-                 container_runtime=constants.default_container_runtime,
-                 output_filename=None,
-                 no_cache=False,
-                 prune_images=False,
-                 verbosity=constants.default_verbosity,
-                 galaxy_keyring=None,
-                 galaxy_required_valid_signature_count=None,
-                 galaxy_ignore_signature_status_codes=(),
-                 container_policy=None,
-                 container_keyring=None,
-                 ):
-        """
-        :param str galaxy_keyring: GPG keyring file used by ansible-galaxy to opportunistically validate collection signatures.
-        :param str galaxy_required_valid_signature_count: Number of sigs (prepend + to disallow no sig( required for ansible-galaxy to accept collections.
-        :param str galaxy_ignore_signature_status_codes: GPG Status code to ignore when validating galaxy collections.
-        :param str container_policy: The container validation policy. A valid string value from the PolicyChoices enum.
-        """
-
-        if not galaxy_keyring and (galaxy_required_valid_signature_count or galaxy_ignore_signature_status_codes):
-            raise ValueError("--galaxy-required-valid-signature-count and --galaxy-ignore-signature-status-code may not be set without --galaxy-keyring")
-
-        self.action = action
-
-        # Read and validate the EE file early
-        self.definition = UserDefinition(filename=filename)
-        self.definition.validate()
-
-        self.tags = tag or []
-        self.build_context = build_context
-        self.build_outputs_dir = os.path.join(
-            build_context, constants.user_content_subfolder)
-        self.container_runtime = container_runtime
-        self.build_args = build_args or {}
-        self.no_cache = no_cache
-        self.prune_images = prune_images
-        self.containerfile = Containerfile(
-            definition=self.definition,
-            build_context=self.build_context,
-            container_runtime=self.container_runtime,
-            output_filename=output_filename,
-            galaxy_keyring=galaxy_keyring,
-            galaxy_required_valid_signature_count=galaxy_required_valid_signature_count,
-            galaxy_ignore_signature_status_codes=galaxy_ignore_signature_status_codes)
-        self.verbosity = verbosity
-        self.container_policy, self.container_keyring = self._handle_image_validation_opts(container_policy, container_keyring)
-
-    def _handle_image_validation_opts(self, policy, keyring):
-        """
-        Process the container_policy and container_keyring arguments.
-
-        :param str policy: The container_policy value.
-        :param str keyring: The container_keyring value.
-
-        The container_policy and container_keyring arguments come from the CLI
-        and work together to help build or use a podman policy.json file used
-        to do image validation. Depending on the policy being used, the keyring
-        may or may not be necessary.
-
-        The keyring, if required, must be a valid path, and will be transformed
-        to an absolute path to be used in the policy.json file.
-
-        :returns: A tuple of a PolicyChoices enum and abs path to the keyring.
-        """
-        resolved_policy = None
-        resolved_keyring = None
-
-        if policy is not None:
-            if self.version != "2":
-                raise ValueError(f'--container-policy not valid with version {self.version} format')
-
-            # Require podman runtime
-            if self.container_runtime != 'podman':
-                raise ValueError('--container-policy is only valid with the podman runtime')
-
-            resolved_policy = PolicyChoices(policy)
-
-            # Require keyring if we write a policy file
-            if resolved_policy == PolicyChoices.SIG_REQ and keyring is None:
-                raise ValueError(f'--container-policy={resolved_policy.value} requires --container-keyring')
-
-            # Do not allow images to be defined with --build-arg CLI option if
-            # any sig policy is defined.
-            for key, _ in self.build_args.items():
-                if key in ('EE_BASE_IMAGE', 'EE_BUILDER_IMAGE'):
-                    raise ValueError(f'{key} not allowed in --build-arg option with version 2 format')
-
-        if keyring is not None:
-            # Require the correct policy to be specified
-            if resolved_policy is None:
-                raise ValueError('--container-keyring requires --container-policy')
-            elif resolved_policy != PolicyChoices.SIG_REQ:
-                raise ValueError(f'--container-keyring is not valid with --container-policy={resolved_policy.value}')
-
-            # Set the keyring to an absolute path to be referenced in the policy file.
-            if not os.path.exists(keyring):
-                raise ValueError('--container-keyring error: file does not exist')
-            if not os.path.isfile(keyring):
-                raise ValueError('--container-keyring error: not a file')
-            resolved_keyring = os.path.abspath(keyring)
-
-        return (resolved_policy, resolved_keyring)
-
-    @property
-    def version(self):
-        return self.definition.version
-
-    @property
-    def ansible_config(self):
-        return self.definition.ansible_config
-
-    def create(self):
-        logger.debug('Ansible Builder is generating your execution environment build context.')
-        return self.write_containerfile()
-
-    def write_containerfile(self):
-        # File preparation
-        self.containerfile.create_folder_copy_files()
-
-        # First stage, galaxy
-        self.containerfile.prepare_galaxy_stage_steps()
-        self.containerfile.prepare_ansible_config_file()
-        self.containerfile.prepare_build_context()
-        self.containerfile.prepare_galaxy_install_steps()
-
-        # Second stage, builder
-        self.containerfile.prepare_build_stage_steps()
-        self.containerfile.prepare_galaxy_copy_steps()
-        self.containerfile.prepare_introspect_assemble_steps()
-
-        # Second stage
-        self.containerfile.prepare_final_stage_steps()
-        self.containerfile.prepare_prepended_steps()
-        self.containerfile.prepare_galaxy_copy_steps()
-        self.containerfile.prepare_system_runtime_deps_steps()
-        self.containerfile.prepare_appended_steps()
-        self.containerfile.prepare_label_steps()
-        logger.debug('Rewriting Containerfile to capture collection requirements')
-        return self.containerfile.write()
-
-    @property
-    def prune_image_command(self):
-        command = [
-            self.container_runtime, "image",
-            "prune", "--force"
-        ]
-        return command
-
-    @property
-    def build_command(self):
-        command = [
-            self.container_runtime, "build",
-            "-f", self.containerfile.path
-        ]
-
-        for tag in self.tags:
-            command.extend(["-t", tag])
-
-        for key, value in self.build_args.items():
-            if value:
-                build_arg = f"--build-arg={key}={value}"
-            else:
-                build_arg = f"--build-arg={key}"
-
-            command.append(build_arg)
-
-        if self.no_cache:
-            command.append('--no-cache')
-
-        if self.container_policy:
-            logger.debug('Container policy is %s', PolicyChoices(self.container_policy).value)
-
-            if self.container_policy == PolicyChoices.IGNORE:
-                policy = IgnoreAll()
-            elif self.container_policy == PolicyChoices.SIG_REQ:
-                logger.debug('Container validation keyring: %s', self.container_keyring)
-                policy = ExactReference(self.container_keyring)
-                if self.definition.base_image:
-                    policy.add_image(self.definition.base_image.name,
-                                     self.definition.base_image.signature_original_name)
-                if self.definition.builder_image:
-                    policy.add_image(self.definition.builder_image.name,
-                                     self.definition.builder_image.signature_original_name)
-
-            # SYSTEM is just a no-op for writing the policy file, but we still
-            # need to use the --pull-always option so that the system policy
-            # files work correctly if they require validating signatures.
-            if self.container_policy != PolicyChoices.SYSTEM:
-                policy_file_path = os.path.join(self.build_context, constants.default_policy_file_name)
-                logger.debug('Writing podman policy file %s', policy_file_path)
-                policy.write_policy(policy_file_path)
-                command.append(f'--signature-policy={policy_file_path}')
-
-            if self.container_policy != PolicyChoices.IGNORE:
-                command.append('--pull-always')
-
-        command.append(self.build_context)
-
-        return command
-
-    def build(self):
-        logger.debug('Ansible Builder is building your execution environment image. Tags: %s', ", ".join(self.tags))
-        self.write_containerfile()
-        run_command(self.build_command)
-        if self.prune_images:
-            logger.debug('Removing all dangling images')
-            run_command(self.prune_image_command)
-        return True
-
-
 class Containerfile:
     newline_char = '\n'
 
-    def __init__(self, definition,
+    def __init__(self, definition: UserDefinition,
                  build_context=None,
                  container_runtime=None,
                  output_filename=None,
                  galaxy_keyring=None,
                  galaxy_required_valid_signature_count=None,
                  galaxy_ignore_signature_status_codes=()):
         """
@@ -255,167 +38,359 @@
             filename = output_filename
         self.path = os.path.join(self.build_context, filename)
         self.container_runtime = container_runtime
         self.original_galaxy_keyring = galaxy_keyring
         self.copied_galaxy_keyring = None
         self.galaxy_required_valid_signature_count = galaxy_required_valid_signature_count
         self.galaxy_ignore_signature_status_codes = galaxy_ignore_signature_status_codes
+        self.steps: list = []
+
+    def prepare(self):
+        """
+        Prepares the steps for the run-time specific build file.
+
+        Incrementally builds the `self.steps` attribute by extending it with the
+        info to eventually be written directly to the container definition file
+        via a separate call to the `Containerfile.write()` method.
+        """
 
         # Build args all need to go at top of file to avoid errors
-        self.steps = [
-            "ARG EE_BASE_IMAGE={}".format(
-                self.definition.build_arg_defaults['EE_BASE_IMAGE']
-            ),
-            "ARG EE_BUILDER_IMAGE={}".format(
-                self.definition.build_arg_defaults['EE_BUILDER_IMAGE']
-            ),
-        ]
-
-    def create_folder_copy_files(self):
-        """Creates the build context file for this Containerfile
-        moves files from the definition into the folder
+        self._insert_global_args(include_values=True)
+
+        ######################################################################
+        # Zero stage: prep base image
+        ######################################################################
+
+        # 'base' (possibly customized) will be used by future build stages
+        self.steps.extend([
+            "# Base build stage",
+            "FROM $EE_BASE_IMAGE as base",
+            "USER root",
+        ])
+
+        self._insert_global_args()
+        self._insert_custom_steps('prepend_base')
+
+        if not self.definition.builder_image:
+            if self.definition.python_package_system:
+                self.steps.append('RUN $PKGMGR install $PYPKG -y && $PKGMGR clean all')
+
+            # We should always make sure pip is available for later stages.
+            self.steps.append('RUN $PYCMD -m ensurepip')
+
+            if self.definition.ansible_ref_install_list:
+                self.steps.append('RUN $PYCMD -m pip install --no-cache-dir $ANSIBLE_INSTALL_REFS')
+
+        self._create_folder_copy_files()
+        self._insert_custom_steps('append_base')
+
+        ######################################################################
+        # First stage (aka, galaxy): install roles/collections
+        #
+        # NOTE: This stage is skipped if there are no galaxy requirements.
+        ######################################################################
+
+        if self.definition.get_dep_abs_path('galaxy'):
+            self.steps.extend([
+                "",
+                "# Galaxy build stage",
+                "FROM base as galaxy",
+            ])
+
+            self._insert_global_args()
+            self._insert_custom_steps('prepend_galaxy')
+
+            # Run the check for the 'ansible-galaxy' executable. This will fail
+            # the build if the command is not found.
+            self.steps.append("RUN /output/scripts/check_galaxy")
+
+            self._prepare_ansible_config_file()
+            self._prepare_build_context()
+            self._prepare_galaxy_install_steps()
+            self._insert_custom_steps('append_galaxy')
+
+        ######################################################################
+        # Second stage (aka, builder): assemble (pip installs, bindep run)
+        ######################################################################
+
+        if self.definition.builder_image:
+            # Note: A builder image can be specified only in V1 or V2 schema.
+            image = "$EE_BUILDER_IMAGE"
+        else:
+            # dynamic builder, create from customized base
+            image = "base"
+
+        self.steps.extend([
+            "",
+            "# Builder build stage",
+            f"FROM {image} as builder",
+        ])
+
+        self._insert_global_args()
+
+        if image == "base":
+            self.steps.append("RUN $PYCMD -m pip install --no-cache-dir bindep pyyaml requirements-parser")
+
+        self._insert_custom_steps('prepend_builder')
+        self._prepare_galaxy_copy_steps()
+        self._prepare_introspect_assemble_steps()
+        self._insert_custom_steps('append_builder')
+
+        ######################################################################
+        # Final stage: package manager installs from bindep output
+        ######################################################################
+
+        self.steps.extend([
+            "",
+            "# Final build stage",
+            "FROM base as final",
+        ])
+
+        self._insert_global_args()
+        self._insert_custom_steps('prepend_final')
+
+        # Run the check for 'ansible' and 'ansible-runner' installations for
+        # any EE version 3 or above, unless explicitly skipped.
+        if self.definition.version >= 3 and not self.definition.options['skip_ansible_check']:
+            self.steps.append("RUN /output/scripts/check_ansible $PYCMD")
+
+        self._prepare_galaxy_copy_steps()
+        self._prepare_system_runtime_deps_steps()
+
+        # install init package if specified
+        # FUTURE: could move this into the pre-install wheel phase
+        if init_pip_pkg := self.definition.container_init.get('package_pip'):
+            self.steps.append(f"RUN $PYCMD -m pip install --no-cache-dir '{init_pip_pkg}'")
+
+        self._insert_custom_steps('append_final')
+        self._prepare_label_steps()
+        self._prepare_entrypoint_steps()
+
+    def write(self):
+        """
+        Writes the steps (built via the `Containerfile.prepare()` method) for
+        the runtime-specific build file (Dockerfile or Containerfile) to the
+        context directory.
+        """
+        with open(self.path, 'w') as f:
+            for step in self.steps:
+                f.write(step + self.newline_char)
+        return True
+
+    def _insert_global_args(self, include_values: bool = False):
+        """
+        Insert Containerfile ARGs and, possibly, their values.
+
+        An ARG with a None or empty value will not be included.
         """
-        os.makedirs(self.build_outputs_dir, exist_ok=True)
+
+        # ARGs will be output in the order listed below.
+        global_args = {
+            'EE_BASE_IMAGE': self.definition.build_arg_defaults['EE_BASE_IMAGE'],
+            'EE_BUILDER_IMAGE': self.definition.build_arg_defaults['EE_BUILDER_IMAGE'],
+            'PYCMD': self.definition.python_path or '/usr/bin/python3',
+            'PYPKG': self.definition.python_package_system,
+            'ANSIBLE_GALAXY_CLI_COLLECTION_OPTS': self.definition.build_arg_defaults['ANSIBLE_GALAXY_CLI_COLLECTION_OPTS'],
+            'ANSIBLE_GALAXY_CLI_ROLE_OPTS': self.definition.build_arg_defaults['ANSIBLE_GALAXY_CLI_ROLE_OPTS'],
+            'ANSIBLE_INSTALL_REFS': self.definition.ansible_ref_install_list,
+        }
+
+        if self.definition.version >= 3:
+            global_args['PKGMGR'] = self.definition.options['package_manager_path']
+
+        for arg, value in global_args.items():
+            if include_values and value:
+                # quote the value in case it includes spaces
+                self.steps.append(f'ARG {arg}="{value}"')
+            elif value:
+                self.steps.append(f"ARG {arg}")
+        self.steps.append("")
+
+    def _create_folder_copy_files(self):
+        """
+        Creates the build context directory, and copies any potential context
+        files (python, galaxy, or bindep requirements) into it.
+        """
+        scripts_dir = str(Path(self.build_outputs_dir) / 'scripts')
+        os.makedirs(scripts_dir, exist_ok=True)
 
         for item, new_name in constants.CONTEXT_FILES.items():
+            # HACK: new dynamic base/builder
+            if not new_name:
+                continue
+
             requirement_path = self.definition.get_dep_abs_path(item)
             if requirement_path is None:
                 continue
             dest = os.path.join(
                 self.build_context, constants.user_content_subfolder, new_name)
             copy_file(requirement_path, dest)
 
         if self.original_galaxy_keyring:
-            self.copied_galaxy_keyring = constants.default_keyring_name
-            copy_file(self.original_galaxy_keyring, os.path.join(self.build_outputs_dir, self.copied_galaxy_keyring))
+            copy_file(self.original_galaxy_keyring, os.path.join(self.build_outputs_dir, constants.default_keyring_name))
+
+        self._handle_additional_build_files()
 
         if self.definition.ansible_config:
             copy_file(
                 self.definition.ansible_config,
                 os.path.join(self.build_outputs_dir, 'ansible.cfg')
             )
 
-    def prepare_ansible_config_file(self):
+        # HACK: this sucks
+        scriptres = importlib.resources.files('ansible_builder._target_scripts')
+        for script in ('assemble', 'get-extras-packages', 'install-from-bindep', 'introspect.py', 'check_galaxy', 'check_ansible'):
+            with importlib.resources.as_file(scriptres / script) as script_path:
+                # FIXME: just use builtin copy?
+                copy_file(str(script_path), scripts_dir)
+
+        # later steps depend on base image containing these scripts
+        context_dir = Path(self.build_outputs_dir).stem
+        self.steps.append(f'COPY {context_dir}/scripts/ /output/scripts/')
+
+    def _handle_additional_build_files(self):
+        """
+        Deal with any files the user wants added to the image build context.
+
+        The 'src' value is either an absolute path, or a path relative to the
+        EE definition file. For example, 'src' can be a relative path like
+        "data_files/configs/*.cfg", but cannot be "/home/user/files/*.cfg",
+        the latter not being relative to the EE.
+        """
+        for entry in self.definition.additional_build_files:
+            src = Path(entry['src'])
+            dst = entry['dest']
+
+            # 'src' is either an absolute path or a path glob relative to the EE file
+            ee_file = Path(self.definition.filename)
+            if src.is_absolute():
+                if not src.exists():
+                    logger.warning(f"User build file {src} does not exist.")
+                    continue
+                src_files = [src]
+            elif not (src_files := list(ee_file.parent.glob(str(src)))):
+                logger.warning(f"No matches for '{src}' in additional_build_files.")
+                continue
+
+            final_dst = Path(self.build_outputs_dir) / dst
+            logger.debug(f"Creating {final_dst}")
+            final_dst.mkdir(parents=True, exist_ok=True)
+
+            for src_file in src_files:
+                if src_file.is_dir():
+                    copy_directory(src_file, final_dst)
+                else:
+                    # Destination is the subdir under context plus the basename of the source
+                    copy_location = final_dst / src_file.name
+                    copy_file(str(src_file), str(copy_location))
+
+    def _prepare_ansible_config_file(self):
+        if self.definition.version != 1:
+            return
+
         ansible_config_file_path = self.definition.ansible_config
         if ansible_config_file_path:
             context_file_path = os.path.join(
                 constants.user_content_subfolder, 'ansible.cfg')
-            return self.steps.extend(AnsibleConfigSteps(context_file_path))
-
-    def prepare_prepended_steps(self):
-        additional_prepend_steps = self.definition.get_additional_commands()
-        if additional_prepend_steps:
-            prepended_steps = additional_prepend_steps.get('prepend')
-            if prepended_steps:
-                return self.steps.extend(AdditionalBuildSteps(prepended_steps))
-
-        return False
-
-    def prepare_appended_steps(self):
-        additional_append_steps = self.definition.get_additional_commands()
-        if additional_append_steps:
-            appended_steps = additional_append_steps.get('append')
-            if appended_steps:
-                return self.steps.extend(AdditionalBuildSteps(appended_steps))
-
-        return False
+            self.steps.extend([
+                f"COPY {context_file_path} ~/.ansible.cfg",
+                "",
+            ])
+
+    def _insert_custom_steps(self, section: str):
+        additional_steps = self.definition.additional_build_steps
+        if additional_steps:
+            section_steps = additional_steps.get(section)
+            if section_steps:
+                if isinstance(section_steps, str):
+                    lines = section_steps.strip().splitlines()
+                else:
+                    lines = section_steps
+                self.steps.extend(lines)
 
-    def prepare_label_steps(self):
+    def _prepare_label_steps(self):
         self.steps.extend([
             "LABEL ansible-execution-environment=true",
         ])
 
-        return self.steps
-
-    def prepare_build_context(self):
+    def _prepare_build_context(self):
         if any(self.definition.get_dep_abs_path(thing) for thing in ('galaxy', 'system', 'python')):
-            self.steps.extend(BuildContextSteps())
-        return self.steps
+            self.steps.extend([
+                f"COPY {constants.user_content_subfolder} /build",
+                "WORKDIR /build",
+                "",
+            ])
+
+    def _prepare_galaxy_install_steps(self):
+        env = ""
+        install_opts = f"-r {constants.CONTEXT_FILES['galaxy']} --collections-path \"{constants.base_collections_path}\""
+
+        if self.galaxy_ignore_signature_status_codes:
+            for code in self.galaxy_ignore_signature_status_codes:
+                install_opts += f" --ignore-signature-status-code {code}"
 
-    def prepare_galaxy_install_steps(self):
-        if self.definition.get_dep_abs_path('galaxy'):
-            self.steps.extend(GalaxyInstallSteps(constants.CONTEXT_FILES['galaxy'],
-                                                 self.copied_galaxy_keyring,
-                                                 self.galaxy_ignore_signature_status_codes,
-                                                 self.galaxy_required_valid_signature_count))
-        return self.steps
+        if self.galaxy_required_valid_signature_count:
+            install_opts += f" --required-valid-signature-count {self.galaxy_required_valid_signature_count}"
+
+        if self.original_galaxy_keyring:
+            install_opts += f" --keyring \"{constants.default_keyring_name}\""
+        else:
+            # We have to use the environment variable to disable signature
+            # verification because older versions (<2.13) of ansible-galaxy do
+            # not support the --disable-gpg-verify option. We don't use ENV in
+            # the Containerfile since we need it only during the build and not
+            # in the final image.
+            env = "ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 "
+
+        self.steps.append(
+            f"RUN ansible-galaxy role install $ANSIBLE_GALAXY_CLI_ROLE_OPTS -r {constants.CONTEXT_FILES['galaxy']}"
+            f" --roles-path \"{constants.base_roles_path}\"",
+        )
+        self.steps.append(f"RUN {env}ansible-galaxy collection install $ANSIBLE_GALAXY_CLI_COLLECTION_OPTS {install_opts}")
 
-    def prepare_introspect_assemble_steps(self):
+    def _prepare_introspect_assemble_steps(self):
         # The introspect/assemble block is valid if there are any form of requirements
         if any(self.definition.get_dep_abs_path(thing) for thing in ('galaxy', 'system', 'python')):
 
-            introspect_cmd = "RUN ansible-builder introspect --sanitize"
+            introspect_cmd = "RUN $PYCMD /output/scripts/introspect.py introspect --sanitize"
 
             requirements_file_exists = os.path.exists(os.path.join(
                 self.build_outputs_dir, constants.CONTEXT_FILES['python']
             ))
+
             if requirements_file_exists:
                 relative_requirements_path = os.path.join(constants.user_content_subfolder, constants.CONTEXT_FILES['python'])
-                self.steps.append(f"ADD {relative_requirements_path} {constants.CONTEXT_FILES['python']}")
+                self.steps.append(f"COPY {relative_requirements_path} {constants.CONTEXT_FILES['python']}")
                 # WORKDIR is /build, so we use the (shorter) relative paths there
                 introspect_cmd += " --user-pip={0}".format(constants.CONTEXT_FILES['python'])
             bindep_exists = os.path.exists(os.path.join(self.build_outputs_dir, constants.CONTEXT_FILES['system']))
             if bindep_exists:
                 relative_bindep_path = os.path.join(constants.user_content_subfolder, constants.CONTEXT_FILES['system'])
-                self.steps.append(f"ADD {relative_bindep_path} {constants.CONTEXT_FILES['system']}")
+                self.steps.append(f"COPY {relative_bindep_path} {constants.CONTEXT_FILES['system']}")
                 introspect_cmd += " --user-bindep={0}".format(constants.CONTEXT_FILES['system'])
 
             introspect_cmd += " --write-bindep=/tmp/src/bindep.txt --write-pip=/tmp/src/requirements.txt"
 
             self.steps.append(introspect_cmd)
-            self.steps.append("RUN assemble")
+            self.steps.append("RUN /output/scripts/assemble")
 
-        return self.steps
-
-    def prepare_system_runtime_deps_steps(self):
+    def _prepare_system_runtime_deps_steps(self):
         self.steps.extend([
             "COPY --from=builder /output/ /output/",
-            "RUN /output/install-from-bindep && rm -rf /output/wheels",
-        ])
-
-        return self.steps
-
-    def prepare_galaxy_stage_steps(self):
-        self.steps.extend([
-            "",
-            "FROM $EE_BASE_IMAGE as galaxy",
-            "ARG ANSIBLE_GALAXY_CLI_COLLECTION_OPTS={}".format(
-                self.definition.build_arg_defaults['ANSIBLE_GALAXY_CLI_COLLECTION_OPTS']
-            ),
-            "ARG ANSIBLE_GALAXY_CLI_ROLE_OPTS={}".format(
-                self.definition.build_arg_defaults['ANSIBLE_GALAXY_CLI_ROLE_OPTS']
-            ),
-            "USER root",
-            ""
-        ])
-
-        return self.steps
-
-    def prepare_build_stage_steps(self):
-        self.steps.extend([
-            "",
-            "FROM $EE_BUILDER_IMAGE as builder"
-            "",
+            "RUN /output/scripts/install-from-bindep && rm -rf /output/wheels",
         ])
 
-        return self.steps
-
-    def prepare_final_stage_steps(self):
-        self.steps.extend([
-            "",
-            "FROM $EE_BASE_IMAGE",
-            "USER root"
-            "",
-        ])
-        return self.steps
-
-    def prepare_galaxy_copy_steps(self):
+    def _prepare_galaxy_copy_steps(self):
         if self.definition.get_dep_abs_path('galaxy'):
-            self.steps.extend(GalaxyCopySteps())
-        return self.steps
-
-    def write(self):
-        with open(self.path, 'w') as f:
-            for step in self.steps:
-                f.write(step + self.newline_char)
-
-        return True
+            self.steps.extend([
+                "",
+                "COPY --from=galaxy {0} {0}".format(
+                    os.path.dirname(constants.base_collections_path.rstrip('/'))  # /usr/share/ansible
+                ),
+                "",
+            ])
+
+    def _prepare_entrypoint_steps(self):
+        if ep := self.definition.container_init.get('entrypoint'):
+            self.steps.append(f"ENTRYPOINT {ep}")
+        if cmd := self.definition.container_init.get('cmd'):
+            self.steps.append(f"CMD {cmd}")
```

### Comparing `ansible-builder-1.2.0/ansible_builder/policies.py` & `ansible-builder-3.0.0.0b1/ansible_builder/policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/ansible_builder/requirements.py` & `ansible-builder-3.0.0.0b1/ansible_builder/requirements.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/ansible_builder/user_definition.py` & `ansible-builder-3.0.0.0b1/ansible_builder/user_definition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import os
 import textwrap
+import tempfile
 import yaml
 
+from pathlib import Path
+from typing import Callable
+
 from . import constants
 from .exceptions import DefinitionError
+from .ee_schema import validate_schema
 
 
-ALLOWED_KEYS_V1 = [
-    'version',
-    'build_arg_defaults',
-    'dependencies',
-    'ansible_config',
-    'additional_build_steps',
-]
-
-ALLOWED_KEYS_V2 = [
-    'images',
-]
+# HACK: manage lifetimes more carefully
+_tempfiles: list[Callable] = []
 
 
 class ImageDescription:
     """
     Class to describe a container image from the EE file.
 
     For the currently supported 'exactReference' type, this class is dead
@@ -93,190 +89,151 @@
 
         if not isinstance(self.raw, dict):
             raise DefinitionError(f"Definition must be a dictionary, not {type(self.raw).__name__}")
 
         # Set default values for the build arguments. User supplied values
         # are set later during validation.
         self.build_arg_defaults = constants.build_arg_defaults.copy()
+        if self.version > 2:
+            # v3 and higher no longer supports a builder image so make
+            # sure this value is cleared of the default value.
+            self.build_arg_defaults['EE_BUILDER_IMAGE'] = None
 
         # Attributes used for creating podman container policies. These will be None
         # if no 'images' section is present in the EE, or an ImageDescription object otherwise.
         self.base_image = None
         self.builder_image = None
 
     @property
     def version(self):
         """
-        Version of the EE file.
+        Integer version of the EE file.
 
         If no version is specified, assume version 1 (for backward compat).
         """
         version = self.raw.get('version', 1)
-        return str(version)
+        return version
 
     @property
     def ansible_config(self):
         """ Path to the user specified ansible.cfg file """
         ansible_config = self.raw.get('ansible_config')
         if not ansible_config:
             return None
         return str(ansible_config)
 
-    def get_additional_commands(self):
+    @property
+    def additional_build_steps(self):
         """Gets additional commands from the exec env file, if any are specified.
         """
-        commands = self.raw.get('additional_build_steps')
-        return commands
+        return self.raw.get('additional_build_steps')
+
+    @property
+    def python_package_system(self):
+        return self.raw.get('dependencies', {}).get('python_interpreter', {}).get('package_system', None)
+
+    @property
+    def python_path(self):
+        return self.raw.get('dependencies', {}).get('python_interpreter', {}).get('python_path', None)
+
+    @property
+    def ansible_core_ref(self):
+        return self.raw.get('dependencies', {}).get('ansible_core', {}).get('package_pip', None)
+
+    @property
+    def ansible_runner_ref(self):
+        return self.raw.get('dependencies', {}).get('ansible_runner', {}).get('package_pip', None)
+
+    @property
+    def ansible_ref_install_list(self):
+        return ' '.join([r for r in (self.ansible_core_ref, self.ansible_runner_ref) if r]) or None
+
+    @property
+    def additional_build_files(self):
+        return self.raw.get('additional_build_files', [])
+
+    @property
+    def container_init(self):
+        return self.raw.get('options', {}).get('container_init', {})
+
+    @property
+    def options(self):
+        return self.raw.get('options', {})
 
     def get_dep_abs_path(self, entry):
         """Unique to the user EE definition, files can be referenced by either
         an absolute path or a path relative to the EE definition folder
         This method will return the absolute path.
         """
         req_file = self.raw.get('dependencies', {}).get(entry)
 
         if not req_file:
             return None
 
+        # HACK: jamming in prototype support for inline deps listing, tempfile handling is ass
+        if (is_list := isinstance(req_file, list)) or (isinstance(req_file, str) and '\n' in req_file):
+            tf = tempfile.NamedTemporaryFile('w')
+            if is_list:
+                tf.write('\n'.join(req_file))
+            else:
+                tf.write(req_file)
+            _tempfiles.append(tf)
+            tf.flush()  # don't close, it'll clean up on GC
+            req_file = tf.name
+        if not isinstance(req_file, str):
+            return None
+
         if os.path.isabs(req_file):
             return req_file
 
         return os.path.join(self.reference_path, req_file)
 
-    def _validate_root_keys(self):
-        """
-        Identify any invalid top-level keys in the execution environment file.
-
-        :raises: DefinitionError exception if any invalid keys are identified.
+    def _validate_additional_build_files(self):
         """
-        def_file_dict = self.raw
-        yaml_keys = set(def_file_dict.keys())
+        Check that entries in additional_build_files look correct.
 
-        valid_keys = set(ALLOWED_KEYS_V1)
-        if self.version == '2':
-            valid_keys = valid_keys.union(set(ALLOWED_KEYS_V2))
-
-        invalid_keys = yaml_keys - valid_keys
-
-        if invalid_keys:
-            raise DefinitionError(textwrap.dedent(
-                f"""
-                Error: Unknown yaml key(s), {invalid_keys}, found in the definition file.\n
-                Allowed options are:
-                {valid_keys}
-                """)
-            )
-
-    def _validate_v2(self):
-        """
-        Validate all execution environment file, version 2, keys.
+        The 'dest' values are checked for the correct format. Since 'src' can
+        be a file glob or an absolute or relative path, it is not checked.
 
         :raises: DefinitionError exception if any errors are found.
         """
+        for entry in self.additional_build_files:
+            dest = Path(entry['dest'])
+            if dest.is_absolute() or '..' in dest.parts:
+                raise DefinitionError(f"'dest' must not be an absolute path or contain '..': {dest}")
 
-        if self.version == "1":
-            return
-
-        images = self.raw.get('images', {})
-
-        # The base and builder images MUST be defined in the 'images' section only.
-        bad = self.raw.get('build_arg_defaults')
-        if bad:
-            if 'EE_BASE_IMAGE' in bad or 'EE_BUILDER_IMAGE' in bad:
-                raise DefinitionError("Error: Version 2 does not allow defining EE_BASE_IMAGE or EE_BUILDER_IMAGE in 'build_arg_defaults'")
-
-        if images:
-            self.base_image = ImageDescription(images, 'base_image')
-            self.builder_image = ImageDescription(images, 'builder_image')
-
-            # Must set these values so that Containerfile uses the proper images
-            self.build_arg_defaults['EE_BASE_IMAGE'] = self.base_image.name
-            self.build_arg_defaults['EE_BUILDER_IMAGE'] = self.builder_image.name
-
-    def _validate_v1(self):
+    def validate(self):
         """
-        Validate all execution environment file, version 1, keys.
+        Check that all specified keys in the definition file are valid.
 
         :raises: DefinitionError exception if any errors are found.
         """
-
-        if self.raw.get('dependencies') is not None:
-            if not isinstance(self.raw.get('dependencies'), dict):
-                raise DefinitionError(textwrap.dedent(
-                    f"""
-                    Error: Unknown type {type(self.raw.get('dependencies'))} found for dependencies, must be a dict.\n
-                    Allowed options are:
-                    {list(constants.CONTEXT_FILES.keys())}
-                    """)
-                )
-
-            dependencies_keys = set(self.raw.get('dependencies'))
-            invalid_dependencies_keys = dependencies_keys - set(constants.CONTEXT_FILES.keys())
-            if invalid_dependencies_keys:
-                raise DefinitionError(textwrap.dedent(
-                    f"""
-                    Error: Unknown yaml key(s), {invalid_dependencies_keys}, found in dependencies.\n
-                    Allowed options are:
-                    {list(constants.CONTEXT_FILES.keys())}
-                    """)
-                )
+        validate_schema(self.raw)
 
         for item in constants.CONTEXT_FILES:
+            # HACK: non-file deps for dynamic base/builder
+            if not constants.CONTEXT_FILES[item]:
+                continue
             requirement_path = self.get_dep_abs_path(item)
             if requirement_path:
                 if not os.path.exists(requirement_path):
                     raise DefinitionError(f"Dependency file {requirement_path} does not exist.")
 
         # Validate and set any user-specified build arguments
         build_arg_defaults = self.raw.get('build_arg_defaults')
         if build_arg_defaults:
-            if not isinstance(build_arg_defaults, dict):
-                raise DefinitionError(
-                    f"Error: Unknown type {type(build_arg_defaults)} found for build_arg_defaults; "
-                    f"must be a dict."
-                )
-            unexpected_keys = set(build_arg_defaults) - set(constants.build_arg_defaults)
-            if unexpected_keys:
-                raise DefinitionError(
-                    f"Keys {unexpected_keys} are not allowed in 'build_arg_defaults'."
-                )
             for key, user_value in build_arg_defaults.items():
-                if user_value and not isinstance(user_value, str):
-                    raise DefinitionError(
-                        f"Expected build_arg_defaults.{key} to be a string; "
-                        f"Found a {type(user_value)} instead."
-                    )
                 self.build_arg_defaults[key] = user_value
 
-        additional_cmds = self.get_additional_commands()
-        if additional_cmds:
-            if not isinstance(additional_cmds, dict):
-                raise DefinitionError(textwrap.dedent("""
-                    Expected 'additional_build_steps' in the provided definition file to be a dictionary
-                    with keys 'prepend' and/or 'append'; found a {0} instead.
-                    """).format(type(additional_cmds).__name__))
-
-            expected_keys = frozenset(('append', 'prepend'))
-            unexpected_keys = set(additional_cmds) - expected_keys
-            if unexpected_keys:
-                raise DefinitionError(
-                    f"Keys {*unexpected_keys,} are not allowed in 'additional_build_steps'."
-                )
-
-        ansible_config_path = self.raw.get('ansible_config')
-        if ansible_config_path:
-            if not isinstance(ansible_config_path, str):
-                raise DefinitionError(textwrap.dedent(f"""
-                    Expected 'ansible_config' in the provided definition file to
-                    be a string; found a {type(ansible_config_path).__name__} instead.
-                    """))
-
-    def validate(self):
-        """
-        Check that all specified keys in the definition file are valid.
-
-        :raises: DefinitionError exception if any errors are found.
-        """
+        if self.version > 1:
+            images = self.raw.get('images', {})
+            if images:
+                self.base_image = ImageDescription(images, 'base_image')
+
+                # Must set these values so that Containerfile uses the proper images
+                if self.base_image.name:
+                    self.build_arg_defaults['EE_BASE_IMAGE'] = self.base_image.name
+                if 'builder_image' in images:
+                    self.builder_image = ImageDescription(images, 'builder_image')
+                    self.build_arg_defaults['EE_BUILDER_IMAGE'] = self.builder_image.name
 
-        self._validate_root_keys()
-        self._validate_v1()
-        self._validate_v2()
+            self._validate_additional_build_files()
```

### Comparing `ansible-builder-1.2.0/ansible_builder/utils.py` & `ansible-builder-3.0.0.0b1/ansible_builder/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import filecmp
 import logging
 import logging.config
 import os
 import shutil
 import subprocess
 import sys
+
 from collections import deque
+from pathlib import Path
 
 from .colors import MessageColors
 from . import constants
 
 
 logger = logging.getLogger(__name__)
 logging_levels = {
@@ -110,15 +112,15 @@
                 logger.error('')
             else:
                 if len(trailing_output) == 20:
                     logger.error('...showing last 20 lines of output...')
                 for line in trailing_output:
                     logger.error(line)
                 logger.error('')
-        logger.error("An error occured (rc=%s), see output line(s) above for details.", rc)
+        logger.error("An error occurred (rc=%s), see output line(s) above for details.", rc)
         sys.exit(1)
 
     return (rc, output)
 
 
 def write_file(filename: str, lines: list) -> bool:
     parent_dir = os.path.dirname(filename)
@@ -134,14 +136,37 @@
             else:
                 logger.warning('File %s had modifications and will be rewritten', filename)
     with open(filename, 'w') as f:
         f.write(new_text)
     return True
 
 
+def copy_directory(source_dir: Path, dest: Path):
+    """
+    Recursively copy a source directory to a path in the context directory.
+
+    In order to not corrupt the build context cache, if it should exist, we
+    attempt to copy files within the source directory to the context directory
+    if necessary by utilizing copy_file() on each file, rather than a blind
+    recursive copy.
+    """
+
+    if not source_dir.is_dir():
+        raise Exception(f"Expected a directory at '{source_dir}'")
+
+    for child in source_dir.iterdir():
+        copy_location = dest / child.name
+        if child.is_dir():
+            # a subdir of our build destination directory
+            copy_location.mkdir(exist_ok=True)
+            copy_directory(child, copy_location)
+        else:
+            copy_file(str(child), str(copy_location))
+
+
 def copy_file(source: str, dest: str) -> bool:
     should_copy = False
 
     if os.path.abspath(source) == os.path.abspath(dest):
         logger.info("File %s was placed in build context by user, leaving unmodified.", dest)
         return False
     elif not os.path.exists(dest):
```

### Comparing `ansible-builder-1.2.0/ansible_builder.egg-info/SOURCES.txt` & `ansible-builder-3.0.0.0b1/ansible_builder.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -27,41 +27,46 @@
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/documentation_report.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
 .github/test-scripts/setup_pulp.sh
 .github/workflows/ci.yml
 .github/workflows/triage_existing.yml
 .github/workflows/triage_new.yml
-.zuul.d/jobs.yaml
-.zuul.d/project.yaml
-.zuul.d/playbooks/.zuul.ignore
-.zuul.d/playbooks/ansible-builder-build-container-image/pre.yaml
 ansible_builder/__init__.py
+ansible_builder/__main__.py
 ansible_builder/cli.py
 ansible_builder/colors.py
 ansible_builder/constants.py
+ansible_builder/containerfile.py
+ansible_builder/ee_schema.py
 ansible_builder/exceptions.py
-ansible_builder/introspect.py
 ansible_builder/main.py
 ansible_builder/policies.py
 ansible_builder/requirements.py
-ansible_builder/steps.py
 ansible_builder/user_definition.py
 ansible_builder/utils.py
 ansible_builder.egg-info/PKG-INFO
 ansible_builder.egg-info/SOURCES.txt
 ansible_builder.egg-info/dependency_links.txt
 ansible_builder.egg-info/entry_points.txt
 ansible_builder.egg-info/not-zip-safe
 ansible_builder.egg-info/pbr.json
 ansible_builder.egg-info/requires.txt
 ansible_builder.egg-info/top_level.txt
+ansible_builder/_target_scripts/__init__.py
+ansible_builder/_target_scripts/assemble
+ansible_builder/_target_scripts/check_ansible
+ansible_builder/_target_scripts/check_galaxy
+ansible_builder/_target_scripts/get-extras-packages
+ansible_builder/_target_scripts/install-from-bindep
+ansible_builder/_target_scripts/introspect.py
 demo/execution-environment.yml
 demo/requirements.txt
 demo/requirements.yml
+demo/v3_demo/execution-environment.yml
 docs/Makefile
 docs/collection_metadata.rst
 docs/conf.py
 docs/definition.rst
 docs/glossary.rst
 docs/index.rst
 docs/installation.rst
@@ -75,22 +80,22 @@
 packaging/rpm/Dockerfile.epel-8-x86_64
 packaging/rpm/ansible-builder.spec.j2
 packaging/rpm/docker-compose.yml
 test/__init__.py
 test/conftest.py
 test/requirements.txt
 test/data/README.md
-test/data/ansible-test.cfg
-test/data/nested-galaxy.yml
 test/data/run.sh
 test/data/ansible.posix.at/execution-environment.yml
 test/data/ansible.posix.at/requirements.yml
 test/data/ansible.posix.at/run.sh
 test/data/ansible.posix.at/env/settings
 test/data/ansible.posix.at/project/ansible.posix.at.yml
+test/data/ansible_cfg_for_galaxy/ansible-test.cfg
+test/data/ansible_cfg_for_galaxy/requirements.yml
 test/data/ansible_collections/other/reqfile/requirements.txt
 test/data/ansible_collections/test/bindep/MANIFEST.json
 test/data/ansible_collections/test/bindep/bindep.txt
 test/data/ansible_collections/test/metadata/MANIFEST.json
 test/data/ansible_collections/test/metadata/my-requirements.txt
 test/data/ansible_collections/test/metadata/meta/execution-environment.yml
 test/data/ansible_collections/test/reqfile/MANIFEST.json
@@ -103,17 +108,18 @@
 test/data/build_args/base-image.yml
 test/data/build_args/execution-environment.yml
 test/data/build_fail/execution-environment.yml
 test/data/definition_files/bad.yml
 test/data/definition_files/invalid.yml
 test/data/definition_files/no_galaxy.yml
 test/data/definition_files/no_python.yml
-test/data/foo/requirements.yml
 test/data/needs_git/execution-environment.yml
 test/data/needs_git/requirements.txt
+test/data/nested_galaxy_file/nested-galaxy.yml
+test/data/nested_galaxy_file/foo/requirements.yml
 test/data/pip/execution-environment.yml
 test/data/pip/run.sh
 test/data/pip/env/settings
 test/data/pip/project/pip.yml
 test/data/pip/project/requirements.txt
 test/data/prepend_steps/execution-environment.yml
 test/data/pytz/execution-environment.yml
@@ -126,22 +132,32 @@
 test/data/subversion/run.sh
 test/data/subversion/env/settings
 test/data/subversion/project/subversion.yml
 test/data/v2/RPM-GPG-KEY-redhat-release
 test/data/v2/invalid-keyring
 test/data/v2/sig_req/ee-good.yml
 test/data/v2/sig_req/ee-no-orig.yml
+test/data/v3/check_ansible/ee-missing-ansible.yml
+test/data/v3/check_ansible/ee-missing-runner.yml
+test/data/v3/check_ansible/ee-skip.yml
+test/data/v3/complete/ee.yml
+test/data/v3/complete/files/random.cfg
+test/data/v3/complete/files/data/a.dat
+test/data/v3/complete/files/data/text_files/a.txt
+test/data/v3/pre_and_post/ee.yml
+test/data/v3/pre_and_post/requirements.yml
 test/integration/conftest.py
 test/integration/test_build.py
 test/integration/test_create.py
 test/integration/test_help.py
 test/integration/test_introspect_cli.py
 test/pulp_integration/test_policies.py
+test/pulp_integration/test_v3.py
 test/unit/__init__.py
 test/unit/test_cli.py
+test/unit/test_containerfile.py
 test/unit/test_introspect.py
 test/unit/test_main.py
 test/unit/test_policies.py
 test/unit/test_requirements.py
-test/unit/test_steps.py
 test/unit/test_user_definition.py
 test/unit/test_utils.py
```

### Comparing `ansible-builder-1.2.0/docs/Makefile` & `ansible-builder-3.0.0.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/docs/collection_metadata.rst` & `ansible-builder-3.0.0.0b1/docs/collection_metadata.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/docs/conf.py` & `ansible-builder-3.0.0.0b1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autosectionlabel',
+    "sphinx_ansible_theme",
     'pbr.sphinxext',
 ]
 
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
@@ -65,15 +66,15 @@
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -84,21 +85,26 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_ansible_theme'
+html_title = "Ansible Builder Documentation"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
-# html_theme_options = {}
+html_theme_options = {
+    'display_version': False,
+    'titles_only': False,
+    'documentation_home_url': 'https://ansible-builder.readthedocs.io/en/latest/',
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
```

### Comparing `ansible-builder-1.2.0/docs/glossary.rst` & `ansible-builder-3.0.0.0b1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/docs/index.rst` & `ansible-builder-3.0.0.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/docs/installation.rst` & `ansible-builder-3.0.0.0b1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/docs/make.bat` & `ansible-builder-3.0.0.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/docs/usage.rst` & `ansible-builder-3.0.0.0b1/docs/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -211,14 +211,32 @@
 
 .. note::
 
    This flag essentially removes all the dangling images on the given machine whether they
    already exists or created by ansible-builder build process.
 
 
+``--squash``
+************
+
+This option controls the final image layer squashing. Valid values are:
+
+* ``new``: Squash all of the final image's new layers into a single new layer
+  (preexisting layers are not squashed). This is the default.
+* ``all``: Squash all of the final image's layers, including those inherited
+  from the base image, into a single new layer.
+* ``off``: Turn off layer squashing.
+
+.. note::
+
+   This flag is compatible only with the ``podman`` runtime and will be ignored
+   for any other runtime. Docker is not supported since layer image squashing is
+   considered an experimental feature.
+
+
 The ``create`` command
 ----------------------
 
 The ``ansible-builder create`` command works similarly to the ``build`` command
 in that it takes an execution environment definition as an input
 and outputs the build context necessary for building an execution environment
 image. However, the ``create`` command *will not* build the execution environment
```

### Comparing `ansible-builder-1.2.0/packaging/rpm/ansible-builder.spec.j2` & `ansible-builder-3.0.0.0b1/packaging/rpm/ansible-builder.spec.j2`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/conftest.py` & `ansible-builder-3.0.0.0b1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/data/README.md` & `ansible-builder-3.0.0.0b1/test/data/README.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/data/ansible.posix.at/project/ansible.posix.at.yml` & `ansible-builder-3.0.0.0b1/test/data/ansible.posix.at/project/ansible.posix.at.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/data/run.sh` & `ansible-builder-3.0.0.0b1/test/data/run.sh`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/data/v2/RPM-GPG-KEY-redhat-release` & `ansible-builder-3.0.0.0b1/test/data/v2/RPM-GPG-KEY-redhat-release`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/integration/test_build.py` & `ansible-builder-3.0.0.0b1/test/integration/test_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,66 +26,66 @@
 
 @pytest.mark.test_all_runtimes
 def test_blank_execution_environment(cli, runtime, ee_tag, tmp_path, data_dir):
     """Just makes sure that the build process does not require any particular input"""
     bc = tmp_path
     ee_def = data_dir / 'blank' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     )
     result = cli(f'{runtime} run --rm {ee_tag} echo "This is a simple test"')
     assert 'This is a simple test' in result.stdout, result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_multiple_tags(cli, runtime, ee_tag, tmp_path, data_dir):
     """Make sure multiple tagging works"""
     bc = tmp_path
     ee_def = data_dir / 'blank' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} -t testmultitags --container-runtime {runtime}'
+        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} -t testmultitags --container-runtime {runtime}'
     )
     result = cli(f'{runtime} run --rm {ee_tag} echo "test: test_multiple_tags 1"')
     assert 'test: test_multiple_tags 1' in result.stdout, result.stdout
 
     result = cli(f'{runtime} run --rm testmultitags echo "test: test_multiple_tags 2"')
     assert 'test: test_multiple_tags 2' in result.stdout, result.stdout
     delete_image(runtime, 'testmultitags')
 
 
 @pytest.mark.test_all_runtimes
 def test_user_system_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'subversion' / 'execution-environment.yml'
-    command = f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+    command = f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     cli(command)
     result = cli(
         f'{runtime} run --rm {ee_tag} svn --help'
     )
     assert 'Subversion is a tool for version control' in result.stdout, result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_collection_system_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v3'
+        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v3'
     )
     result = cli(
         f'{runtime} run --rm {ee_tag} at -V'
     )
     assert 'at version' in result.stderr, result.stderr
 
 
 @pytest.mark.test_all_runtimes
 def test_user_python_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'pip' / 'execution-environment.yml'
-    command = f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+    command = f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     cli(command)
     result = cli(
         f'{runtime} run --rm {ee_tag} pip3 show awxkit'
     )
     assert 'The official command line interface for Ansible AWX' in result.stdout, result.stdout
     for py_library in ('requirements-parser'):
         result = cli(
@@ -94,29 +94,29 @@
         assert result.rc != 0, py_library
 
 
 @pytest.mark.test_all_runtimes
 def test_python_git_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'needs_git' / 'execution-environment.yml'
-    command = f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+    command = f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     cli(command)
     result = cli(f'{runtime} run --rm {ee_tag} pip3 freeze')
     assert 'flask' in result.stdout.lower(), result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_prepended_steps(cli, runtime, ee_tag, tmp_path, data_dir):
     """
     Tests that prepended steps are in final stage
     """
     bc = tmp_path
     ee_def = data_dir / 'prepend_steps' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     )
 
     _file = 'Dockerfile' if runtime == 'docker' else 'Containerfile'
     content = open(os.path.join(bc, _file), 'r').read()
 
     stages_content = content.split('FROM')
 
@@ -124,52 +124,53 @@
 
 
 @pytest.mark.test_all_runtimes
 def test_build_args_basic(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'build_args' / 'execution-environment.yml'
     result = cli(
-        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO=bar -v3'
+        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO=bar -v3'
     )
     assert 'FOO=bar' in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_build_args_from_environment(cli, runtime, ee_tag, tmp_path, data_dir):
     if runtime == 'podman':
         pytest.skip('Skipped. Podman does not support this')
 
     bc = tmp_path
     ee_def = data_dir / 'build_args' / 'execution-environment.yml'
     os.environ['FOO'] = 'secretsecret'
     result = cli(
-        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO -v3'
+        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO -v3'
     )
     assert 'secretsecret' in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_base_image_build_arg(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'build_args' / 'base-image.yml'
     os.environ['FOO'] = 'secretsecret'
 
     # Build with custom image tag, then use that as input to --build-arg EE_BASE_IMAGE
-    cli(f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag}-custom --container-runtime {runtime} -v3')
-    cli(f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag}-custom '
+    cli(f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag}-custom --container-runtime {runtime} -v3')
+    cli(f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag}-custom '
         f'--container-runtime {runtime} --build-arg EE_BASE_IMAGE={ee_tag}-custom -v3')
-    result = cli(f"{runtime} run {ee_tag}-custom cat /base_image")
+
+    result = cli(f"{runtime} run --rm {ee_tag}-custom cat /base_image")
     assert f"{ee_tag}-custom" in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 @pytest.mark.xfail(reason='Unreliable on podman')
 def test_has_pytz(cli, runtime, data_dir, ee_tag, tmp_path):
     ee_def = data_dir / 'pytz' / 'execution-environment.yml'
-    cli(f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
+    cli(f'ansible-builder build --no-cache -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
     result = cli(f'{runtime} run --rm {ee_tag} pip3 show pytz')
 
     assert 'World timezone definitions, modern and historical' in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 @pytest.mark.xfail(reason='Unreliable on podman')
@@ -193,48 +194,49 @@
 
 @pytest.mark.test_all_runtimes
 def test_collection_verification_off(cli, runtime, data_dir, ee_tag, tmp_path):
     """
     Test that, by default, collection verification is off via the env var.
     """
     ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
-    result = cli(f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
+    result = cli(f'ansible-builder build --no-cache -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
     assert "RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy" in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_collection_verification_on(cli, runtime, data_dir, ee_tag, tmp_path):
     """
     Test that collection verification is on when given a keyring.
     """
     keyring = tmp_path / "mykeyring.gpg"
     keyring.touch()
     ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
 
     # ansible-galaxy might error (older Ansible), but that should be ok
-    result = cli(f'ansible-builder build --galaxy-keyring {keyring} -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3', allow_error=True)
+    result = cli(f'ansible-builder build --no-cache --galaxy-keyring {keyring} -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3',
+                 allow_error=True)
 
     keyring_copy = tmp_path / constants.user_content_subfolder / constants.default_keyring_name
     assert keyring_copy.exists()
 
     assert "RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy" not in result.stdout
     assert f"--keyring \"{constants.default_keyring_name}\"" in result.stdout
 
 
 @pytest.mark.xfail(reason="Needs ansible 2.13")
 @pytest.mark.test_all_runtimes
 def test_galaxy_signing_extra_args(cli, runtime, data_dir, ee_tag, tmp_path):
     """
-    Test that all extr asigning args for gpg are passed into the container file.
+    Test that all extra signing args for gpg are passed into the container file.
     """
     pytest.xfail("failing configuration (but should work)")
 
     keyring = tmp_path / "mykeyring.gpg"
     keyring.touch()
     ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
 
-    result = cli(f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3 '
+    result = cli(f'ansible-builder build --no-cache -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3 '
                  f'--galaxy-keyring {keyring} --galaxy-ignore-signature-status-code 500 '
                  f'--galaxy-required-valid-signature-count 3', allow_error=True)
 
     assert "--galaxy-ignore-signature-status-code 500" in result.stdout
     assert "--galaxy-required-valid-signature-count 3" in result.stdout
```

### Comparing `ansible-builder-1.2.0/test/integration/test_create.py` & `ansible-builder-3.0.0.0b1/test/unit/test_containerfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,110 @@
-import os
-
 from ansible_builder import constants
+from ansible_builder.containerfile import Containerfile
+from ansible_builder.user_definition import UserDefinition
+
+
+def make_containerfile(tmpdir, ee_path, **cf_kwargs):
+    definition = UserDefinition(ee_path)
+    build_context = str(tmpdir / '_build')
+    c = Containerfile(definition, build_context=build_context, container_runtime='podman', **cf_kwargs)
+    return c
+
+
+def test_insert_custom_steps_list(build_dir_and_ee_yml):
+    ee_data = [
+        'additional_build_steps:',
+        '  prepend:',
+        '    - RUN echo This is the custom steps list test',
+        '    - RUN whoami',
+    ]
+
+    tmpdir, ee_path = build_dir_and_ee_yml("\n".join(ee_data))
+    c = make_containerfile(tmpdir, ee_path)
+    c._insert_custom_steps("prepend")
+    assert c.steps == ['RUN echo This is the custom steps list test', 'RUN whoami']
+
+
+def test_insert_custom_steps_string(build_dir_and_ee_yml):
+    ee_data = [
+        'additional_build_steps:',
+        '  append: |',
+        '    RUN echo This is the custom steps string test',
+        '    RUN whoami',
+    ]
+
+    tmpdir, ee_path = build_dir_and_ee_yml("\n".join(ee_data))
+    c = make_containerfile(tmpdir, ee_path)
+    c._insert_custom_steps("append")
+    assert c.steps == ['RUN echo This is the custom steps string test', 'RUN whoami']
 
 
-def test_definition_syntax_error(cli, data_dir):
-    ee_def = os.path.join(data_dir, 'definition_files', 'invalid.yml')
-    r = cli(f'ansible-builder create -f {ee_def}', allow_error=True)
-    assert r.rc != 0
-    assert 'An error occurred while parsing the definition file' in (r.stdout + r.stderr), (r.stdout + r.stderr)
-
-
-def test_missing_python_requirements_file(cli, data_dir):
-    """If a user specifies a python requirements file, but we can't find it, fail sanely."""
-    ee_def = os.path.join(data_dir, 'definition_files', 'no_python.yml')
-    r = cli(f'ansible-builder create -f {ee_def}', allow_error=True)
-    assert r.rc != 0
-    assert 'does not exist' in (r.stdout + r.stderr), (r.stdout + r.stderr)
-
-
-def test_missing_galaxy_requirements_file(cli, data_dir):
-    """If a user specifies a galaxy requirements file, but we can't find it, fail sanely."""
-    ee_def = os.path.join(data_dir, 'definition_files', 'no_galaxy.yml')
-    r = cli(f'ansible-builder create -f {ee_def}', allow_error=True)
-    assert r.rc != 0
-    assert 'does not exist' in (r.stdout + r.stderr), (r.stdout + r.stderr)
-
-
-def test_create_streams_output_with_verbosity_on(cli, build_dir_and_ee_yml):
-    """Test that 'ansible-builder build' streams build output."""
-    tmpdir, eeyml = build_dir_and_ee_yml("")
-    result = cli(f"ansible-builder create -c {tmpdir} -f {eeyml} -v 3")
-    assert 'Ansible Builder is generating your execution environment build context.' in result.stdout
-    assert f'The build context can be found at: {tmpdir}' in result.stdout
-
-
-def test_create_streams_output_with_verbosity_off(cli, build_dir_and_ee_yml):
-    """
-    Like the test_create_streams_output_with_verbosity_on test but making sure less output is shown with default verbosity level of 2.
-    """
-    tmpdir, eeyml = build_dir_and_ee_yml("")
-    result = cli(f"ansible-builder create -c {tmpdir} -f {eeyml}")
-    assert 'Ansible Builder is generating your execution environment build context.' not in result.stdout
-    assert f'The build context can be found at: {tmpdir}' in result.stdout
-
-
-def test_create_streams_output_with_invalid_verbosity(cli, build_dir_and_ee_yml):
-    """
-    Like the test_create_streams_output_with_verbosity_off test but making sure it errors out correctly with invalid verbosity level.
-    """
-    tmpdir, eeyml = build_dir_and_ee_yml("")
-    result = cli(f"ansible-builder create -c {tmpdir} -f {eeyml} -v 6", allow_error=True)
-    assert result.rc != 0
-    assert 'invalid choice: 6 (choose from 0, 1, 2, 3)' in (result.stdout + result.stderr)
-
-
-def test_collection_verification_off(cli, build_dir_and_ee_yml):
-    """
-    Test that, by default, collection verification is off via the env var.
-    """
-    ee = [
+def test_prepare_galaxy_install_steps(build_dir_and_ee_yml):
+    ee_data = [
         'dependencies:',
         '  galaxy: requirements.yml',
     ]
-    req = [
-        'collections:',
-        '  - name: community.general',
-    ]
-    tmpdir, eeyml = build_dir_and_ee_yml("\n".join(ee))
-    reqyml = tmpdir / "requirements.yml"
-    reqyml.write_text("\n".join(req))
-    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
-
-    containerfile = tmpdir / "Containerfile"
-    assert containerfile.exists()
-    assert "RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy" in containerfile.read_text()
-
-
-def test_collection_verification_on(cli, build_dir_and_ee_yml):
-    """
-    Test that collection verification is on when given a keyring.
-    """
-    ee = [
+    tmpdir, ee_path = build_dir_and_ee_yml("\n".join(ee_data))
+    c = make_containerfile(tmpdir, ee_path)
+    c._prepare_galaxy_install_steps()
+    expected = [
+        f"RUN ansible-galaxy role install $ANSIBLE_GALAXY_CLI_ROLE_OPTS -r {constants.CONTEXT_FILES['galaxy']} --roles-path \"{constants.base_roles_path}\"",
+        f"RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy collection install "
+        f"$ANSIBLE_GALAXY_CLI_COLLECTION_OPTS -r {constants.CONTEXT_FILES['galaxy']} --collections-path \"{constants.base_collections_path}\""
+    ]
+    assert c.steps == expected
+
+
+def test_prepare_galaxy_install_steps_with_keyring(build_dir_and_ee_yml):
+    ee_data = [
+        'dependencies:',
+        '  galaxy: requirements.yml',
+    ]
+    tmpdir, ee_path = build_dir_and_ee_yml("\n".join(ee_data))
+    c = make_containerfile(tmpdir, ee_path, galaxy_keyring=constants.default_keyring_name)
+    c._prepare_galaxy_install_steps()
+    expected = [
+        f"RUN ansible-galaxy role install $ANSIBLE_GALAXY_CLI_ROLE_OPTS -r {constants.CONTEXT_FILES['galaxy']} --roles-path \"{constants.base_roles_path}\"",
+        f"RUN ansible-galaxy collection install $ANSIBLE_GALAXY_CLI_COLLECTION_OPTS -r {constants.CONTEXT_FILES['galaxy']} "
+        f"--collections-path \"{constants.base_collections_path}\" --keyring \"{constants.default_keyring_name}\""
+    ]
+    assert c.steps == expected
+
+
+def test_prepare_galaxy_install_steps_with_sigcount(build_dir_and_ee_yml):
+    sig_count = 3
+    ee_data = [
         'dependencies:',
         '  galaxy: requirements.yml',
     ]
-    req = [
-        'collections:',
-        '  - name: community.general',
-    ]
-    tmpdir, eeyml = build_dir_and_ee_yml("\n".join(ee))
-    reqyml = tmpdir / "requirements.yml"
-    reqyml.write_text("\n".join(req))
-    keyring = tmpdir / "mykeyring.gpg"
-    keyring.touch()
-    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile --galaxy-keyring {keyring}')
-
-    containerfile = tmpdir / "Containerfile"
-    assert containerfile.exists()
-    text = containerfile.read_text()
-
-    keyring_copy = tmpdir / constants.user_content_subfolder / constants.default_keyring_name
-    assert keyring_copy.exists()
-
-    assert "RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy" not in text
-    assert f"--keyring \"{constants.default_keyring_name}\"" in text
-
-
-def test_galaxy_signing_extra_args(cli, build_dir_and_ee_yml):
-    """
-    Test that all extr asigning args for gpg are passed into the container file.
-    """
-    ee = [
+    tmpdir, ee_path = build_dir_and_ee_yml("\n".join(ee_data))
+    c = make_containerfile(tmpdir, ee_path,
+                           galaxy_keyring=constants.default_keyring_name,
+                           galaxy_required_valid_signature_count=sig_count)
+    c._prepare_galaxy_install_steps()
+    expected = [
+        f"RUN ansible-galaxy role install $ANSIBLE_GALAXY_CLI_ROLE_OPTS -r {constants.CONTEXT_FILES['galaxy']} --roles-path \"{constants.base_roles_path}\"",
+        f"RUN ansible-galaxy collection install $ANSIBLE_GALAXY_CLI_COLLECTION_OPTS -r {constants.CONTEXT_FILES['galaxy']} "
+        f"--collections-path \"{constants.base_collections_path}\" --required-valid-signature-count {sig_count} --keyring \"{constants.default_keyring_name}\""
+    ]
+    assert c.steps == expected
+
+
+def test_prepare_galaxy_install_steps_with_ignore_code(build_dir_and_ee_yml):
+    codes = [1, 2]
+    ee_data = [
         'dependencies:',
         '  galaxy: requirements.yml',
     ]
-    req = [
-        'collections:',
-        '  - name: community.general',
-    ]
-    tmpdir, eeyml = build_dir_and_ee_yml("\n".join(ee))
-    reqyml = tmpdir / "requirements.yml"
-    reqyml.write_text("\n".join(req))
-    keyring = tmpdir / "mykeyring.gpg"
-    keyring.touch()
-    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile --galaxy-keyring {keyring} '
-        '--galaxy-ignore-signature-status-code 500 --galaxy-required-valid-signature-count 3')
-
-    containerfile = tmpdir / "Containerfile"
-    assert containerfile.exists()
-    text = containerfile.read_text()
-
-    assert "--ignore-signature-status-code 500" in text
-    assert "--required-valid-signature-count 3" in text
+    tmpdir, ee_path = build_dir_and_ee_yml("\n".join(ee_data))
+    c = make_containerfile(tmpdir, ee_path,
+                           galaxy_keyring=constants.default_keyring_name,
+                           galaxy_ignore_signature_status_codes=codes)
+    c._prepare_galaxy_install_steps()
+    expected = [
+        f"RUN ansible-galaxy role install $ANSIBLE_GALAXY_CLI_ROLE_OPTS -r {constants.CONTEXT_FILES['galaxy']} --roles-path \"{constants.base_roles_path}\"",
+        f"RUN ansible-galaxy collection install $ANSIBLE_GALAXY_CLI_COLLECTION_OPTS -r {constants.CONTEXT_FILES['galaxy']} "
+        f"--collections-path \"{constants.base_collections_path}\" "
+        f"--ignore-signature-status-code {codes[0]} --ignore-signature-status-code {codes[1]} "
+        f"--keyring \"{constants.default_keyring_name}\""
+    ]
+    assert c.steps == expected
```

### Comparing `ansible-builder-1.2.0/test/integration/test_help.py` & `ansible-builder-3.0.0.0b1/test/integration/test_help.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/integration/test_introspect_cli.py` & `ansible-builder-3.0.0.0b1/test/integration/test_introspect_cli.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/pulp_integration/test_policies.py` & `ansible-builder-3.0.0.0b1/test/pulp_integration/test_policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/unit/test_cli.py` & `ansible-builder-3.0.0.0b1/test/unit/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -210,7 +210,67 @@
         prepare(['build',
                  '-f', path,
                  '-c', str(tmp_path),
                  '--container-policy', 'signature_required',
                  '--container-runtime', 'podman',
                  '--container-keyring', 'TBD',
                  ])
+
+
+def test_squash_default(exec_env_definition_file, tmp_path):
+    '''
+    Test the squash CLI option with default.
+    '''
+    content = {'version': 2}
+    path = str(exec_env_definition_file(content=content))
+    aee = prepare(['build',
+                   '-f', path,
+                   '-c', str(tmp_path),
+                   '--container-runtime', 'podman',
+                   ])
+    assert '--squash' in aee.build_command
+    assert '--squash-all' not in aee.build_command
+
+
+def test_squash_all(exec_env_definition_file, tmp_path):
+    '''
+    Test the squash CLI option with 'all'.
+    '''
+    content = {'version': 2}
+    path = str(exec_env_definition_file(content=content))
+    aee = prepare(['build',
+                   '-f', path,
+                   '-c', str(tmp_path),
+                   '--container-runtime', 'podman',
+                   '--squash', 'all'
+                   ])
+    assert '--squash-all' in aee.build_command
+
+
+def test_squash_off(exec_env_definition_file, tmp_path):
+    '''
+    Test the squash CLI option with 'off'.
+    '''
+    content = {'version': 2}
+    path = str(exec_env_definition_file(content=content))
+    aee = prepare(['build',
+                   '-f', path,
+                   '-c', str(tmp_path),
+                   '--container-runtime', 'podman',
+                   '--squash', 'off'
+                   ])
+    assert '--squash' not in aee.build_command
+
+
+def test_squash_ignored(exec_env_definition_file, tmp_path):
+    '''
+    Test the squash CLI option is ignored with docker.
+    '''
+    content = {'version': 2}
+    path = str(exec_env_definition_file(content=content))
+    aee = prepare(['build',
+                   '-f', path,
+                   '-c', str(tmp_path),
+                   '--container-runtime', 'docker',
+                   '--squash', 'all'
+                   ])
+    assert '--squash' not in aee.build_command
```

### Comparing `ansible-builder-1.2.0/test/unit/test_introspect.py` & `ansible-builder-3.0.0.0b1/test/unit/test_introspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from ansible_builder.introspect import process, process_collection, simple_combine
+from ansible_builder._target_scripts.introspect import process, process_collection, simple_combine
 from ansible_builder.requirements import sanitize_requirements
 
 
 def test_multiple_collection_metadata(data_dir):
 
     files = process(data_dir)
     files['python'] = sanitize_requirements(files['python'])
```

### Comparing `ansible-builder-1.2.0/test/unit/test_main.py` & `ansible-builder-3.0.0.0b1/test/unit/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import os
-import pathlib
-
 import pytest
 
 from ansible_builder import constants
 from ansible_builder.main import AnsibleBuilder
 
 
 def test_definition_version(exec_env_definition_file):
     path = exec_env_definition_file(content={'version': 1})
     aee = AnsibleBuilder(filename=path)
-    assert aee.version == '1'
+    assert aee.version == 1
 
 
 def test_definition_version_missing(exec_env_definition_file):
     path = exec_env_definition_file(content={})
     aee = AnsibleBuilder(filename=path)
-    assert aee.version == '1'
+    assert aee.version == 1
 
 
 @pytest.mark.parametrize('path_spec', ('absolute', 'relative'))
 def test_galaxy_requirements(exec_env_definition_file, galaxy_requirements_file, path_spec, tmp_path):
     galaxy_requirements_content = {
         'collections': [
             {'name': 'geerlingguy.php_roles', 'version': '0.9.3', 'source': 'https://galaxy.ansible.com'}
@@ -40,15 +37,15 @@
 
     aee = AnsibleBuilder(filename=exec_env_path, build_context=str(tmp_path / 'bc'))
     aee.build()
 
     with open(aee.containerfile.path) as f:
         content = f.read()
 
-    assert f'ADD {constants.user_content_subfolder} /build' in content
+    assert f'COPY {constants.user_content_subfolder} /build' in content
 
 
 def test_base_image_via_build_args(exec_env_definition_file, tmp_path):
     content = {'version': 1}
     path = exec_env_definition_file(content=content)
     aee = AnsibleBuilder(filename=path, build_context=tmp_path.joinpath('bc').as_posix())
     aee.build()
@@ -80,63 +77,63 @@
     path = exec_env_definition_file(content=content)
     aee = AnsibleBuilder(filename=path, build_context=tmp_path.joinpath('bc'))
     aee.build()
 
     with open(aee.containerfile.path) as f:
         content = f.read()
 
-    assert 'EE_BASE_IMAGE=my-other-custom-image' in content
+    assert 'EE_BASE_IMAGE="my-other-custom-image"' in content
 
 
 @pytest.mark.test_all_runtimes
 def test_build_command(exec_env_definition_file, runtime):
     content = {'version': 1}
     path = exec_env_definition_file(content=content)
 
-    aee = AnsibleBuilder(filename=path, tag='my-custom-image')
+    aee = AnsibleBuilder(filename=path, tag=['my-custom-image'])
     command = aee.build_command
     assert 'build' and 'my-custom-image' in command
 
     aee = AnsibleBuilder(filename=path, build_context='foo/bar/path', container_runtime=runtime)
 
     command = aee.build_command
     assert 'foo/bar/path' in command
-    assert 'foo/bar/path/Dockerfile' in " ".join(command)
+    fpath = 'foo/bar/path/' + constants.runtime_files[runtime]
+    assert fpath in " ".join(command)
 
 
 def test_nested_galaxy_file(data_dir, tmp_path):
-    if not os.path.exists('test/data/nested-galaxy.yml'):
-        pytest.skip('Test is only valid when ran from ansible-builder root')
-
-    AnsibleBuilder(filename='test/data/nested-galaxy.yml', build_context=tmp_path).build()
+    nested_galaxy_file = str(data_dir / 'nested_galaxy_file' / 'nested-galaxy.yml')
+    AnsibleBuilder(filename=nested_galaxy_file, build_context=tmp_path).build()
 
     req_in_bc = tmp_path.joinpath(constants.user_content_subfolder, 'requirements.yml')
     assert req_in_bc.exists()
 
-    req_original = pathlib.Path('test/data/foo/requirements.yml')
+    req_original = data_dir / 'nested_galaxy_file' / 'foo' / 'requirements.yml'
     assert req_in_bc.read_text() == req_original.read_text()
 
 
-def test_ansible_config_for_galaxy(exec_env_definition_file, tmp_path):
-    if not os.path.exists('test/data/ansible-test.cfg'):
-        pytest.skip('Test is only valid when ran from ansible-builder root')
-
-    ansible_config_path = 'test/data/ansible-test.cfg'
+def test_ansible_config_for_galaxy(exec_env_definition_file, tmp_path, data_dir):
+    ansible_config_path = str(data_dir / 'ansible_cfg_for_galaxy' / 'ansible-test.cfg')
+    galaxy_req = str(data_dir / 'ansible_cfg_for_galaxy' / 'requirements.yml')
     content = {
         'version': 1,
-        'ansible_config': ansible_config_path
+        'ansible_config': ansible_config_path,
+        'dependencies': {
+            'galaxy': galaxy_req,
+        },
     }
     path = exec_env_definition_file(content=content)
     aee = AnsibleBuilder(filename=path, build_context=tmp_path.joinpath('bc'))
     aee.build()
 
     with open(aee.containerfile.path) as f:
         content = f.read()
 
-    assert f'ADD {constants.user_content_subfolder}/ansible.cfg ~/.ansible.cfg' in content
+    assert f'COPY {constants.user_content_subfolder}/ansible.cfg ~/.ansible.cfg' in content
 
 
 @pytest.mark.test_all_runtimes
 def test_use_dockerfile(exec_env_definition_file, tmp_path, runtime):
     path = exec_env_definition_file(content={'version': 1})
     aee = AnsibleBuilder(
         filename=path, build_context=tmp_path.joinpath('bc'),
```

### Comparing `ansible-builder-1.2.0/test/unit/test_policies.py` & `ansible-builder-3.0.0.0b1/test/unit/test_policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/unit/test_requirements.py` & `ansible-builder-3.0.0.0b1/test/unit/test_requirements.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/test/unit/test_utils.py` & `ansible-builder-3.0.0.0b1/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-1.2.0/tox.ini` & `ansible-builder-3.0.0.0b1/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 [testenv]
 description = Run all tests with {basepython}
 usedevelop = True
 deps =
     -r {toxinidir}/test/requirements.txt
 commands = pytest {posargs}
 
-[testenv:linters]
+[testenv:linters{,-py39,-py310,-py311}]
 description = Run code linters
 commands =
     flake8 --version
     flake8 ansible_builder test
     yamllint --version
     yamllint -s .
+    mypy ansible_builder
 
-[testenv:unit{,-py38,-py39,-py310}]
+[testenv:unit{,-py39,-py310,-py311}]
 description = Run unit tests
 commands = pytest {posargs:test/unit}
 
-[testenv:pulp-integration{,-py310}]
+[testenv:pulp-integration{-py39,-py310,-py311}]
 # Some of these tests must run serially because of a shared resource
 # (the system policy.json file).
 description = Run pulp integration tests
-commands = pytest -n 1 -m "serial" {posargs:test/pulp_integration}
+commands =
+    pytest -n 1 -m "serial" {posargs:test/pulp_integration}
+    pytest -m "not serial" {posargs:test/pulp_integration}
 
-[testenv:integration{,-py38,-py39,-py310}]
+[testenv:integration{,-py39,-py310,-py311}]
 description = Run integration tests
 # rootless podman reads $HOME
 passenv =
     HOME
     KEEP_IMAGES
 commands = pytest {posargs:test/integration}
```

