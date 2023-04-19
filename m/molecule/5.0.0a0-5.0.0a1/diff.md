# Comparing `tmp/molecule-5.0.0a0.tar.gz` & `tmp/molecule-5.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-5.0.0a0.tar", last modified: Tue Feb  7 16:20:19 2023, max compression
+gzip compressed data, was "molecule-5.0.0a1.tar", last modified: Wed Apr 19 17:52:07 2023, max compression
```

## Comparing `molecule-5.0.0a0.tar` & `molecule-5.0.0a1.tar`

### file list

```diff
@@ -1,440 +1,422 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.047816 molecule-5.0.0a0/.config/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.047816 molecule-5.0.0a0/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.config/molecule/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.config/molecule.spec
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.047816 molecule-5.0.0a0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.051817 molecule-5.0.0a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.051817 molecule-5.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3358 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.npmrc
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-02-07 16:20:01.000000 molecule-5.0.0a0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-02-07 16:20:01.000000 molecule-5.0.0a0/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-02-07 16:20:01.000000 molecule-5.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4636 2023-02-07 16:20:19.159817 molecule-5.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-02-07 16:20:01.000000 molecule-5.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-02-07 16:20:01.000000 molecule-5.0.0a0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-02-07 16:20:01.000000 molecule-5.0.0a0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-02-07 16:20:01.000000 molecule-5.0.0a0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.055817 molecule-5.0.0a0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:18.995816 molecule-5.0.0a0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.055817 molecule-5.0.0a0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (122)    15406 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    33945 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/_static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)   143898 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/_static/images/logo_big.png
--rw-r--r--   0 runner    (1001) docker     (122)    10484 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (122)     7997 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (122)     3599 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (122)    12956 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (122)     6991 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/getting-started.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.055817 molecule-5.0.0a0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (122)    15406 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    33945 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     4347 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-02-07 16:20:01.000000 molecule-5.0.0a0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-02-07 16:20:01.000000 molecule-5.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-02-07 16:20:01.000000 molecule-5.0.0a0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.059816 molecule-5.0.0a0/playbooks/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-02-07 16:20:01.000000 molecule-5.0.0a0/playbooks/snap-pre-run.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4781 2023-02-07 16:20:01.000000 molecule-5.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-02-07 16:20:01.000000 molecule-5.0.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-02-07 16:20:01.000000 molecule-5.0.0a0/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-07 16:20:19.159817 molecule-5.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.059816 molecule-5.0.0a0/snap/
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-02-07 16:20:01.000000 molecule-5.0.0a0/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:18.999817 molecule-5.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.063816 molecule-5.0.0a0/src/molecule/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.075816 molecule-5.0.0a0/src/molecule/command/
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9273 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/converge.py
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/drivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4540 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/idempotence.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.075816 molecule-5.0.0a0/src/molecule/command/init/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3507 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/init/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/init/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     5942 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/init/role.py
--rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/init/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     3696 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4546 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/prepare.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/reset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/side_effect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/syntax.py
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/command/verify.py
--rw-r--r--   0 runner    (1001) docker     (122)    17043 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/console.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.003816 molecule-5.0.0a0/src/molecule/cookiecutter/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.075816 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.075816 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.003816 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.003816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.003816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.003816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.007816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/ansible/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/ansible/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.007816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.007816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.007816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.079816 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.083816 molecule-5.0.0a0/src/molecule/data/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15363 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/data/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.083816 molecule-5.0.0a0/src/molecule/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.087817 molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4327 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     4194 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/dependency/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.087817 molecule-5.0.0a0/src/molecule/driver/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9288 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     9098 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/driver/delegated.py
--rw-r--r--   0 runner    (1001) docker     (122)     4444 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6682 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.087817 molecule-5.0.0a0/src/molecule/model/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/model/schema_v3.py
--rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.091817 molecule-5.0.0a0/src/molecule/provisioner/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    33579 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/provisioner/ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/provisioner/ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/provisioner/ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/provisioner/base.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     4949 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (122)     5765 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/shell.py
--rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.091817 molecule-5.0.0a0/src/molecule/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4709 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.095816 molecule-5.0.0a0/src/molecule/test/functional/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8876 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/functional/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.095816 molecule-5.0.0a0/src/molecule/test/resources/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.095816 molecule-5.0.0a0/src/molecule/test/resources/invalid_role_template/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.099816 molecule-5.0.0a0/src/molecule/test/resources/invalid_role_template/bad_format/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/invalid_role_template/bad_format/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/invalid_role_template/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.011816 molecule-5.0.0a0/src/molecule/test/resources/playbooks/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.099816 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/create.yml
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.015817 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.015817 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.099816 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.015817 molecule-5.0.0a0/src/molecule/test/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.015817 molecule-5.0.0a0/src/molecule/test/resources/roles/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.099816 molecule-5.0.0a0/src/molecule/test/resources/roles/molecule/meta/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/roles/molecule/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.099816 molecule-5.0.0a0/src/molecule/test/resources/roles/molecule/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/roles/molecule/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.019816 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.019816 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.019816 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/template.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.019816 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      218 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.103817 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/meta/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.107817 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.107817 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.107817 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.107817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.023816 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/hosts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.111817 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/links/
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/idempotence/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/interpolation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/interpolation/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/overrride_driver/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      333 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.027816 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.115816 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.119817 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.119817 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.031816 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.119817 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.123817 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.123817 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.123817 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.123817 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.131816 molecule-5.0.0a0/src/molecule/test/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.143817 molecule-5.0.0a0/src/molecule/test/unit/command/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.143817 molecule-5.0.0a0/src/molecule/test/unit/command/init/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/init/test_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/init/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)    11367 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     2658 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1786 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     5017 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_idempotence.py
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4722 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_side_effect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/command/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (122)     6424 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.143817 molecule-5.0.0a0/src/molecule/test/unit/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2302 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/cookiecutter/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.147817 molecule-5.0.0a0/src/molecule/test/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.147817 molecule-5.0.0a0/src/molecule/test/unit/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6832 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     6671 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     4476 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/dependency/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.147817 molecule-5.0.0a0/src/molecule/test/unit/driver/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9573 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/driver/test_delegated.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.151816 molecule-5.0.0a0/src/molecule/test/unit/lint/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.151816 molecule-5.0.0a0/src/molecule/test/unit/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.151816 molecule-5.0.0a0/src/molecule/test/unit/model/v2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_dependency_section.py
--rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_driver_section.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_platforms_section.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_provisioner_section.py
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_scenario_section.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_verifier_section.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.151816 molecule-5.0.0a0/src/molecule/test/unit/provisioner/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25333 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/provisioner/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)     7220 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/provisioner/test_ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (122)     4488 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/provisioner/test_ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    10802 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4145 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (122)     6767 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     6301 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_scenarios_ordered.py
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_text.py
--rw-r--r--   0 runner    (1001) docker     (122)     9545 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.151816 molecule-5.0.0a0/src/molecule/test/unit/verifier/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2790 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/verifier/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/test/unit/verifier/test_testinfra.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/text.py
--rw-r--r--   0 runner    (1001) docker     (122)    12951 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.155817 molecule-5.0.0a0/src/molecule/verifier/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/verifier/ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/verifier/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6782 2023-02-07 16:20:01.000000 molecule-5.0.0a0/src/molecule/verifier/testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.067817 molecule-5.0.0a0/src/molecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4636 2023-02-07 16:20:18.000000 molecule-5.0.0a0/src/molecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13741 2023-02-07 16:20:18.000000 molecule-5.0.0a0/src/molecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 16:20:18.000000 molecule-5.0.0a0/src/molecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-02-07 16:20:18.000000 molecule-5.0.0a0/src/molecule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-02-07 16:20:18.000000 molecule-5.0.0a0/src/molecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-07 16:20:18.000000 molecule-5.0.0a0/src/molecule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.155817 molecule-5.0.0a0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (122)      248 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/get-version.sh
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/opts.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      235 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/smoketest.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/.mocharc.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/f/
--rw-r--r--   0 runner    (1001) docker     (122)    15363 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/f/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.035817 molecule-5.0.0a0/tools/test-schema/negative_test/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.035817 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/platforms_children/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/platforms_children/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/platforms_children/molecule.yml.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/platforms_networks/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/platforms_networks/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/negative_test/molecule/platforms_networks/molecule.yml.md
--rw-r--r--   0 runner    (1001) docker     (122)    87766 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/src/
--rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/src/schema.spec.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.035817 molecule-5.0.0a0/tools/test-schema/test/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.035817 molecule-5.0.0a0/tools/test-schema/test/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/test/molecule/cluster/
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/test/molecule/cluster/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/test/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/test/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 16:20:19.159817 molecule-5.0.0a0/tools/test-schema/test/molecule/vagrant/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/test/molecule/vagrant/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-schema/tsconfig.json
--rwxr-xr-x   0 runner    (1001) docker     (122)      688 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      214 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (122)     4867 2023-02-07 16:20:01.000000 molecule-5.0.0a0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.041295 molecule-5.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.965293 molecule-5.0.0a1/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.965293 molecule-5.0.0a1/.config/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.config/molecule/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.config/molecule.spec
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/patchback.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.969293 molecule-5.0.0a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-19 17:51:46.000000 molecule-5.0.0a1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-19 17:51:46.000000 molecule-5.0.0a1/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 17:51:46.000000 molecule-5.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 17:51:46.000000 molecule-5.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-19 17:52:07.041295 molecule-5.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-19 17:51:46.000000 molecule-5.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 17:51:47.000000 molecule-5.0.0a1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 17:51:47.000000 molecule-5.0.0a1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-19 17:51:47.000000 molecule-5.0.0a1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.933292 molecule-5.0.0a1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/_static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/_static/images/logo_big.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/getting-started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-19 17:51:47.000000 molecule-5.0.0a1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-19 17:51:47.000000 molecule-5.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-19 17:51:47.000000 molecule-5.0.0a1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.973293 molecule-5.0.0a1/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 17:51:47.000000 molecule-5.0.0a1/playbooks/snap-pre-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-19 17:51:47.000000 molecule-5.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-19 17:51:47.000000 molecule-5.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 17:51:47.000000 molecule-5.0.0a1/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:52:07.041295 molecule-5.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.977293 molecule-5.0.0a1/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 17:51:47.000000 molecule-5.0.0a1/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.981293 molecule-5.0.0a1/src/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/idempotence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/init/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/command/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.937292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.989294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/data/driver.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/data/molecule.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.993294 molecule-5.0.0a1/src/molecule/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/dependency/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/driver/delegated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/model/schema_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34238 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/provisioner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.997294 molecule-5.0.0a1/src/molecule/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/functional/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/invalid_role_template/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/test/resources/playbooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.941292 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/roles/molecule/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.001294 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.945292 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.005294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/hosts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.009294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.949292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/idempotence/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.013294 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.953292 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.957293 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.017295 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.021294 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.025295 molecule-5.0.0a1/src/molecule/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.029295 molecule-5.0.0a1/src/molecule/test/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.029295 molecule-5.0.0a1/src/molecule/test/unit/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/init/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/init/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_idempotence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/command/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/dependency/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/driver/test_delegated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.033295 molecule-5.0.0a1/src/molecule/test/unit/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_dependency_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_driver_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_platforms_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_provisioner_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_scenario_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_verifier_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.037295 molecule-5.0.0a1/src/molecule/test/unit/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25691 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_scenarios_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.037295 molecule-5.0.0a1/src/molecule/test/unit/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/verifier/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/test/unit/verifier/test_testinfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.037295 molecule-5.0.0a1/src/molecule/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-19 17:51:47.000000 molecule-5.0.0a1/src/molecule/verifier/testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:06.981293 molecule-5.0.0a1/src/molecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 17:52:06.000000 molecule-5.0.0a1/src/molecule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:52:07.041295 molecule-5.0.0a1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/get-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/opts.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/smoketest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-19 17:51:47.000000 molecule-5.0.0a1/tox.ini
```

### Comparing `molecule-5.0.0a0/.config/molecule.spec` & `molecule-5.0.0a1/.config/molecule.spec`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/.gitattributes` & `molecule-5.0.0a1/.gitattributes`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md` & `molecule-5.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/.github/ISSUE_TEMPLATE/config.yml` & `molecule-5.0.0a1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/.github/dependabot.yml` & `molecule-5.0.0a1/.github/dependabot.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically/enabling-and-disabling-dependabot-version-updates
 version: 2
+enable-beta-ecosystems: true
 updates:
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
-      interval: "daily"
+      interval: daily
     labels:
       - dependencies
       - skip-changelog
-    open-pull-requests-limit: 3
     allow:
-      - dependency-type: all
+      - dependency-name: "ansible*"
+      - dependency-name: pyyaml
   - package-ecosystem: "github-actions"
     directory: "/"
     schedule:
       interval: daily
-    open-pull-requests-limit: 3
     labels:
-      - "dependencies"
-      - "skip-changelog"
+      - dependencies
+      - skip-changelog
```

### Comparing `molecule-5.0.0a0/.github/workflows/tox.yml` & `molecule-5.0.0a1/.github/workflows/tox.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+---
 name: tox
 
 on:
-  create: # is used for publishing to PyPI and TestPyPI
-    tags: # any tag regardless of its name, no branches
   push: # only publishes pushes to the main branch to TestPyPI
     branches: # any integration branch but not tag
       - "main"
-    tags-ignore:
-      - "**"
   pull_request:
-  schedule:
-    - cron: 1 0 * * * # Run daily at 0:01 UTC
+    branches:
+      - "main"
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
+  cancel-in-progress: true
+
+env:
+  FORCE_COLOR: 1 # tox, pytest, ansible-lint
+  PY_COLORS: 1
 
 jobs:
   pre:
     name: pre
     runs-on: ubuntu-22.04
     outputs:
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
@@ -26,34 +31,44 @@
           min_python: "3.9"
           max_python: "3.11"
           other_names: |
             lint
             docs
             pkg
             eco
-            py39-devel
-            py310-devel
+            py311-devel
 
   build:
     name: ${{ matrix.name }}
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os || 'ubuntu-22.04' }}
     needs: pre
-    env:
-      PYTEST_REQPASS: 453
+    defaults:
+      run:
+        shell: ${{ matrix.shell || 'bash'}}
     # limit potential endless looks like we had with build-containers
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
 
+    env:
+      PYTEST_REQPASS: 454
     steps:
-      - name: Check out src from Git
-        uses: actions/checkout@v3
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
+          submodules: true
+
+      - name: Set pre-commit cache
+        uses: actions/cache@v3
+        if: ${{ matrix.passed_name == 'lint' }}
+        with:
+          path: |
+            ~/.cache/pre-commit
+          key: pre-commit-${{ matrix.name || matrix.passed_name }}-${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Install system dependencies
         # remove broken .deb ansible and replace with pip version:
         # https://github.com/actions/virtual-environments/issues/3001
         run: |
           sudo apt-get remove -y ansible \
           && sudo apt-get update \
           && sudo apt-get install -y libvirt-dev python3-cryptography python3-jinja2 python3-yaml virtualenv \
@@ -62,26 +77,36 @@
         # https://docs.github.com/en/actions/reference/workflow-commands-for-github-actions#adding-a-system-path
       - name: Validate that ansible works
         run: |
           ansible --version \
           && virtualenv foo \
           && source foo/bin/activate \
           && ansible --version
-      - name: Install a default Python
+      - name: Set up Python ${{ matrix.python_version || '3.9' }}
+        if: "!contains(matrix.shell, 'wsl')"
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python_version }}
-      - name: Install dependencies
-        run: |
-          python3 -m pip install -U pip 'coverage[toml]'
-          python3 -m pip install 'tox>=4.0.0'
-      - name: Run tox -e ${{ matrix.passed_name }}
+          cache: pip
+          python-version: ${{ matrix.python_version || '3.9' }}
+
+      - name: Install tox
         run: |
-          ${{ matrix.PREFIX }} tox -e ${{ matrix.passed_name }}
-        continue-on-error: ${{ matrix.experimental || false }}
+          python3 -m pip install --upgrade pip
+          python3 -m pip install --upgrade "tox>=4.0.0"
+
+      - name: Log installed dists
+        run: python3 -m pip freeze --all
+
+      - name: Initialize tox envs ${{ matrix.passed_name }}
+        run: python3 -m tox --notest --skip-missing-interpreters false -vv -e ${{ matrix.passed_name }}
+        timeout-minutes: 5 # average is under 1, but macos can be over 3
+
+      # sequential run improves browsing experience (almost no speed impact)
+      - name: tox -e ${{ matrix.passed_name }}
+        run: python3 -m tox -e ${{ matrix.passed_name }}
 
       - name: Combine coverage data
         if: ${{ startsWith(matrix.passed_name, 'py') }}
         # produce a single .coverage file at repo root
         run: tox -e coverage
 
       - name: Upload coverage data
@@ -89,14 +114,23 @@
         uses: codecov/codecov-action@v3
         with:
           name: ${{ matrix.passed_name }}
           fail_ci_if_error: false # see https://github.com/codecov/codecov-action/issues/598
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true # optional (default = false)
 
+      - name: Report failure if git reports dirty status
+        run: |
+          if [[ -n $(git status -s) ]]; then
+            # shellcheck disable=SC2016
+            echo -n '::error file=git-status::'
+            printf '### Failed as git reported modified and/or untracked files\n```\n%s\n```\n' "$(git status -s)" | tee -a "$GITHUB_STEP_SUMMARY"
+            exit 99
+          fi
+        # https://github.com/actions/toolkit/issues/193
   check:
     if: always()
 
     needs:
       - build
 
     runs-on: ubuntu-latest
```

### Comparing `molecule-5.0.0a0/.packit.yaml` & `molecule-5.0.0a1/.packit.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/.pre-commit-config.yaml` & `molecule-5.0.0a1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,72 @@
 ---
 ci:
   skip:
     # https://github.com/pre-commit-ci/issues/issues/55
     - pip-compile
-    - schema
 default_language_version:
   python: python3.9
 repos:
-  - repo: local
-    hooks:
-      - id: schema
-        name: schema
-        entry: bash -c "cd tools/test-schema && npm install && npm test"
-        pass_filenames: false
-        always_run: true
-        language: node
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.6"
     hooks:
       - id: prettier
         # Temporary excludes so we can gradually normalize the formatting
         exclude: >
           (?x)^(
             src/molecule/cookiecutter/.*|
             src/molecule/test/resources/templates/.*|
-            tools/test-schema/(negative_test|test)/.*|
           )$
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
   - repo: https://github.com/PyCQA/doc8
     rev: "v1.1.1"
     hooks:
       - id: doc8
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
-        exclude: >
-          (?x)^(
-            tools/test-schema/package-lock.json
-          )$
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
         language_version: python3
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - pydocstyle>=5.1.1
-          - flake8-absolute-import
-          - flake8-black>=0.1.1
-          - flake8-docstrings>=1.5.0
-        language_version: python3
+
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.29.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.261"
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.0
+    rev: v1.2.0
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: []
         entry: mypy src/
         pass_filenames: false
         additional_dependencies:
@@ -96,30 +78,32 @@
           - packaging
           - rich
           - ruamel.yaml>=0.17.10
           - types-PyYAML
           - types-dataclasses
           - types-filelock
           - types-setuptools
-  - repo: https://github.com/PyCQA/pylint
-    rev: v2.16.1
+  - repo: https://github.com/pycqa/pylint
+    rev: v3.0.0a6
     hooks:
       - id: pylint
+        args:
+          - --output-format=colorized
         additional_dependencies:
           - ansible-compat>=2.2.0
           - click
           - click-help-colors
           - cookiecutter
           - enrich>=1.2.7
           - filelock
           - jsonschema
           - pexpect
           - testinfra
   - repo: https://github.com/jazzband/pip-tools
-    rev: 6.12.2
+    rev: 6.13.0
     hooks:
       - id: pip-compile
         entry: pip-compile -q --resolver=backtracking --strip-extras --no-annotate --output-file=requirements.txt tools/opts.txt pyproject.toml --extra docs --extra test --extra lint
         files: ^(pyproject\.toml|requirements.txt|constraints\.txt)$
       - id: pip-compile
         name: pip-compile-upgrade
         entry: pip-compile -q  --resolver=backtracking --strip-extras -q --upgrade --no-annotate --output-file=requirements.txt tools/opts.txt pyproject.toml --extra docs --extra test --extra lint
```

### Comparing `molecule-5.0.0a0/.yamllint` & `molecule-5.0.0a1/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/DCO_1_1.md` & `molecule-5.0.0a1/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/LICENSE` & `molecule-5.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/PKG-INFO` & `molecule-5.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 5.0.0a0
+Version: 5.0.0a1
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
```

### Comparing `molecule-5.0.0a0/README.md` & `molecule-5.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/bindep.txt` & `molecule-5.0.0a1/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/conftest.py` & `molecule-5.0.0a1/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """PyTest Config File."""
 
-from __future__ import print_function
 
 import os
 
 import pytest
 
 
 @pytest.fixture(scope="session", autouse=True)
```

### Comparing `molecule-5.0.0a0/docs/_static/images/favicon.ico` & `molecule-5.0.0a1/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/_static/images/logo.png` & `molecule-5.0.0a1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/_static/images/logo_big.png` & `molecule-5.0.0a1/docs/_static/images/logo_big.png`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/ci.md` & `molecule-5.0.0a1/docs/ci.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/configuration.md` & `molecule-5.0.0a1/docs/configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 ## Role name check
 
 By default, `Molecule` will check whether the role name follows the name
 standard. If not, it will raise an error.
 
 If computed fully qualified role name does not follow current galaxy
-requirements, you can ignore it by adding [role_name_check:
-1]{.title-ref} inside the configuration file.
+requirements, you can ignore it by adding `role_name_check:1` inside the configuration file.
 
 It is strongly recommended to follow the name standard of
 [namespace](https://galaxy.ansible.com/docs/contributing/namespaces.html#galaxy-namespace-limitations)
 and
 [role](https://galaxy.ansible.com/docs/contributing/creating_role.html#role-names).
 
 ## Variable Substitution
@@ -134,17 +133,17 @@
 
 ::: molecule.dependency.shell.Shell
 
 ## Driver
 
 Molecule uses [Ansible](#ansible-1) to manage instances to operate on.
 Molecule supports any provider [Ansible](#ansible-1) supports. This work
-is offloaded to the [provisioner]{.title-ref}.
+is offloaded to the `provisioner`.
 
-The driver's name is specified in [molecule.yml]{.title-ref}, and can
+The driver's name is specified in `molecule.yml`, and can
 be overridden on the command line. Molecule will remember the last
 successful driver used, and continue to use the driver for all
 subsequent subcommands, or until the instances are destroyed by
 Molecule.
 
 !!! warning
```

### Comparing `molecule-5.0.0a0/docs/contributing.md` & `molecule-5.0.0a1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/examples.md` & `molecule-5.0.0a1/docs/examples.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 The `Dockerfile.j2` template is generated at
 `molecule init scenario`-time when `--driver-name` is `docker`. The
 template can be customized as needed to create the desired modifications
 to the Docker image used in the scenario.
 
 Note: `platforms[*].pre_build_image` defaults to `true` in each
-scenario's generated [molecule.yml]{.title-ref} file.
+scenario's generated `molecule.yml` file.
 
 ## Docker With Non-Privileged User
 
 The default Molecule Docker driver executes Ansible playbooks as the
 root user. If your workflow requires adding support for running as a
 non-privileged user, then adapt `molecule.yml` and `Dockerfile.j2` as
 follows.
 
 Note: The `Dockerfile` templating and image building processes are only
 done for scenarios with `pre_build_image = False`, which is not the
-default setting in generated [molecule.yml]{.title-ref} files.
+default setting in generated `molecule.yml` files.
 
 To modify the Docker image to support running as normal user:
 
 Append the following code block to the end of `Dockerfile.j2`. It
 creates an `ansible` user with passwordless sudo privileges. Note the
 variable `SUDO_GROUP` depends on the target distribution[^2].
 
@@ -343,25 +343,25 @@
 │   │   └── molecule.yml
 │   └── ubuntu-upstart
 │       └── molecule.yml
 ```
 
 Tests and playbooks can be shared across scenarios.
 
-In this example the [tests]{.title-ref} directory lives in a shared
+In this example the `tests` directory lives in a shared
 location and `molecule.yml` points to the shared tests.
 
 ```yaml
 verifier:
   name: testinfra
   directory: ../resources/tests/
 ```
 
-In this second example the actions [create]{.title-ref},
-[destroy]{.title-ref}, [converge]{.title-ref} and [prepare]{.title-ref}
+In this second example the actions `create`,
+`destroy`, `converge` and `prepare`
 are loaded from a shared directory.
 
 ```yaml
 provisioner:
   name: ansible
   playbooks:
     create: ../resources/playbooks/create.yml
```

### Comparing `molecule-5.0.0a0/docs/faq.md` & `molecule-5.0.0a1/docs/faq.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 ## Does Molecule support monorepos?
 
 Yes, roles contained in a
 [monorepo](https://en.wikipedia.org/wiki/Monorepo) with other roles are
 automatically picked up and `ANSIBLE_ROLES_PATH` is set accordingly. See
 [this
-page](https://molecule.readthedocs.io/en/latest/examples.html#monolith-repo)
+page](https://molecule.readthedocs.io/en/latest/examples/#monolith-repo)
 for more information.
 
 ## How can I add development/testing-only dependencies?
 
 Sometimes, it's desirable to only run a dependency role when developing
 your role with molecule, but not impose a hard dependency on the role
 itself; for example when you rely on one of its side effects. This can
```

### Comparing `molecule-5.0.0a0/docs/getting-started.md` & `molecule-5.0.0a1/docs/getting-started.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
   specify that in this section.
 - The [provisioner](/configuration/#provisioner). Molecule only
   provides an Ansible provisioner. Ansible manages the life cycle of
   the instance based on this configuration.
 - The [scenario][] definition.
   Molecule relies on this configuration to control the scenario
   sequence order.
-- The [verifier](/configuration/#verifier)` framework. Molecule
+- The [verifier](/configuration/#verifier) framework. Molecule
   uses Ansible by default to provide a way to write specific state
   checking tests (such as deployment smoke tests) on the target
   instance.
 
 ## Run test sequence commands
 
 Let's create the first Molecule managed instance with the Docker
```

### Comparing `molecule-5.0.0a0/docs/images/favicon.ico` & `molecule-5.0.0a1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/images/logo.png` & `molecule-5.0.0a1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/images/logo.svg` & `molecule-5.0.0a1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/index.md` & `molecule-5.0.0a1/docs/index.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/installation.md` & `molecule-5.0.0a1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/docs/usage.md` & `molecule-5.0.0a1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/mkdocs.yml` & `molecule-5.0.0a1/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 site_name: Ansible Molecule
 site_url: https://molecule.readthedocs.io/
 repo_url: https://github.com/ansible-community/molecule
 edit_uri: blob/main/docs/
 copyright: Copyright © 2023 Red Hat, Inc.
 strict: true
 
@@ -47,17 +48,17 @@
     - icon: fontawesome/solid/comments
       link: https://github.com/ansible-community/molecule/discussions
       name: Discussions
     - icon: fontawesome/brands/github-alt
       link: https://github.com/ansible-community/molecule
 
 nav:
-  - home: index.md
+  - Home: index.md
   - installation.md
-  - using:
+  - Using:
       - getting-started.md
       - usage.md
       - configuration.md
       - ci.md
   - examples.md
   - faq.md
   - contributing.md
@@ -95,22 +96,19 @@
   - def_list
   - footnotes
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.inlinehilite
   - pymdownx.snippets:
       check_paths: true
-  - pymdownx.superfences
   - pymdownx.magiclink:
       repo_url_shortener: true
       repo_url_shorthand: true
       social_url_shorthand: true
       social_url_shortener: true
-      user: facelessuser
-      repo: pymdown-extensions
       normalize_issue_symbols: true
   - pymdownx.tabbed:
       alternate_style: true
   - toc:
       # reduced to keep TOC nice under Changelog page
       toc_depth: 2
       permalink: true
```

### Comparing `molecule-5.0.0a0/mypy.ini` & `molecule-5.0.0a1/mypy.ini`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/playbooks/snap-pre-run.yaml` & `molecule-5.0.0a1/playbooks/snap-pre-run.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/pyproject.toml` & `molecule-5.0.0a1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -122,28 +122,85 @@
 # see https://github.com/PyCQA/doc8/issues/75
 ignore-path = [
   ".eggs",
   ".tox",
   "requirements.txt",
   "build",
   "molecule.egg-info",
-  "src/molecule.egg-info"
+  "src/molecule.egg-info",
 ]
 
 [tool.black]
 skip-string-normalization = false
 
 [tool.isort]
 profile = "black"
 known_first_party = "molecule"
 
+[tool.pylint."MESSAGES CONTROL"]
+disable = [
+  # TODO(ssbarnea): remove temporary skips adding during initial adoption:
+  "abstract-method",
+  "arguments-differ",
+  "broad-except",
+  "consider-merging-isinstance",
+  # We will clean this up in a dedicated refactoring commit
+  "consider-using-in",
+  "dangerous-default-value",
+  "duplicate-code",
+  "fixme",
+  "implicit-str-concat",
+  "import-outside-toplevel",
+  "inconsistent-return-statements",
+  "invalid-name",
+  "line-too-long",
+  "logging-format-interpolation",
+  "logging-not-lazy",
+  "missing-function-docstring",
+  "missing-module-docstring",
+  "no-else-raise",
+  "no-else-return",
+  "no-member",
+  "no-self-argument",
+  "no-value-for-parameter",
+  "not-callable",
+  "protected-access",
+  "raise-missing-from",
+  "redefined-builtin",
+  "redefined-outer-name",
+  "subprocess-run-check",
+  "super-init-not-called",
+  "super-with-arguments",
+  "too-few-public-methods",
+  "too-many-ancestors",
+  "too-many-arguments",
+  "too-many-public-methods",
+  "unidiomatic-typecheck",
+  "unnecessary-comprehension",
+  "unnecessary-lambda",
+  # Next rule was added because we cannot adjust the open calls during minor
+  # releases since there is no guarantee that this will not break existing
+  # scenarios (right now, we have no idea what encoding files that molecule
+  # wrote to disk have).
+  "unspecified-encoding",
+  "unused-argument",
+  "unused-import",
+  "unused-variable",
+  "useless-object-inheritance",
+  "useless-super-delegation",
+]
+
+[tool.pylint.SUMMARY]
+# We don't need the score spamming console, as we either pass or fail
+score = "n"
+
 [tool.pytest.ini_options]
 markers = [
   "serial: Run this test serially via filelock.",
-  "extensive: marks tests that we want to skip by default, as they are indirectly covered by other tests"
+  "extensive: marks tests that we want to skip by default, as they are indirectly covered by other tests",
 ]
 norecursedirs = [
   ".eggs",
   ".tox",
   "build",
   "dist",
   "doc",
@@ -162,9 +219,51 @@
   "ignore:path is deprecated.*:DeprecationWarning",
   # https://github.com/pytest-dev/pytest-cov/issues/557
   "ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning",
   # ignore::UserWarning
 
 ]
 
+[tool.ruff]
+ignore = [
+  "E501", # we use black
+  # temporary disabled until we fix them:
+  "A",
+  "ANN",
+  "ARG",
+  "B",
+  "BLE001",
+  "C901",
+  "D",
+  "E741",
+  "EM",
+  "EXE",
+  "FBT",
+  "INP",
+  "ISC",
+  "N",
+  "PGH",
+  "PLC",
+  "PLR",
+  "PLW",
+  "PT",
+  "PTH",
+  "RET",
+  "S",
+  "SIM",
+  "SLF",
+  "T",
+  "TRY",
+]
+select = ["ALL"]
+target-version = "py39"
+# Same as Black.
+line-length = 88
+
+[tool.ruff.flake8-pytest-style]
+parametrize-values-type = "tuple"
+
+[tool.ruff.isort]
+known-first-party = ["ansiblelint"]
+
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `molecule-5.0.0a0/requirements.txt` & `molecule-5.0.0a1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,118 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=docs --extra=lint --extra=test --no-annotate --output-file=requirements.txt --resolver=backtracking --strip-extras pyproject.toml tools/opts.txt
 #
 ansi2html==1.8.0
-ansible-compat==3.0.1
-ansible-core==2.14.2
-ansible-lint==6.12.1
-argparse-manpage==4
+ansible-compat==3.0.2
+ansible-core==2.14.4
+ansible-lint==6.14.6
+argparse-manpage==4.1
 arrow==1.2.3
 asyncio==3.4.3
-attrs==22.2.0
-babel==2.11.0
+attrs==23.1.0
+babel==2.12.1
 binaryornot==0.4.4
-black==23.1.0
+black==23.3.0
 bracex==2.3.post1
-cairocffi==1.4.0
-cairosvg==2.6.0
+cairocffi==1.5.1
+cairosvg==2.7.0
 certifi==2022.12.7
 cffi==1.15.1
 cfgv==3.3.1
 chardet==5.1.0
-charset-normalizer==3.0.1
-check-jsonschema==0.21.0
+charset-normalizer==3.1.0
+check-jsonschema==0.22.0
 click==8.1.3
 click-help-colors==0.9.1
 colorama==0.4.6
 cookiecutter==2.1.1
-coverage==7.1.0
-cryptography==39.0.0
+coverage==7.2.3
+cryptography==40.0.2
 cssselect2==0.7.0
 dacite==1.8.0
 defusedxml==0.7.1
 distlib==0.3.6
 distro==1.8.0
 enrich==1.2.7
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
 execnet==1.9.0
-filelock==3.9.0
+filelock==3.12.0
 flake8==6.0.0
 ghp-import==2.1.0
 gitdb==4.0.10
-gitpython==3.1.30
-griffe==0.25.4
-identify==2.5.17
+gitpython==3.1.31
+griffe==0.27.1
+identify==2.5.22
 idna==3.4
-importlib-metadata==6.0.0
+importlib-metadata==6.5.0
 iniconfig==2.0.0
 jinja2==3.1.2
 jinja2-time==0.2.0
 jsonschema==4.17.3
 markdown==3.3.7
 markdown-include==0.8.1
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
 markupsafe==2.1.2
 mccabe==0.7.0
 mdurl==0.1.2
 mergedeep==1.3.4
 mkdocs==1.4.2
 mkdocs-autorefs==0.4.1
-mkdocs-git-revision-date-localized-plugin==1.1.0
-mkdocs-material==9.0.11
+mkdocs-git-revision-date-localized-plugin==1.2.0
+mkdocs-material==9.1.6
 mkdocs-material-extensions==1.1.1
-mkdocs-multirepo-plugin==0.6.0
-mkdocstrings==0.20.0
-mkdocstrings-python==0.8.3
+mkdocs-multirepo-plugin==0.6.1
+mkdocstrings==0.21.2
+mkdocstrings-python==0.9.0
 mypy-extensions==1.0.0
 nodeenv==1.7.0
-packaging==23.0
-pathspec==0.11.0
+packaging==23.1
+pathspec==0.11.1
 pexpect==4.8.0
-pillow==9.4.0
-platformdirs==2.6.2
+pillow==9.5.0
+platformdirs==3.2.0
 pluggy==1.0.0
-pre-commit==3.0.4
+pre-commit==3.2.2
 ptyprocess==0.7.0
 pycodestyle==2.10.0
 pycparser==2.21
 pyflakes==3.0.1
-pygments==2.14.0
-pymdown-extensions==9.9.2
+pygments==2.15.1
+pymdown-extensions==9.11
 pyrsistent==0.19.3
-pytest==7.2.1
+pytest==7.3.1
 pytest-mock==3.10.0
 pytest-plus==0.4.0
 pytest-testinfra==7.0.0
-pytest-xdist==3.1.0
+pytest-xdist==3.2.1
 python-dateutil==2.8.2
-python-slugify==8.0.0
-pytz==2022.7.1
+python-slugify==8.0.1
+pytz==2023.3
 pyyaml==6.0
 pyyaml-env-tag==0.1
-regex==2022.10.31
+regex==2023.3.23
 requests==2.28.2
 resolvelib==0.8.1
-rich==13.3.1
+rich==13.3.4
 ruamel-yaml==0.17.21
 ruamel-yaml-clib==0.2.7
 six==1.16.0
 smmap==5.0.0
 subprocess-tee==0.4.1
 text-unidecode==1.3
 tinycss2==1.2.1
 tomli==2.0.1
-typing-extensions==4.4.0
+typing-extensions==4.5.0
 typing-inspect==0.8.0
-urllib3==1.26.14
-virtualenv==20.18.0
-watchdog==2.2.1
+urllib3==1.26.15
+virtualenv==20.21.0
+watchdog==3.0.0
 wcmatch==8.4.1
 webencodings==0.5.1
-yamllint==1.29.0
-zipp==3.12.1
+yamllint==1.30.0
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `molecule-5.0.0a0/snap/snapcraft.yaml` & `molecule-5.0.0a1/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/__init__.py` & `molecule-5.0.0a1/src/molecule/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,12 +16,11 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Molecule version information."""
 
-from __future__ import absolute_import, division, print_function
 
 from importlib.metadata import version
 
 __version__ = version("molecule")
```

### Comparing `molecule-5.0.0a0/src/molecule/__main__.py` & `molecule-5.0.0a1/src/molecule/__main__.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/api.py` & `molecule-5.0.0a1/src/molecule/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 LOG = logging.getLogger(__name__)
 
 
 class UserListMap(UserList):
     """A list where you can also access elements by their name.
 
     Example:
+    -------
     foo['boo']
     foo.boo
     """
 
     def __getitem__(self, i):
         """Implement indexing."""
         if isinstance(i, int):
-            return super(UserListMap, self).__getitem__(i)
+            return super().__getitem__(i)
         else:
             return self.__dict__[i]
 
     def get(self, key, default):
         return self.__dict__.get(key, default)
 
     def append(self, item) -> None:
         self.__dict__[str(item)] = item
-        super(UserListMap, self).append(item)
+        super().append(item)
 
 
 class MoleculeRuntimeWarning(RuntimeWarning):
     """A runtime warning used by Molecule and its plugins."""
 
 
 class IncompatibleMoleculeRuntimeWarning(MoleculeRuntimeWarning):
```

### Comparing `molecule-5.0.0a0/src/molecule/command/__init__.py` & `molecule-5.0.0a1/src/molecule/command/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# noqa D104
+# D104
 #
 #  Copyright (c) 2015-2018 Cisco Systems, Inc.
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to
 #  deal in the Software without restriction, including without limitation the
 #  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
```

### Comparing `molecule-5.0.0a0/src/molecule/command/base.py` & `molecule-5.0.0a1/src/molecule/command/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,51 +35,48 @@
 from molecule.console import should_do_markup
 
 LOG = logging.getLogger(__name__)
 MOLECULE_GLOB = os.environ.get("MOLECULE_GLOB", "molecule/*/molecule.yml")
 MOLECULE_DEFAULT_SCENARIO_NAME = "default"
 
 
-class Base(object, metaclass=abc.ABCMeta):
+class Base(metaclass=abc.ABCMeta):
     """An abstract base class used to define the command interface."""
 
-    def __init__(self, c: config.Config):
-        """
-        Initialize code for all command classes.
+    def __init__(self, c: config.Config) -> None:
+        """Initialize code for all command classes.
 
         :param c: An instance of a Molecule config.
         :returns: None
         """
         self._config = c
         self._setup()
 
     def __init_subclass__(cls) -> None:
         """Decorate execute from all subclasses."""
         super().__init_subclass__()
         for wrapper in logger.get_section_loggers():
-            setattr(cls, "execute", wrapper(cls.execute))
+            cls.execute = wrapper(cls.execute)  # type: ignore
 
     @abc.abstractmethod
     def execute(self, action_args=None):  # pragma: no cover
         pass
 
     def _setup(self) -> None:
-        """
-        Prepare Molecule's provisioner and returns None.
+        """Prepare Molecule's provisioner and returns None.
 
         :return: None
         """
         self._config.write()
         self._config.provisioner.write_config()
         self._config.provisioner.manage_inventory()
 
 
 def execute_cmdline_scenarios(scenario_name, args, command_args, ansible_args=()):
-    """
-    Execute scenario sequences based on parsed command-line arguments.
+    """Execute scenario sequences based on parsed command-line arguments.
 
     This is useful for subcommands that run scenario sequences, which
     excludes subcommands such as ``list``, ``login``, and ``matrix``.
 
     ``args`` and ``command_args`` are combined using :func:`get_configs`
     to generate the scenario(s) configuration.
 
@@ -90,30 +87,32 @@
     :returns: None
 
     """
     glob_str = MOLECULE_GLOB
     if scenario_name:
         glob_str = glob_str.replace("*", scenario_name)
     scenarios = molecule.scenarios.Scenarios(
-        get_configs(args, command_args, ansible_args, glob_str), scenario_name
+        get_configs(args, command_args, ansible_args, glob_str),
+        scenario_name,
     )
 
     if scenario_name and scenarios:
         LOG.info(
             "%s scenario test matrix: %s",
             scenario_name,
             ", ".join(scenarios.sequence(scenario_name)),
         )
 
     for scenario in scenarios:
         if scenario.config.config["prerun"]:
             role_name_check = scenario.config.config["role_name_check"]
             LOG.info("Performing prerun with role_name_check=%s...", role_name_check)
             scenario.config.runtime.prepare_environment(
-                install_local=True, role_name_check=role_name_check
+                install_local=True,
+                role_name_check=role_name_check,
             )
 
         if command_args.get("subcommand") == "reset":
             LOG.info("Removing %s", scenario.ephemeral_directory)
             shutil.rmtree(scenario.ephemeral_directory)
             return
         try:
@@ -150,16 +149,15 @@
     # and is also used for reporting in execute_cmdline_scenarios
     config.action = subcommand
 
     return command(config).execute(args)
 
 
 def execute_scenario(scenario):
-    """
-    Execute each command in the given scenario's configured sequence.
+    """Execute each command in the given scenario's configured sequence.
 
     :param scenario: The scenario to execute.
     :returns: None
     """
     for action in scenario.sequence:
         execute_subcommand(scenario.config, action)
 
@@ -170,16 +168,15 @@
         scenario.prune()
 
         if scenario.config.is_parallel:
             scenario._remove_scenario_state_directory()
 
 
 def get_configs(args, command_args, ansible_args=(), glob_str=MOLECULE_GLOB):
-    """
-    Glob the current directory for Molecule config files, instantiate config \
+    """Glob the current directory for Molecule config files, instantiate config \
     objects, and returns a list.
 
     :param args: A dict of options, arguments and commands from the CLI.
     :param command_args: A dict of options passed to the subcommand from
      the CLI.
     :param ansible_args: An optional tuple of arguments provided to the
      `ansible-playbook` command.
@@ -196,16 +193,15 @@
     ]
     _verify_configs(configs, glob_str)
 
     return configs
 
 
 def _verify_configs(configs, glob_str=MOLECULE_GLOB):
-    """
-    Verify a Molecule config was found and returns None.
+    """Verify a Molecule config was found and returns None.
 
     :param configs: A list containing absolute paths to Molecule config files.
     :return: None
     """
     if configs:
         scenario_names = [c.scenario.name for c in configs]
         for scenario_name, n in collections.Counter(scenario_names).items():
@@ -248,15 +244,17 @@
         result_callback=result_callback,
     )
 
 
 def click_command_ex() -> Callable[[Callable[..., Any]], click.Command]:
     """Return extended version of click.command()."""
     return click.command(  # type: ignore
-        cls=HelpColorsCommand, help_headers_color="yellow", help_options_color="green"
+        cls=HelpColorsCommand,
+        help_headers_color="yellow",
+        help_options_color="green",
     )
 
 
 def result_callback(*args, **kwargs):
     """Click natural exit callback."""
     # We want to be used we run out custom exit code, regardless if run was
     # a success or failure.
```

### Comparing `molecule-5.0.0a0/src/molecule/command/check.py` & `molecule-5.0.0a1/src/molecule/command/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 MOLECULE_PARALLEL = os.environ.get("MOLECULE_PARALLEL", False)
 
 
 class Check(base.Base):
     """Check Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule check` and \
+        """Execute the actions necessary to perform a `molecule check` and \
         returns None.
 
         :return: None
         """
         self._config.provisioner.check()
 
 
@@ -55,15 +54,16 @@
 @click.option(
     "--parallel/--no-parallel",
     default=MOLECULE_PARALLEL,
     help="Enable or disable parallel mode. Default is disabled.",
 )
 def check(ctx, scenario_name, parallel):  # pragma: no cover
     """Use the provisioner to perform a Dry-Run (destroy, dependency, create, \
-    prepare, converge)."""
+    prepare, converge).
+    """
     args = ctx.obj.get("args")
     subcommand = base._get_subcommand(__name__)
     command_args = {"parallel": parallel, "subcommand": subcommand}
 
     if parallel:
         util.validate_parallel_cmd_args(command_args)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/cleanup.py` & `molecule-5.0.0a1/src/molecule/command/cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 LOG = logging.getLogger(__name__)
 
 
 class Cleanup(base.Base):
     """Cleanup Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to cleanup the instances and returns \
+        """Execute the actions necessary to cleanup the instances and returns \
         None.
 
         :return: None
         """
         if not self._config.provisioner.playbooks.cleanup:
             msg = "Skipping, cleanup playbook not configured."
             LOG.warning(msg)
@@ -52,13 +51,14 @@
     "--scenario-name",
     "-s",
     default=base.MOLECULE_DEFAULT_SCENARIO_NAME,
     help=f"Name of the scenario to target. ({base.MOLECULE_DEFAULT_SCENARIO_NAME})",
 )
 def cleanup(ctx, scenario_name):  # pragma: no cover
     """Use the provisioner to cleanup any changes made to external systems during \
-    the stages of testing."""
+    the stages of testing.
+    """
     args = ctx.obj.get("args")
     subcommand = base._get_subcommand(__name__)
     command_args = {"subcommand": subcommand}
 
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/converge.py` & `molecule-5.0.0a1/src/molecule/command/converge.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 LOG = logging.getLogger(__name__)
 
 
 class Converge(base.Base):
     """Converge Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule converge` and \
+        """Execute the actions necessary to perform a `molecule converge` and \
         returns None.
 
         :return: None
         """
         self._config.provisioner.converge()
         self._config.state.change_state("converged", True)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/create.py` & `molecule-5.0.0a1/src/molecule/command/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 LOG = logging.getLogger(__name__)
 
 
 class Create(base.Base):
     """Create Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule create` and \
+        """Execute the actions necessary to perform a `molecule create` and \
         returns None.
 
         :return: None
         """
         self._config.state.change_state("driver", self._config.driver.name)
 
         if self._config.driver.delegated and not self._config.driver.managed:
```

### Comparing `molecule-5.0.0a0/src/molecule/command/dependency.py` & `molecule-5.0.0a1/src/molecule/command/dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 LOG = logging.getLogger(__name__)
 
 
 class Dependency(base.Base):
     """Dependency Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule dependency` and \
+        """Execute the actions necessary to perform a `molecule dependency` and \
         returns None.
 
         :return: None
         """
         self._config.dependency.execute()
```

### Comparing `molecule-5.0.0a0/src/molecule/command/destroy.py` & `molecule-5.0.0a1/src/molecule/command/destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 MOLECULE_PARALLEL = os.environ.get("MOLECULE_PARALLEL", False)
 
 
 class Destroy(base.Base):
     """Destroy Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule destroy` and \
+        """Execute the actions necessary to perform a `molecule destroy` and \
         returns None.
 
         :return: None
         """
         if self._config.command_args.get("destroy") == "never":
             msg = "Skipping, '--destroy=never' requested."
             LOG.warning(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/drivers.py` & `molecule-5.0.0a1/src/molecule/command/drivers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Create Command Module."""
 
-from __future__ import print_function
 
 import logging
 
 import click
 from rich import box
 from rich.table import Table
 
@@ -55,16 +54,15 @@
     else:
         headers = []
         table_format = format
         _print_tabulate_data(headers, drivers, table_format)
 
 
 def _print_tabulate_data(headers, data, table_format):  # pragma: no cover
-    """
-    Show the tabulate data on the screen and returns None.
+    """Show the tabulate data on the screen and returns None.
 
     :param headers: A list of column headers.
     :param data:  A list of tabular data to display.
     :returns: None
     """
     t = Table(box=box.MINIMAL)
     for header in headers:
```

### Comparing `molecule-5.0.0a0/src/molecule/command/idempotence.py` & `molecule-5.0.0a1/src/molecule/command/idempotence.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,22 @@
 from molecule.command import base
 from molecule.text import strip_ansi_escape
 
 LOG = logging.getLogger(__name__)
 
 
 class Idempotence(base.Base):
-    """
-    Runs the converge step a second time.
+    """Runs the converge step a second time.
 
     If no tasks will be marked as changed \
     the scenario will be considered idempotent.
     """
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule idempotence` and \
+        """Execute the actions necessary to perform a `molecule idempotence` and \
         returns None.
 
         :return: None
         """
         if not self._config.state.converged:
             msg = "Instances not converged.  Please converge instances first."
             util.sysexit_with_message(msg)
@@ -76,16 +74,15 @@
         if changed:
             # Not idempotent
             return False
 
         return True
 
     def _non_idempotent_tasks(self, output):
-        """
-        Parse the output to identify the non idempotent tasks.
+        """Parse the output to identify the non idempotent tasks.
 
         :param (str) output: A string containing the output of the ansible run.
         :return: A list containing the names of the non idempotent tasks.
         """
         # Remove blank lines to make regex matches easier.
         output = re.sub(r"\n\s*\n*", "\n", output)
 
@@ -114,13 +111,14 @@
     "-s",
     default=base.MOLECULE_DEFAULT_SCENARIO_NAME,
     help=f"Name of the scenario to target. ({base.MOLECULE_DEFAULT_SCENARIO_NAME})",
 )
 @click.argument("ansible_args", nargs=-1, type=click.UNPROCESSED)
 def idempotence(ctx, scenario_name, ansible_args):  # pragma: no cover
     """Use the provisioner to configure the instances and parse the output to \
-    determine idempotence."""
+    determine idempotence.
+    """
     args = ctx.obj.get("args")
     subcommand = base._get_subcommand(__name__)
     command_args = {"subcommand": subcommand}
 
     base.execute_cmdline_scenarios(scenario_name, args, command_args, ansible_args)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/init/base.py` & `molecule-5.0.0a1/src/molecule/command/init/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,27 @@
 import cookiecutter.main
 
 from molecule import util
 
 LOG = logging.getLogger(__name__)
 
 
-class Base(object):
+class Base:
     """Init Command Base Class."""
 
     __metaclass__ = abc.ABCMeta
 
     def _process_templates(
-        self, template_dir, extra_context, output_dir, overwrite=True
+        self,
+        template_dir,
+        extra_context,
+        output_dir,
+        overwrite=True,
     ):
-        """
-        Process templates as found in the named directory.
+        """Process templates as found in the named directory.
 
         :param template_dir: A string containing an absolute or relative path
          to a directory where the templates are located. If the provided
          directory is a relative path, it is resolved using a known location.
         :param extra_context: A dict of values that are used to override
          default or user specified values.
         :param output_dir: An string with an absolute path to a directory where
@@ -64,31 +67,31 @@
                 overwrite_if_exists=overwrite,
                 no_input=True,
             )
         except cookiecutter.exceptions.NonTemplatedInputDirException:
             util.sysexit_with_message(
                 "The specified template directory ("
                 + str(template_dir)
-                + ") is in an invalid format"
+                + ") is in an invalid format",
             )
 
     def _resolve_template_dir(self, template_dir):
         if not os.path.isabs(template_dir):
             template_dir = os.path.abspath(
                 os.path.join(
                     os.path.dirname(__file__),
                     os.path.pardir,
                     os.path.pardir,
                     "cookiecutter",
                     template_dir,
-                )
+                ),
             )
 
         return template_dir
 
     def _validate_template_dir(self, template_dir):
         if not os.path.isdir(template_dir):
             util.sysexit_with_message(
                 "The specified template directory ("
                 + str(template_dir)
-                + ") does not exist"
+                + ") does not exist",
             )
```

### Comparing `molecule-5.0.0a0/src/molecule/command/init/init.py` & `molecule-5.0.0a1/src/molecule/command/init/init.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/command/init/role.py` & `molecule-5.0.0a1/src/molecule/command/init/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,35 +30,33 @@
 from molecule.command.init import base
 from molecule.config import DEFAULT_DRIVER
 
 LOG = logging.getLogger(__name__)
 
 
 class Role(base.Base):
-    """
-    Init Role Command Class.
+    """Init Role Command Class.
 
     .. program:: molecule init role acme.foo
 
     .. option:: molecule init role acme.foo
 
         Initialize a new role.
 
         Initialize a new role using ansible-galaxy and include default
         molecule directory. Please refer to the ``init scenario``
         command in order to generate a custom ``molecule`` scenario.
     """
 
-    def __init__(self, command_args):
+    def __init__(self, command_args) -> None:
         """Construct Role."""
         self._command_args = command_args
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule init role` and \
+        """Execute the actions necessary to perform a `molecule init role` and \
         returns None.
 
         :return: None
         """
         namespace = None
         role_name = self._command_args["role_name"]
         role_directory = os.getcwd()
@@ -67,15 +65,15 @@
         if not os.path.isfile("../galaxy.yml"):
             name_re = re.compile(r"^[a-z][a-z0-9_]+\.[a-z][a-z0-9_]+$")
 
             if not name_re.match(role_name):
                 util.sysexit_with_message(
                     "Outside collections you must mention role "
                     "namespace like: molecule init role 'acme.myrole'. Be sure "
-                    "you use only lowercase characters and underlines. See https://galaxy.ansible.com/docs/contributing/creating_role.html"
+                    "you use only lowercase characters and underlines. See https://galaxy.ansible.com/docs/contributing/creating_role.html",
                 )
             namespace, role_name = role_name.split(".")
 
         msg = f"Initializing new role {role_name}..."
         LOG.info(msg)
 
         if os.path.isdir(role_name):
@@ -83,15 +81,15 @@
             util.sysexit_with_message(msg)
 
         cmd = ["ansible-galaxy", "init", "-v", "--offline", role_name]
         result = util.run_command(cmd)
 
         if result.returncode != 0:
             util.sysexit_with_message(
-                f"Galaxy failed to create role, returned {result.returncode!s}"
+                f"Galaxy failed to create role, returned {result.returncode!s}",
             )
 
         if namespace:
             # we need to inject namespace info into meta/main.yml
             cmd = [
                 "ansible",
                 "localhost",
@@ -105,19 +103,23 @@
 
         scenario_base_directory = os.path.join(role_directory, role_name)
         templates = [
             api.drivers()[self._command_args["driver_name"]].template_dir(),
             api.verifiers()[self._command_args["verifier_name"]].template_dir(),
         ]
         self._process_templates(
-            "molecule", {**self._command_args, "role_name": role_name}, role_directory
+            "molecule",
+            {**self._command_args, "role_name": role_name},
+            role_directory,
         )
         for template in templates:
             self._process_templates(
-                template, self._command_args, scenario_base_directory
+                template,
+                self._command_args,
+                scenario_base_directory,
             )
 
         role_directory = os.path.join(role_directory, role_name)
         msg = f"Initialized role in {role_directory} successfully."
         LOG.info(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/init/scenario.py` & `molecule-5.0.0a1/src/molecule/command/init/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Base class used by init scenario command."""
 
 import logging
 import os
-from typing import Dict
 
 import click
 
 from molecule import api, config, util
 from molecule.command import base as command_base
 from molecule.command.init import base
 from molecule.config import DEFAULT_DRIVER
@@ -52,35 +51,34 @@
 
     .. program:: cd foo; molecule init scenario bar --role-name foo
 
     .. option:: cd foo; molecule init scenario bar --role-name foo
 
         Initialize a new scenario using a local *cookiecutter* template for the
         driver configuration.
-    """  # noqa
+    """
 
-    def __init__(self, command_args: Dict[str, str]):
+    def __init__(self, command_args: dict[str, str]) -> None:
         """Construct Scenario."""
         self._command_args = command_args
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule init scenario` and \
+        """Execute the actions necessary to perform a `molecule init scenario` and \
         returns None.
 
         :return: None
         """
         scenario_name = self._command_args["scenario_name"]
         role_name = os.getcwd().split(os.sep)[-1]
         role_directory = util.abs_path(os.path.join(os.getcwd(), os.pardir))
 
         msg = f"Initializing new scenario {scenario_name}..."
         LOG.info(msg)
         molecule_directory = config.molecule_directory(
-            os.path.join(role_directory, role_name)
+            os.path.join(role_directory, role_name),
         )
         scenario_directory = os.path.join(molecule_directory, scenario_name)
 
         if os.path.isdir(scenario_directory):
             msg = (
                 f"The directory molecule/{scenario_name} exists. "
                 "Cannot create new scenario."
@@ -105,15 +103,17 @@
         templates = [
             driver_template,
             api.verifiers()[self._command_args["verifier_name"]].template_dir(),
         ]
         self._process_templates("molecule", self._command_args, role_directory)
         for template in templates:
             self._process_templates(
-                template, self._command_args, scenario_base_directory
+                template,
+                self._command_args,
+                scenario_base_directory,
             )
 
         role_directory = os.path.join(role_directory, role_name)
         msg = f"Initialized scenario in {scenario_directory} successfully."
         LOG.info(msg)
 
 
@@ -131,15 +131,16 @@
 
 
 def _default_scenario_exists(ctx, param, value: str):  # pragma: no cover
     if value == command_base.MOLECULE_DEFAULT_SCENARIO_NAME:
         return value
 
     default_scenario_directory = os.path.join(
-        "molecule", command_base.MOLECULE_DEFAULT_SCENARIO_NAME
+        "molecule",
+        command_base.MOLECULE_DEFAULT_SCENARIO_NAME,
     )
     if not os.path.exists(default_scenario_directory):
         msg = f"The default scenario not found.  Please create a scenario named '{command_base.MOLECULE_DEFAULT_SCENARIO_NAME}' first."
         util.sysexit_with_message(msg)
     return value
```

### Comparing `molecule-5.0.0a0/src/molecule/command/list.py` & `molecule-5.0.0a1/src/molecule/command/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """List Command Module."""
 
-from __future__ import print_function
 
 import logging
 
 import click
 from rich import box
 from rich.syntax import Syntax
 from rich.table import Table
@@ -36,16 +35,15 @@
 LOG = logging.getLogger(__name__)
 
 
 class List(base.Base):
     """List command shows information about current scenarios."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule list` and \
+        """Execute the actions necessary to perform a `molecule list` and \
         returns None.
 
         :return: None
         """
         return self._config.driver.status()
 
 
@@ -79,16 +77,15 @@
             table_format = format
         _print_tabulate_data(headers, statuses, table_format)
     else:
         _print_yaml_data(headers, statuses)
 
 
 def _print_tabulate_data(headers, data, table_format):  # pragma: no cover
-    """
-    Show the tabulate data on the screen and returns None.
+    """Show the tabulate data on the screen and returns None.
 
     :param headers: A list of column headers.
     :param data:  A list of tabular data to display.
     :returns: None
     """
     if table_format == "plain":
         for line in data:
```

### Comparing `molecule-5.0.0a0/src/molecule/command/login.py` & `molecule-5.0.0a1/src/molecule/command/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,21 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class Login(base.Base):
     """Login Command Class."""
 
-    def __init__(self, c):
+    def __init__(self, c) -> None:
         """Construct Login."""
-        super(Login, self).__init__(c)
+        super().__init__(c)
         self._pt = None
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule login` and \
+        """Execute the actions necessary to perform a `molecule login` and \
         returns None.
 
         :return: None
         """
         c = self._config
         if (not c.state.created) and c.driver.managed:
             msg = "Instances not created.  Please create instances first."
```

### Comparing `molecule-5.0.0a0/src/molecule/command/matrix.py` & `molecule-5.0.0a1/src/molecule/command/matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 from molecule import scenarios
 from molecule.command import base
 
 LOG = logging.getLogger(__name__)
 
 
 class Matrix(base.Base):
-    """
-    Matric Command Class.
+    """Matric Command Class.
 
     .. program:: molecule matrix subcommand
 
     .. option:: molecule matrix subcommand
 
         Target the default scenario.
```

### Comparing `molecule-5.0.0a0/src/molecule/command/prepare.py` & `molecule-5.0.0a1/src/molecule/command/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 from molecule.command import base
 from molecule.config import DEFAULT_DRIVER
 
 LOG = logging.getLogger(__name__)
 
 
 class Prepare(base.Base):
-    """
-    This action is for the purpose of preparing a molecule managed instance \
+    """This action is for the purpose of preparing a molecule managed instance \
     before the :py:class:`molecule.command.converge.Converge` action is run.
 
     Tasks contained within the ``prepare.yml`` playbook in the scenario
     directory will be run remotely on the managed instance. This action is run
     only once per test sequence.
 
     .. program:: molecule prepare
@@ -80,16 +79,15 @@
     .. option:: molecule --env-file foo.yml prepare
 
         Load an env file to read variables from when rendering
         molecule.yml.
     """
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to prepare the instances and returns \
+        """Execute the actions necessary to prepare the instances and returns \
         None.
 
         :return: None
         """
         if self._config.state.prepared and not self._config.command_args.get("force"):
             msg = "Skipping, instances already prepared."
             LOG.warning(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/reset.py` & `molecule-5.0.0a1/src/molecule/command/reset.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/command/side_effect.py` & `molecule-5.0.0a1/src/molecule/command/side_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,21 @@
 
 from molecule.command import base
 
 LOG = logging.getLogger(__name__)
 
 
 class SideEffect(base.Base):
-    """
-    This action has side effects and not enabled by default.
+    """This action has side effects and not enabled by default.
 
     See the provisioners documentation for further details.
     """
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule side-effect` and \
+        """Execute the actions necessary to perform a `molecule side-effect` and \
         returns None.
 
         :return: None
         """
         if not self._config.provisioner.playbooks.side_effect:
             msg = "Skipping, side effect playbook not configured."
             LOG.warning(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/command/syntax.py` & `molecule-5.0.0a1/src/molecule/command/syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/command/test.py` & `molecule-5.0.0a1/src/molecule/command/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 MOLECULE_PLATFORM_NAME = os.environ.get("MOLECULE_PLATFORM_NAME", None)
 
 
 class Test(base.Base):
     """Test Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule test` and \
+        """Execute the actions necessary to perform a `molecule test` and \
         returns None.
 
         :return: None
         """
 
 
 @base.click_command_ex()
```

### Comparing `molecule-5.0.0a0/src/molecule/command/verify.py` & `molecule-5.0.0a1/src/molecule/command/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 LOG = logging.getLogger(__name__)
 
 
 class Verify(base.Base):
     """Verify Command Class."""
 
     def execute(self, action_args=None):
-        """
-        Execute the actions necessary to perform a `molecule verify` and \
+        """Execute the actions necessary to perform a `molecule verify` and \
         returns None.
 
         :return: None
         """
         self._config.verifier.execute(action_args)
```

### Comparing `molecule-5.0.0a0/src/molecule/config.py` & `molecule-5.0.0a1/src/molecule/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  DEALINGS IN THE SOFTWARE.
 """Config Module."""
 
 import copy
 import logging
 import os
 import warnings
-from typing import MutableMapping
+from collections.abc import MutableMapping
 from uuid import uuid4
 
 from ansible_compat.ports import cache, cached_property
 from packaging.version import Version
 
 from molecule import api, interpolation, platforms, scenario, state, util
 from molecule.app import app
@@ -51,27 +51,26 @@
     warnings.warn(
         "molecule.config.ansible_version is deprecated, will be removed in the future.",
         category=DeprecationWarning,
     )
     return app.runtime.version
 
 
-# https://stackoverflow.com/questions/16017397/injecting-function-call-after-init-with-decorator  # noqa
+# https://stackoverflow.com/questions/16017397/injecting-function-call-after-init-with-decorator
 class NewInitCaller(type):
     """NewInitCaller."""
 
     def __call__(cls, *args, **kwargs):
         obj = type.__call__(cls, *args, **kwargs)
         obj.after_init()
         return obj
 
 
-class Config(object, metaclass=NewInitCaller):
-    """
-    Config Class.
+class Config(metaclass=NewInitCaller):
+    """Config Class.
 
     Molecule searches the current directory for ``molecule.yml`` files by
     globbing `molecule/*/molecule.yml`.  The files are instantiated into
     a list of Molecule [molecule.config.Config][] objects, and each Molecule subcommand
     operates on this list.
 
     The directory in which the ``molecule.yml`` resides is the Scenario's
@@ -80,17 +79,22 @@
     The [molecule.config.Config][] object instantiates Dependency, Driver,
     Platforms, Provisioner, Verifier_,
     [scenario][], and State_ references.
     """
 
     # pylint: disable=too-many-instance-attributes
     # Config objects should be allowed to have any number of attributes
-    def __init__(self, molecule_file: str, args={}, command_args={}, ansible_args=()):
-        """
-        Initialize a new config class and returns None.
+    def __init__(
+        self,
+        molecule_file: str,
+        args={},
+        command_args={},
+        ansible_args=(),
+    ) -> None:
+        """Initialize a new config class and returns None.
 
         :param molecule_file: A string containing the path to the Molecule file
          to be parsed.
         :param args: An optional dict of options, arguments and commands from
          the CLI.
         :param command_args: An optional dict of options passed to the
          subcommand from the CLI.
@@ -212,14 +216,15 @@
         )
 
     @cached_property
     def provisioner(self):
         provisioner_name = self.config["provisioner"]["name"]
         if provisioner_name == "ansible":
             return ansible.Ansible(self)
+        return None
 
     @cached_property
     def scenario(self):
         return scenario.Scenario(self)
 
     @cached_property
     def state(self):
@@ -229,15 +234,15 @@
             modTime = os.path.getmtime(self.molecule_file)
             if myState.molecule_yml_date_modified is None:
                 myState.change_state("molecule_yml_date_modified", modTime)
             elif myState.molecule_yml_date_modified != modTime:
                 LOG.warning(
                     f"The scenario config file ('{self.molecule_file}') has been modified since the scenario was created. "
                     + "If recent changes are important, reset the scenario with 'molecule destroy' to clean up created items or "
-                    + "'molecule reset' to clear current configuration."
+                    + "'molecule reset' to clear current configuration.",
                 )
         return state.State(self)
 
     @cached_property
     def verifier(self):
         return api.verifiers(self).get(self.config["verifier"]["name"], None)
 
@@ -277,41 +282,38 @@
                 "To change drivers, run 'molecule destroy' for converged scenarios or 'molecule reset' otherwise."
             )
             LOG.warning(msg)
 
         return driver_name
 
     def _get_config(self) -> MutableMapping:
-        """
-        Perform a prioritized recursive merge of config files.
+        """Perform a prioritized recursive merge of config files.
 
         Returns a new dict.  Prior to merging the config files are interpolated with
         environment variables.
 
         :return: dict
         """
         return self._combine(keep_string=MOLECULE_KEEP_STRING)
 
     def _reget_config(self):
-        """
-        Perform the same prioritized recursive merge from `get_config`.
+        """Perform the same prioritized recursive merge from `get_config`.
 
         Interpolates the ``keep_string`` left behind in the original
         ``get_config`` call.  This is probably __very__ bad.
 
         :return: dict
         """
         env = util.merge_dicts(os.environ, self.env)
         env = set_env_from_file(env, self.env_file)
 
         return self._combine(env=env)
 
     def _combine(self, env=os.environ, keep_string=None) -> MutableMapping:
-        """
-        Perform a prioritized recursive merge of config files.
+        """Perform a prioritized recursive merge of config files.
 
         Returns a new dict.  Prior to merging the config files are interpolated with
         environment variables.
 
         1. Loads Molecule defaults.
         2. Loads a base config (if provided) and merges on top of defaults.
         3. Loads the scenario's ``molecule file`` and merges on top of previous
@@ -322,23 +324,25 @@
         defaults = self._get_defaults()
         base_configs = filter(os.path.exists, self.args.get("base_config", []))
         for base_config in base_configs:
             with util.open_file(base_config) as stream:
                 s = stream.read()
                 interpolated_config = self._interpolate(s, env, keep_string)
                 defaults = util.merge_dicts(
-                    defaults, util.safe_load(interpolated_config)
+                    defaults,
+                    util.safe_load(interpolated_config),
                 )
 
         if self.molecule_file:
             with util.open_file(self.molecule_file) as stream:
                 s = stream.read()
                 interpolated_config = self._interpolate(s, env, keep_string)
                 defaults = util.merge_dicts(
-                    defaults, util.safe_load(interpolated_config)
+                    defaults,
+                    util.safe_load(interpolated_config),
                 )
 
         return defaults
 
     def _interpolate(self, stream: str, env: MutableMapping, keep_string: str) -> str:
         env = set_env_from_file(env, self.env_file)
```

### Comparing `molecule-5.0.0a0/src/molecule/console.py` & `molecule-5.0.0a1/src/molecule/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Console and terminal utilities."""
 import os
 import sys
-from typing import Any, Dict
+from typing import Any
 
 from enrich.console import Console
 from rich.style import Style
 from rich.theme import Theme
 
 theme = Theme(
     {
@@ -18,15 +18,15 @@
         "logging.level.notset": Style(dim=True),
         "logging.level.debug": Style(color="white", dim=True),
         "logging.level.info": Style(color="blue"),
         "logging.level.warning": Style(color="red"),
         "logging.level.error": Style(color="red", bold=True),
         "logging.level.critical": Style(color="red", bold=True),
         "logging.level.success": Style(color="green", bold=True),
-    }
+    },
 )
 
 
 # Based on Ansible implementation
 def to_bool(a: Any) -> bool:
     """Return a bool for the arg."""
     if a is None or isinstance(a, bool):
@@ -67,18 +67,21 @@
     # Use tty detection logic as last resort because there are numerous
     # factors that can make isatty return a misleading value, including:
     # - stdin.isatty() is the only one returning true, even on a real terminal
     # - stderr returting false if user user uses a error stream coloring solution
     return sys.stdout.isatty()
 
 
-console_options: Dict[str, Any] = {"emoji": False, "theme": theme, "soft_wrap": True}
+console_options: dict[str, Any] = {"emoji": False, "theme": theme, "soft_wrap": True}
 
 console = Console(
-    force_terminal=should_do_markup(), theme=theme, record=True, redirect=True
+    force_terminal=should_do_markup(),
+    theme=theme,
+    record=True,
+    redirect=True,
 )
 console_options_stderr = console_options.copy()
 console_options_stderr["stderr"] = True
 console_stderr: Console = Console(**console_options_stderr)
 
 # Define ANSIBLE_FORCE_COLOR if markup is enabled and another value is not
 # already given. This assures that Ansible subprocesses are still colored,
```

### Comparing `molecule-5.0.0a0/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint` & `molecule-5.0.0a1/src/molecule/cookiecutter/molecule/{{cookiecutter.role_name}}/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-5.0.0a1/src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py` & `molecule-5.0.0a1/src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """PyTest Fixtures."""
-from __future__ import absolute_import
 
 import os
 
 import pytest
 
 
 def pytest_runtest_setup(item):
     """Run tests only when under molecule with testinfra installed."""
     try:
         import testinfra
     except ImportError:
         pytest.skip("Test requires testinfra", allow_module_level=True)
     if "MOLECULE_INVENTORY_FILE" in os.environ:
         pytest.testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-            os.environ["MOLECULE_INVENTORY_FILE"]
+            os.environ["MOLECULE_INVENTORY_FILE"],
         ).get_hosts("all")
     else:
         pytest.skip(
-            "Test should run only from inside molecule.", allow_module_level=True
+            "Test should run only from inside molecule.",
+            allow_module_level=True,
         )
```

### Comparing `molecule-5.0.0a0/src/molecule/data/molecule.json` & `molecule-5.0.0a1/src/molecule/data/molecule.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990325261158595%*

 * *Differences: {"'$defs'": "{'MoleculeDriverModel': {'additionalProperties': True, 'properties': {delete: "*

 * *            "['cachier', 'default_box', 'options', 'parallel', 'provider', 'provision', "*

 * *            "'safe_files', 'ssh_connection_options']}}}",*

 * * "'properties'": "{'platforms': {'items': {replace: OrderedDict([('type', 'object')])}}}"}*

```diff
@@ -86,24 +86,16 @@
                 }
             },
             "title": "MoleculeDependencyModel",
             "type": "object",
             "unevaluatedProperties": false
         },
         "MoleculeDriverModel": {
-            "additionalProperties": false,
+            "additionalProperties": true,
             "properties": {
-                "cachier": {
-                    "title": "Cachier",
-                    "type": "string"
-                },
-                "default_box": {
-                    "title": "DefaultBox",
-                    "type": "string"
-                },
                 "name": {
                     "anyOf": [
                         {
                             "enum": [
                                 "azure",
                                 "ec2",
                                 "delegated",
@@ -128,43 +120,14 @@
                         }
                     ],
                     "messages": {
                         "anyOf": "is not one of ['azure', 'ec2', 'delegated', 'docker', 'containers', 'openstack', 'podman', 'vagrant', 'digitalocean', 'gce', 'libvirt', 'lxd', 'molecule-*', 'molecule_*', 'custom-*', 'custom_*']"
                     },
                     "title": "Name",
                     "type": "string"
-                },
-                "options": {
-                    "$ref": "#/$defs/MoleculeDriverOptionsModel"
-                },
-                "parallel": {
-                    "title": "Parallel",
-                    "type": "boolean"
-                },
-                "provider": {
-                    "title": "Provider",
-                    "type": "object"
-                },
-                "provision": {
-                    "title": "Provision",
-                    "type": "boolean"
-                },
-                "safe_files": {
-                    "items": {
-                        "type": "string"
-                    },
-                    "title": "SafeFiles",
-                    "type": "array"
-                },
-                "ssh_connection_options": {
-                    "items": {
-                        "type": "string"
-                    },
-                    "title": "SshConnectionOptions",
-                    "type": "array"
                 }
             },
             "title": "MoleculeDriverModel",
             "type": "object"
         },
         "MoleculeDriverOptionsModel": {
             "additionalProperties": false,
@@ -627,15 +590,15 @@
         "log": {
             "default": true,
             "title": "Log",
             "type": "boolean"
         },
         "platforms": {
             "items": {
-                "$ref": "#/$defs/MoleculePlatformModel"
+                "type": "object"
             },
             "title": "Platforms",
             "type": "array"
         },
         "prerun": {
             "title": "Prerun",
             "type": "boolean"
```

### Comparing `molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/__init__.py` & `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from molecule import util
 from molecule.dependency.ansible_galaxy.collections import Collections
 from molecule.dependency.ansible_galaxy.roles import Roles
 from molecule.dependency.base import Base
 
 
 class AnsibleGalaxy(Base):
-    """
-    Galaxy is the default dependency manager.
+    """Galaxy is the default dependency manager.
 
     Additional options can be passed to ``ansible-galaxy install`` through the
     options dict.  Any option set in this section will override the defaults.
 
     !!! note
 
         Molecule will remove any options matching '^[v]+$', and pass ``-vvv``
@@ -59,19 +58,20 @@
     Environment variables can be passed to the dependency.
 
     ``` yaml
         dependency:
           name: galaxy
           env:
             FOO: bar
+    ```
     """
 
-    def __init__(self, config):
+    def __init__(self, config) -> None:
         """Construct AnsibleGalaxy."""
-        super(AnsibleGalaxy, self).__init__(config)
+        super().__init__(config)
         self.invocations = [Roles(config), Collections(config)]
 
     def execute(self, action_args=None):
         for invoker in self.invocations:
             invoker.execute()
 
     def _has_requirements_file(self):
```

### Comparing `molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/base.py` & `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,54 +33,53 @@
 class AnsibleGalaxyBase(base.Base):
     """Ansible Galaxy dependency base class."""
 
     __metaclass__ = abc.ABCMeta
 
     FILTER_OPTS = ()
 
-    def __init__(self, config):
+    def __init__(self, config) -> None:
         """Construct AnsibleGalaxy."""
-        super(AnsibleGalaxyBase, self).__init__(config)
+        super().__init__(config)
         self._sh_command = None
 
         self.command = "ansible-galaxy"
 
     @property
     @abc.abstractmethod
-    def install_path(self):  # noqa cover
+    def install_path(self):  # cover
         pass
 
     @property
     @abc.abstractmethod
-    def requirements_file(self):  # noqa cover
+    def requirements_file(self):  # cover
         pass
 
     @property
     def default_options(self):
         d = {
             "force": True,
         }
         if self._config.debug:
             d["vvv"] = True
 
         return d
 
     def filter_options(self, opts, keys):
-        """
-        Filter certain keys from a dictionary.
+        """Filter certain keys from a dictionary.
 
         Removes all the values of ``keys`` from the dictionary ``opts``, if
         they are present. Returns the resulting dictionary. Does not modify the
         existing one.
 
         :return: A copy of ``opts`` without the value of keys
         """
         c = copy.copy(opts)
         for key in keys:
-            if key in c.keys():
+            if key in c:
                 del c[key]
         return c
 
     # NOTE(retr0h): Override the base classes' options() to handle
     # ``ansible-galaxy`` one-off.
     @property
     def options(self):
@@ -94,16 +93,15 @@
         return self.filter_options(o, self.FILTER_OPTS)
 
     @property
     def default_env(self):
         return util.merge_dicts(os.environ, self._config.env)
 
     def bake(self):
-        """
-        Bake an ``ansible-galaxy`` command so it's ready to execute and returns \
+        """Bake an ``ansible-galaxy`` command so it's ready to execute and returns \
         None.
 
         :return: None
         """
         options = self.options
         verbose_flag = util.verbose_flag(options)
 
@@ -127,16 +125,15 @@
         if self._sh_command is None:
             self.bake()
 
         self._setup()
         self.execute_with_retries()
 
     def _setup(self):
-        """
-        Prepare the system for using ``ansible-galaxy`` and returns None.
+        """Prepare the system for using ``ansible-galaxy`` and returns None.
 
         :return: None
         """
         if not os.path.isdir(self.install_path):
             os.makedirs(self.install_path, exist_ok=True)
 
     def _has_requirements_file(self):
```

### Comparing `molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/collections.py` & `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,34 +12,37 @@
     """Collection-specific Ansible Galaxy dependency handling."""
 
     FILTER_OPTS = ("role-file", "roles-path")  # type: ignore
     COMMANDS = ("collection", "install")
 
     @property
     def default_options(self):
-        general = super(Collections, self).default_options
+        general = super().default_options
         specific = util.merge_dicts(
             general,
             {
                 "requirements-file": os.path.join(
-                    self._config.scenario.directory, "collections.yml"
+                    self._config.scenario.directory,
+                    "collections.yml",
                 ),
                 "collections-path": os.path.join(
-                    self._config.scenario.ephemeral_directory, "collections"
+                    self._config.scenario.ephemeral_directory,
+                    "collections",
                 ),
             },
         )
 
         return specific
 
     @property
     def default_env(self):
-        general = super(Collections, self).default_env
+        general = super().default_env
         return util.merge_dicts(
-            general, {self._config.ansible_collections_path: self.install_path}
+            general,
+            {self._config.ansible_collections_path: self.install_path},
         )
 
     @property
     def install_path(self):
         return self.options["collections-path"]
 
     @property
```

### Comparing `molecule-5.0.0a0/src/molecule/dependency/ansible_galaxy/roles.py` & `molecule-5.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,25 @@
     """Role-specific Ansible Galaxy dependency handling."""
 
     FILTER_OPTS = ("requirements-file", "collections-path")  # type: ignore
     COMMANDS = ("install",)
 
     @property
     def default_options(self):
-        general = super(Roles, self).default_options
+        general = super().default_options
         specific = util.merge_dicts(
             general,
             {
                 "role-file": os.path.join(
-                    self._config.scenario.directory, "requirements.yml"
+                    self._config.scenario.directory,
+                    "requirements.yml",
                 ),
                 "roles-path": os.path.join(
-                    self._config.scenario.ephemeral_directory, "roles"
+                    self._config.scenario.ephemeral_directory,
+                    "roles",
                 ),
             },
         )
         return specific
 
     @property
     def install_path(self):
```

### Comparing `molecule-5.0.0a0/src/molecule/dependency/base.py` & `molecule-5.0.0a1/src/molecule/dependency/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,36 @@
 from subprocess import CalledProcessError
 
 from molecule import util
 
 LOG = logging.getLogger(__name__)
 
 
-class Base(object):
+class Base:
     """Dependency Base Class."""
 
     __metaclass__ = abc.ABCMeta
 
     RETRY = 3
     SLEEP = 3
     BACKOFF = 3
 
-    def __init__(self, config):
-        """
-        Initialize code for all :ref:`Dependency` classes.
+    def __init__(self, config) -> None:
+        """Initialize code for all :ref:`Dependency` classes.
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
 
     def execute_with_retries(self):
         """Run dependency downloads with retry and timed back-off."""
         exception = None
 
         try:
-            # print(555, self._sh_command)
             util.run_command(self._sh_command, debug=self._config.debug, check=True)
             msg = "Dependency completed successfully."
             LOG.info(msg)
             return
         except CalledProcessError:
             pass
 
@@ -79,58 +77,56 @@
                 exception = _exception
 
         LOG.error(str(exception))
         util.sysexit(exception.returncode)
 
     @abc.abstractmethod
     def execute(self, action_args=None):  # pragma: no cover
-        """
-        Execute ``cmd`` and returns None.
+        """Execute ``cmd`` and returns None.
 
         :return: None
         """
         for name, version in self._config.driver.required_collections.items():
             self._config.runtime.require_collection(name, version)
 
     @property
     @abc.abstractmethod
     def default_options(self):  # pragma: no cover
-        """
-        Get default CLI arguments provided to ``cmd`` as a dict.
+        """Get default CLI arguments provided to ``cmd`` as a dict.
 
         :return: dict
         """
 
     @property
     def default_env(self):  # pragma: no cover
-        """
-        Get default env variables provided to ``cmd`` as a dict.
+        """Get default env variables provided to ``cmd`` as a dict.
 
         :return: dict
         """
         env = util.merge_dicts(os.environ, self._config.env)
         return env
 
     @property
     def name(self):
-        """
-        Name of the dependency and returns a string.
+        """Name of the dependency and returns a string.
 
         :returns: str
         """
         return self._config.config["dependency"]["name"]
 
     @property
     def enabled(self):
         return self._config.config["dependency"]["enabled"]
 
     @property
     def options(self):
         return util.merge_dicts(
-            self.default_options, self._config.config["dependency"]["options"]
+            self.default_options,
+            self._config.config["dependency"]["options"],
         )
 
     @property
     def env(self):
         return util.merge_dicts(
-            self.default_env, self._config.config["dependency"]["env"]
+            self.default_env,
+            self._config.config["dependency"]["env"],
         )
```

### Comparing `molecule-5.0.0a0/src/molecule/dependency/shell.py` & `molecule-5.0.0a1/src/molecule/dependency/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 from molecule.dependency import base
 from molecule.util import BakedCommand
 
 LOG = logging.getLogger(__name__)
 
 
 class Shell(base.Base):
-    """
-    ``Shell`` is an alternate dependency manager.
+    """``Shell`` is an alternate dependency manager.
 
     It is intended to run a command in situations where `Ansible Galaxy`_
     don't suffice.
 
     The ``command`` to execute is required, and is relative to Molecule's
     project directory when referencing a script not in $PATH.
 
@@ -64,32 +63,32 @@
           name: shell
           command: path/to/command --flag1 subcommand --flag2
           env:
             FOO: bar
     ```
     """
 
-    def __init__(self, config):
+    def __init__(self, config) -> None:
         """Construct Shell."""
-        super(Shell, self).__init__(config)
+        super().__init__(config)
         self._sh_command = None
 
         # self.command = config..config['dependency']['command']
 
     @property
     def command(self):
         return self._config.config["dependency"]["command"]
 
     @property
     def default_options(self):
         return {}
 
     def bake(self) -> None:
         """Bake a ``shell`` command so it's ready to execute."""
-        self._sh_command = BakedCommand(cmd=self.command, env=self.env)
+        self._sh_command = BakedCommand(cmd=self.command, env=self.env)  # type: ignore
 
     def execute(self, action_args=None):
         if not self.enabled:
             msg = "Skipping, dependency is disabled."
             LOG.warning(msg)
             return
         super().execute()
```

### Comparing `molecule-5.0.0a0/src/molecule/driver/base.py` & `molecule-5.0.0a1/src/molecule/driver/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,117 +18,106 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Base Driver Module."""
 
 import inspect
 import os
 from abc import ABCMeta, abstractmethod
-from typing import Dict
 
 import molecule
 from molecule.status import Status
 
 
-class Driver(object):
+class Driver:
     """Driver Class."""
 
     __metaclass__ = ABCMeta
 
-    def __init__(self, config=None):
-        """
-        Initialize code for all :ref:`Driver` classes.
+    def __init__(self, config=None) -> None:
+        """Initialize code for all :ref:`Driver` classes.
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
         self._path = os.path.abspath(os.path.dirname(inspect.getfile(self.__class__)))
         self.module = self.__module__.split(".", maxsplit=1)[0]
         self.version = molecule.version(self.module)
 
     @property
     @abstractmethod
     def name(self) -> str:  # pragma: no cover
-        """
-        Name of the driver and returns a string.
+        """Name of the driver and returns a string.
 
         :returns: str
         """
 
     @name.setter  # type: ignore
     def name(self, value):  # pragma: no cover
-        """
-        Driver name setter and returns None.
+        """Driver name setter and returns None.
 
         :returns: None
         """
 
     @property
     def testinfra_options(self):
-        """
-        Testinfra specific options and returns a dict.
+        """Testinfra specific options and returns a dict.
 
         :returns: dict
         """
         return {
             "connection": "ansible",
             "ansible-inventory": self._config.provisioner.inventory_directory,
         }
 
     @property
     @abstractmethod
     def login_cmd_template(self):  # pragma: no cover
-        """
-        Get the login command template to be populated by ``login_options`` as \
+        """Get the login command template to be populated by ``login_options`` as \
         a string.
 
         :returns: str
         """
 
     @property
     @abstractmethod
     def default_ssh_connection_options(self):  # pragma: no cover
-        """
-        SSH client options and returns a list.
+        """SSH client options and returns a list.
 
         :returns: list
         """
 
     @property
     @abstractmethod
     def default_safe_files(self):  # pragma: no cover
-        """
-        Generate files to be preserved.
+        """Generate files to be preserved.
 
         :returns: list
         """
 
     @abstractmethod
     def login_options(self, instance_name):  # pragma: no cover
-        """
-        Options used in the login command and returns a dict.
+        """Options used in the login command and returns a dict.
 
         :param instance_name: A string containing the instance to login to.
         :returns: dict
         """
 
     @abstractmethod
     def ansible_connection_options(self, instance_name):  # pragma: no cover
-        """
-        Ansible specific connection options supplied to inventory and returns a \
+        """Ansible specific connection options supplied to inventory and returns a \
         dict.
 
         :param instance_name: A string containing the instance to login to.
         :returns: dict
         """
 
     @abstractmethod
     def sanity_checks(self):
-        """
-        Confirm that driver is usable.
+        """Confirm that driver is usable.
 
         Sanity checks to ensure the driver can do work successfully. For
         example, when using the Docker driver, we want to know that the Docker
         daemon is running and we have the correct Docker Python dependency.
         Each driver implementation can decide what is the most stable sanity
         check for itself.
 
@@ -138,48 +127,46 @@
     @property
     def options(self):
         return self._config.config["driver"]["options"]
 
     @property
     def instance_config(self):
         return os.path.join(
-            self._config.scenario.ephemeral_directory, "instance_config.yml"
+            self._config.scenario.ephemeral_directory,
+            "instance_config.yml",
         )
 
     @property
     def ssh_connection_options(self):
         if self._config.config["driver"]["ssh_connection_options"]:
             return self._config.config["driver"]["ssh_connection_options"]
         return self.default_ssh_connection_options
 
     @property
     def safe_files(self):
         return self.default_safe_files + self._config.config["driver"]["safe_files"]
 
     @property
     def delegated(self):
-        """
-        Is the driver delegated and returns a bool.
+        """Is the driver delegated and returns a bool.
 
         :returns: bool
         """
         return self.name == "delegated"
 
     @property
     def managed(self):
-        """
-        Is the driver is managed and returns a bool.
+        """Is the driver is managed and returns a bool.
 
         :returns: bool
         """
         return self.options["managed"]
 
     def status(self):
-        """
-        Collect the instances state and returns a list.
+        """Collect the instances state and returns a list.
 
         !!! note
 
             Molecule assumes all instances were created successfully by
             Ansible, otherwise Ansible would return an error on create.  This
             may prove to be a bad assumption.  However, configuring Molecule's
             driver to match the options passed to the playbook may prove
@@ -198,15 +185,15 @@
                 Status(
                     instance_name=instance_name,
                     driver_name=driver_name,
                     provisioner_name=provisioner_name,
                     scenario_name=scenario_name,
                     created=self._created(),
                     converged=self._converged(),
-                )
+                ),
             )
 
         return status_list
 
     def _get_ssh_connection_options(self):
         # LogLevel=ERROR is needed in order to avoid warnings like:
         # Warning: Permanently added ... to the list of known hosts.
@@ -236,19 +223,19 @@
         """Implement lower than comparison."""
         return str.__lt__(str(self), str(other))
 
     def __hash__(self):
         """Perform object hash."""
         return self.name.__hash__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return readable string representation of object."""
         return self.name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Return detailed string representation of object."""
         return self.name
 
     def __rich__(self):
         """Return rich representation of object."""
         return self.__str__()
 
@@ -259,15 +246,15 @@
             p = os.path.abspath(
                 os.path.join(
                     os.path.dirname(molecule.__file__),
                     "cookiecutter",
                     "scenario",
                     "driver",
                     self.name,
-                )
+                ),
             )
         return p
 
     def get_playbook(self, step):
         """Return embedded playbook location or None.
 
         The default location is relative to the file implementing the driver
@@ -277,26 +264,28 @@
         p = os.path.join(
             self._path,
             "playbooks",
             step + ".yml",
         )
         if os.path.isfile(p):
             return p
+        return None
 
     def modules_dir(self):
         """Return path to ansible modules included with driver."""
         p = os.path.join(self._path, "modules")
         if os.path.isdir(p):
             return p
+        return None
 
     def reset(self):
         """Release all resources owned by molecule.
 
         This is a destructive operation that would affect all resources managed
         by molecule, regardless the scenario name.  Molecule will use metadata
         like labels or tags to annotate resources allocated by it.
         """
 
     @property
-    def required_collections(self) -> Dict[str, str]:
+    def required_collections(self) -> dict[str, str]:
         """Return collections dict containing names and versions required."""
         return {}
```

### Comparing `molecule-5.0.0a0/src/molecule/driver/delegated.py` & `molecule-5.0.0a1/src/molecule/driver/delegated.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 from molecule import util
 from molecule.api import Driver
 
 LOG = logging.getLogger(__name__)
 
 
 class Delegated(Driver):
-    r"""
-    The class responsible for managing delegated instances.
+    r"""The class responsible for managing delegated instances.
 
     Delegated is `not` the default driver used in Molecule.
 
     Under this driver, it is the developers responsibility to implement the
     create and destroy playbooks.  ``Managed`` is the default behaviour of all
     drivers.
 
@@ -131,17 +130,17 @@
           options:
             managed: False
             ansible_connection_options:
               ansible_connection: local
     ```
     """
 
-    def __init__(self, config=None):
+    def __init__(self, config=None) -> None:
         """Construct Delegated."""
-        super(Delegated, self).__init__(config)
+        super().__init__(config)
         self._name = "delegated"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -159,30 +158,32 @@
             return (
                 "ssh {address} "
                 "-l {user} "
                 "-p {port} "
                 "-i {identity_file} "
                 f"{connection_options}"
             )
+        return None
 
     @property
     def default_safe_files(self):
         return []
 
     @property
     def default_ssh_connection_options(self):
         if self.managed:
             ssh_connopts = self._get_ssh_connection_options()
             if self.options.get("ansible_connection_options", {}).get(
-                "ansible_ssh_common_args", None
+                "ansible_ssh_common_args",
+                None,
             ):
                 ssh_connopts.append(
                     self.options.get("ansible_connection_options").get(
-                        "ansible_ssh_common_args"
-                    )
+                        "ansible_ssh_common_args",
+                    ),
                 )
             return ssh_connopts
         return []
 
     def login_options(self, instance_name):
         if self.managed:
             d = {"instance": instance_name}
@@ -203,47 +204,47 @@
                 if d.get("become_method", False):
                     conn_dict["ansible_become_method"] = d.get("become_method")
                 if d.get("become_pass", None):
                     conn_dict["ansible_become_pass"] = d.get("become_pass")
                 if d.get("identity_file", None):
                     conn_dict["ansible_private_key_file"] = d.get("identity_file")
                     conn_dict["ansible_ssh_common_args"] = " ".join(
-                        self.ssh_connection_options
+                        self.ssh_connection_options,
                     )
                 if d.get("password", None):
                     conn_dict["ansible_password"] = d.get("password")
                     # Based on testinfra documentation, ansible password must be passed via ansible_ssh_pass
                     # issue to fix this can be found https://github.com/pytest-dev/pytest-testinfra/issues/580
                     conn_dict["ansible_ssh_pass"] = d.get("password")
                 if d.get("winrm_transport", None):
                     conn_dict["ansible_winrm_transport"] = d.get("winrm_transport")
                 if d.get("winrm_cert_pem", None):
                     conn_dict["ansible_winrm_cert_pem"] = d.get("winrm_cert_pem")
                 if d.get("winrm_cert_key_pem", None):
                     conn_dict["ansible_winrm_cert_key_pem"] = d.get(
-                        "winrm_cert_key_pem"
+                        "winrm_cert_key_pem",
                     )
                 if d.get("winrm_server_cert_validation", None):
                     conn_dict["ansible_winrm_server_cert_validation"] = d.get(
-                        "winrm_server_cert_validation"
+                        "winrm_server_cert_validation",
                     )
 
                 return conn_dict
 
             except StopIteration:
                 return {}
-            except IOError:
+            except OSError:
                 # Instance has yet to be provisioned , therefore the
                 # instance_config is not on disk.
                 return {}
         return self.options.get("ansible_connection_options", {})
 
     def _created(self):
         if self.managed:
-            return super(Delegated, self)._created()
+            return super()._created()
         return "unknown"
 
     def _get_instance_config(self, instance_name):
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
 
         return next(
             item for item in instance_config_dict if item["instance"] == instance_name
```

### Comparing `molecule-5.0.0a0/src/molecule/interpolation.py` & `molecule-5.0.0a1/src/molecule/interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 #    under the License.
 
 # Taken from Docker Compose:
 # https://github.com/docker/compose/blob/master/compose/config/interpolation.py
 """Iterpolation Module."""
 
 import string
-from typing import MutableMapping, Type
+from collections.abc import MutableMapping
 
 
 class InvalidInterpolation(Exception):
     """InvalidInterpolation Exception."""
 
-    def __init__(self, string: str, place: Exception):
+    def __init__(self, string: str, place: Exception) -> None:
         """Construct InvalidInterpolation."""
         self.string = string
         self.place = place
 
 
-class Interpolator(object):
-    """
-    Configuration options may contain environment variables.
+class Interpolator:
+    """Configuration options may contain environment variables.
 
     For example, suppose the shell contains ``VERIFIER_NAME=testinfra`` and
     the following molecule.yml is supplied.
 
     ```yaml
         verifier:
           - name: ${VERIFIER_NAME}
@@ -68,16 +67,18 @@
         prefix your own variables with `MOLECULE_`.
 
     A file may be placed in the root of the project as `.env.yml`, and Molecule
     will read variables when rendering `molecule.yml`.  See command usage.
     """
 
     def __init__(
-        self, templater: Type["TemplateWithDefaults"], mapping: MutableMapping
-    ):
+        self,
+        templater: type["TemplateWithDefaults"],
+        mapping: MutableMapping,
+    ) -> None:
         """Construct Interpolator."""
         self.templater = templater
         self.mapping = mapping
 
     def interpolate(self, string: str, keep_string=None) -> str:
         try:
             return self.templater(string).substitute(self.mapping, keep_string)  # type: ignore
@@ -86,15 +87,15 @@
 
 
 class TemplateWithDefaults(string.Template):
     """TemplateWithDefaults Class."""
 
     idpattern = r"[_a-z][_a-z0-9]*(?::?-[^}]+)?"
 
-    # Modified from python2.7/string.py
+    # pylint: disable=too-many-return-statements
     def substitute(self, mapping, keep_string):
         # Helper function for .sub()
         def convert(mo):
             # Check the most common path first.
             named = mo.group("named") or mo.group("braced")
             if named is not None:
                 # TODO(retr0h): This needs to be better handled.
@@ -114,9 +115,11 @@
                     return mapping.get(var, default)
                 val = mapping.get(named, "")
                 return f"{val}"
             if mo.group("escaped") is not None:
                 return self.delimiter
             if mo.group("invalid") is not None:
                 self._invalid(mo)
+                return None
+            return None
 
         return self.pattern.sub(convert, self.template)
```

### Comparing `molecule-5.0.0a0/src/molecule/logger.py` & `molecule-5.0.0a1/src/molecule/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Logging Module."""
 
 import logging
 import os
 import time
+from collections.abc import Iterable
 from functools import wraps
-from typing import Callable, Iterable
+from typing import Callable
 
 from ansible_compat.ports import cache
 from enrich.logging import RichHandler
 
 from molecule.console import console, console_stderr
 from molecule.text import underscore
 
@@ -36,47 +37,47 @@
 LOG_LEVEL_LUT = {
     0: logging.INFO,
     1: logging.DEBUG,
 }
 
 
 def configure() -> None:
-    """
-    Configure a molecule root logger.
+    """Configure a molecule root logger.
 
     All other loggers will inherit the configuration we set here.
     """
     # Keep using root logger because we do want to process messages from other
     # libraries.
     logger = logging.getLogger()
     handler = RichHandler(
-        console=console_stderr, show_time=False, show_path=False, markup=True
+        console=console_stderr,
+        show_time=False,
+        show_path=False,
+        markup=True,
     )  # type: ignore
     logger.addHandler(handler)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
 
 def set_log_level(log_level: int, debug: bool) -> None:
-    """
-    Set logging level.
+    """Set logging level.
 
     :param log_level: verbosity control (0 - INFO, 1 - DEBUG)
     :param debug: debug mode indicator
     """
     # If we get verbosity level > 1, we just use debug because this is the
     # most detailed log level we have.
     if debug:
         log_level = 1  # DEBUG from the LOG_LEVEL_LUT
     logging.getLogger("molecule").setLevel(LOG_LEVEL_LUT.get(log_level, logging.DEBUG))
 
 
 def get_logger(name: str) -> logging.Logger:
-    """
-    Return a child logger.
+    """Return a child logger.
 
     Returned logger inherits configuration from the molecule logger.
     """
     return logging.getLogger("molecule." + name)
 
 
 def github_actions_groups(func: Callable) -> Callable:
@@ -195,14 +196,14 @@
 @cache
 def get_section_loggers() -> Iterable[Callable]:
     """Return a list of section wrappers to be added."""
     default_section_loggers = [section_logger]
     if not os.getenv("CI"):
         return default_section_loggers
     elif os.getenv("GITHUB_ACTIONS"):
-        return [github_actions_groups] + default_section_loggers
+        return [github_actions_groups, *default_section_loggers]
     elif os.getenv("GITLAB_CI"):
-        return [gitlab_ci_sections] + default_section_loggers
+        return [gitlab_ci_sections, *default_section_loggers]
     elif os.getenv("TRAVIS"):
-        return [travis_ci_folds] + default_section_loggers
+        return [travis_ci_folds, *default_section_loggers]
     # CI is set but no extra section_loggers apply.
     return default_section_loggers
```

### Comparing `molecule-5.0.0a0/src/molecule/platforms.py` & `molecule-5.0.0a1/src/molecule/platforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 import logging
 
 from molecule import util
 
 LOG = logging.getLogger(__name__)
 
 
-class Platforms(object):
-    """
-    Platforms define the instances to be tested, and the groups to which the \
+class Platforms:
+    """Platforms define the instances to be tested, and the groups to which the \
     instances belong.
 
     ``` yaml
 
         platforms:
           - name: instance-1
     ```
@@ -65,29 +64,30 @@
               - group1
               - group2
             children:
               - child_group1
     ```
     """
 
-    def __init__(self, config, parallelize_platforms=False, platform_name=None):
-        """
-        Initialize a new platform class and returns None.
+    def __init__(self, config, parallelize_platforms=False, platform_name=None) -> None:
+        """Initialize a new platform class and returns None.
 
         :param config: An instance of a Molecule config.
         :param parallelize_platforms: Parallel mode. Default is False.
         :param platform_name: One platform to target only, defaults to None.
         :return: None
         """
         if platform_name:
             config.config["platforms"] = util._filter_platforms(
-                config.config, platform_name
-            )
+                config.config,
+                platform_name,
+            )  # type: ignore
         if parallelize_platforms:
             config.config["platforms"] = util._parallelize_platforms(
-                config.config, config._run_uuid
-            )
+                config.config,
+                config._run_uuid,
+            )  # type: ignore
         self._config = config
 
     @property
     def instances(self):
         return self._config.config["platforms"]
```

### Comparing `molecule-5.0.0a0/src/molecule/provisioner/ansible.py` & `molecule-5.0.0a1/src/molecule/provisioner/ansible.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
 # pylint: disable=too-many-lines
 import collections
 import copy
 import logging
 import os
 import shutil
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 from ansible_compat.ports import cached_property
 
 from molecule import util
 from molecule.api import drivers
 from molecule.provisioner import ansible_playbook, ansible_playbooks, base
 
 LOG = logging.getLogger(__name__)
 
 
 class Ansible(base.Base):
     """
-    `Ansible`_ is the default provisioner.  No other provisioner will be \
+    `Ansible` is the default provisioner.  No other provisioner will be \
     supported.
 
     Molecule's provisioner manages the instances lifecycle.  However, the user
     must provide the create, destroy, and converge playbooks.  Molecule's
     ``init`` subcommand will provide the necessary files for convenience.
 
     Molecule will skip tasks which are tagged with either `molecule-notest` or
@@ -66,15 +66,15 @@
 
     !!! note
 
         Options do not affect the create and destroy actions.
 
     !!! note
 
-        Molecule will remove any options matching '^[v]+$', and pass ``-vvv``
+        Molecule will remove any options matching `^[v]+$`, and pass ``-vvv``
         to the underlying ``ansible-playbook`` command when executing
         `molecule --debug`.
 
     Molecule will silence log output, unless invoked with the ``--debug`` flag.
     However, this results in quite a bit of output.  To enable Ansible log
     output, add the following to the ``provisioner`` section of ``molecule.yml``.
 
@@ -371,35 +371,59 @@
         provisioner:
           name: ansible
           connection_options:
             ansible_ssh_user: foo
             ansible_ssh_common_args: -o IdentitiesOnly=no
     ```
 
+    Override tags:
+
+    ``` yaml
+        provisioner:
+        name: ansible
+        config_options:
+          tags:
+            run: tag1,tag2,tag3
+    ```
+
+    A typical use case is if you want to use tags within a scenario.
+    Don't forget to add a tag `always` in `converge.yml` as below.
+
+    ``` yaml
+        ---
+        - name: Converge
+          hosts: all
+          tasks:
+            - name: "Include acme.my_role_name"
+              ansible.builtin.include_role:
+                name: "acme.my_role_name"
+              tags:
+                - always
+    ```
+
     .. _`variables defined in a playbook`: https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html#defining-variables-in-a-playbook
 
     Add arguments to ansible-playbook when running converge:
 
     ``` yaml
         provisioner:
           name: ansible
           ansible_args:
             - --inventory=mygroups.yml
             - --limit=host1,host2
     ```
-    """  # noqa
+    """
 
-    def __init__(self, config):
-        """
-        Initialize a new ansible class and returns None.
+    def __init__(self, config) -> None:
+        """Initialize a new ansible class and returns None.
 
         :param config: An instance of a Molecule config.
         :return: None
         """
-        super(Ansible, self).__init__(config)
+        super().__init__(config)
 
     @property
     def default_config_options(self) -> dict[str, Any]:
         """Provide Default options to construct ansible.cfg and returns a dict."""
         return {
             "defaults": {
                 "ansible_managed": "Ansible managed: Do NOT edit this file manually!",
@@ -435,61 +459,64 @@
         collection_indicator = "ansible_collections"
         # isolating test environment by injects ephemeral scenario directory on
         # top of the collection_path_list. This prevents dependency commands
         # from installing dependencies to user list of collections.
         collections_path_list = [
             util.abs_path(
                 os.path.join(
-                    self._config.scenario.config.runtime.cache_dir, "collections"
-                )
+                    self._config.scenario.config.runtime.cache_dir,
+                    "collections",
+                ),
             ),
             util.abs_path(
-                os.path.join(self._config.scenario.ephemeral_directory, "collections")
+                os.path.join(self._config.scenario.ephemeral_directory, "collections"),
             ),
         ]
         if collection_indicator in self._config.project_directory:
             collection_path, right = self._config.project_directory.rsplit(
-                collection_indicator, 1
+                collection_indicator,
+                1,
             )
             collections_path_list.append(util.abs_path(collection_path))
         collections_path_list.extend(
             [
                 util.abs_path(
-                    os.path.join(os.path.expanduser("~"), ".ansible/collections")
+                    os.path.join(os.path.expanduser("~"), ".ansible/collections"),
                 ),
                 "/usr/share/ansible/collections",
                 "/etc/ansible/collections",
-            ]
+            ],
         )
 
         if os.environ.get("ANSIBLE_COLLECTIONS_PATH", ""):
             collections_path_list.extend(
                 list(
                     map(
-                        util.abs_path, os.environ["ANSIBLE_COLLECTIONS_PATH"].split(":")
-                    )
-                )
+                        util.abs_path,
+                        os.environ["ANSIBLE_COLLECTIONS_PATH"].split(":"),
+                    ),
+                ),
             )
 
         roles_path_list = [
             util.abs_path(
-                os.path.join(self._config.scenario.config.runtime.cache_dir, "roles")
+                os.path.join(self._config.scenario.config.runtime.cache_dir, "roles"),
             ),
             util.abs_path(
-                os.path.join(self._config.scenario.ephemeral_directory, "roles")
+                os.path.join(self._config.scenario.ephemeral_directory, "roles"),
             ),
             util.abs_path(os.path.join(self._config.project_directory, os.path.pardir)),
             util.abs_path(os.path.join(os.path.expanduser("~"), ".ansible", "roles")),
             "/usr/share/ansible/roles",
             "/etc/ansible/roles",
         ]
 
         if os.environ.get("ANSIBLE_ROLES_PATH", ""):
             roles_path_list.extend(
-                list(map(util.abs_path, os.environ["ANSIBLE_ROLES_PATH"].split(":")))
+                list(map(util.abs_path, os.environ["ANSIBLE_ROLES_PATH"].split(":"))),
             )
 
         env = util.merge_dicts(
             os.environ,
             {
                 "ANSIBLE_CONFIG": self._config.provisioner.config_file,
                 "ANSIBLE_ROLES_PATH": ":".join(roles_path_list),
@@ -499,28 +526,33 @@
                     [
                         self._get_filter_plugin_directory(),
                         util.abs_path(
                             os.path.join(
                                 self._config.scenario.ephemeral_directory,
                                 "plugins",
                                 "filter",
-                            )
+                            ),
                         ),
                         util.abs_path(
                             os.path.join(
-                                self._config.project_directory, "plugins", "filter"
-                            )
+                                self._config.project_directory,
+                                "plugins",
+                                "filter",
+                            ),
                         ),
                         util.abs_path(
                             os.path.join(
-                                os.path.expanduser("~"), ".ansible", "plugins", "filter"
-                            )
+                                os.path.expanduser("~"),
+                                ".ansible",
+                                "plugins",
+                                "filter",
+                            ),
                         ),
                         "/usr/share/ansible/plugins/filter",
-                    ]
+                    ],
                 ),
             },
         )
         env = util.merge_dicts(env, self._config.env)
 
         return env
 
@@ -601,16 +633,15 @@
 
     @property
     def links(self):
         return self._config.config["provisioner"]["inventory"]["links"]
 
     @property
     def inventory(self):
-        """
-        Create an inventory structure and returns a dict.
+        """Create an inventory structure and returns a dict.
 
         ``` yaml
             ungrouped:
               vars:
                 foo: bar
               hosts:
                 instance-1:
@@ -683,68 +714,64 @@
             os.path.pardir,
             "molecule",
             "provisioner",
             "ansible",
         )
 
     def cleanup(self):
-        """
-        Execute `ansible-playbook` against the cleanup playbook and returns \
+        """Execute `ansible-playbook` against the cleanup playbook and returns \
         None.
 
         :return: None
         """
         pb = self._get_ansible_playbook(self.playbooks.cleanup)
         pb.execute()
 
     def connection_options(self, instance_name):
         d = self._config.driver.ansible_connection_options(instance_name)
 
         return util.merge_dicts(
-            d, self._config.config["provisioner"]["connection_options"]
+            d,
+            self._config.config["provisioner"]["connection_options"],
         )
 
     def check(self):
-        """
-        Execute ``ansible-playbook`` against the converge playbook with the \
+        """Execute ``ansible-playbook`` against the converge playbook with the \
         ``--check`` flag and returns None.
 
         :return: None
         """
         pb = self._get_ansible_playbook(self.playbooks.converge)
         pb.add_cli_arg("check", True)
         pb.execute()
 
     def converge(self, playbook=None, **kwargs):
-        """
-        Execute ``ansible-playbook`` against the converge playbook unless \
+        """Execute ``ansible-playbook`` against the converge playbook unless \
         specified otherwise and returns a string.
 
         :param playbook: An optional string containing an absolute path to a
          playbook.
         :param kwargs: An optional keyword arguments.
         :return: str
         """
         pb = self._get_ansible_playbook(playbook or self.playbooks.converge, **kwargs)
 
         return pb.execute()
 
     def destroy(self):
-        """
-        Execute ``ansible-playbook`` against the destroy playbook and returns \
+        """Execute ``ansible-playbook`` against the destroy playbook and returns \
         None.
 
         :return: None
         """
         pb = self._get_ansible_playbook(self.playbooks.destroy)
         pb.execute()
 
     def side_effect(self, action_args=None):
-        """
-        Execute ``ansible-playbook`` against the side_effect playbook and \
+        """Execute ``ansible-playbook`` against the side_effect playbook and \
         returns None.
 
         :return: None
         """
         if action_args:
             playbooks = [
                 self._get_ansible_playbook(self._config.provisioner.abs_path(playbook))
@@ -752,47 +779,43 @@
             ]
         else:
             playbooks = [self._get_ansible_playbook(self.playbooks.side_effect)]
         for pb in playbooks:
             pb.execute()
 
     def create(self):
-        """
-        Execute ``ansible-playbook`` against the create playbook and returns \
+        """Execute ``ansible-playbook`` against the create playbook and returns \
         None.
 
         :return: None
         """
         pb = self._get_ansible_playbook(self.playbooks.create)
         pb.execute()
 
     def prepare(self):
-        """
-        Execute ``ansible-playbook`` against the prepare playbook and returns \
+        """Execute ``ansible-playbook`` against the prepare playbook and returns \
         None.
 
         :return: None
         """
         pb = self._get_ansible_playbook(self.playbooks.prepare)
         pb.execute()
 
     def syntax(self):
-        """
-        Execute ``ansible-playbook`` against the converge playbook with the \
+        """Execute ``ansible-playbook`` against the converge playbook with the \
         ``-syntax-check`` flag and returns None.
 
         :return: None
         """
         pb = self._get_ansible_playbook(self.playbooks.converge)
         pb.add_cli_arg("syntax-check", True)
         pb.execute()
 
     def verify(self, action_args=None):
-        """
-        Execute ``ansible-playbook`` against the verify playbook and returns \
+        """Execute ``ansible-playbook`` against the verify playbook and returns \
         None.
 
         :return: None
         """
         if action_args:
             playbooks = [
                 self._config.provisioner.abs_path(playbook) for playbook in action_args
@@ -804,43 +827,41 @@
             return
         for playbook in playbooks:
             # Get ansible playbooks for `verify` instead of `provision`
             pb = self._get_ansible_playbook(playbook, verify=True)
             pb.execute()
 
     def write_config(self):
-        """
-        Write the provisioner's config file to disk and returns None.
+        """Write the provisioner's config file to disk and returns None.
 
         :return: None
         """
         template = util.render_template(
-            self._get_config_template(), config_options=self.config_options
+            self._get_config_template(),
+            config_options=self.config_options,
         )
         util.write_file(self.config_file, template)
 
     def manage_inventory(self):
-        """
-        Manage inventory for Ansible and returns None.
+        """Manage inventory for Ansible and returns None.
 
         :returns: None
         """
         self._write_inventory()
         self._remove_vars()
         if not self.links:
             self._add_or_update_vars()
         else:
             self._link_or_update_vars()
 
     def abs_path(self, path: str) -> Optional[str]:
         return util.abs_path(os.path.join(self._config.scenario.directory, path))
 
     def _add_or_update_vars(self):
-        """
-        Create host and/or group vars and returns None.
+        """Create host and/or group vars and returns None.
 
         :returns: None
         """
         # Create the hosts extra inventory source (only if not empty)
         hosts_file = os.path.join(self.inventory_directory, "hosts")
         if self.hosts:
             util.write_file(hosts_file, util.safe_dump(self.hosts))
@@ -857,45 +878,42 @@
 
             if vars_target:
                 target_vars_directory = os.path.join(self.inventory_directory, target)
 
                 if not os.path.isdir(util.abs_path(target_vars_directory)):
                     os.mkdir(util.abs_path(target_vars_directory))
 
-                for target in vars_target.keys():
+                for target in vars_target:
                     target_var_content = vars_target[target]
                     path = os.path.join(util.abs_path(target_vars_directory), target)
                     util.write_file(path, util.safe_dump(target_var_content))
 
     def _write_inventory(self):
-        """
-        Write the provisioner's inventory file to disk and returns None.
+        """Write the provisioner's inventory file to disk and returns None.
 
         :return: None
         """
         self._verify_inventory()
 
         util.write_file(self.inventory_file, util.safe_dump(self.inventory))
 
     def _remove_vars(self):
-        """
-        Remove hosts/host_vars/group_vars and returns None.
+        """Remove hosts/host_vars/group_vars and returns None.
 
         :returns: None
         """
         for name in ("hosts", "group_vars", "host_vars"):
             d = os.path.join(self.inventory_directory, name)
             if os.path.islink(d) or os.path.isfile(d):
                 os.unlink(d)
             elif os.path.isdir(d):
                 shutil.rmtree(d)
 
     def _link_or_update_vars(self):
-        """
-        Create or updates the symlink to group_vars and returns None.
+        """Create or updates the symlink to group_vars and returns None.
 
         :returns: None
         """
         for d, source in self.links.items():
             target = os.path.join(self.inventory_directory, d)
             source = os.path.join(self._config.scenario.directory, source)
 
@@ -903,103 +921,102 @@
                 msg = f"The source path '{source}' does not exist."
                 util.sysexit_with_message(msg)
             msg = f"Inventory {source} linked to {target}"
             LOG.debug(msg)
             os.symlink(source, target)
 
     def _get_ansible_playbook(self, playbook, verify=False, **kwargs):
-        """
-        Get an instance of AnsiblePlaybook and returns it.
+        """Get an instance of AnsiblePlaybook and returns it.
 
         :param playbook: A string containing an absolute path to a
          provisioner's playbook.
         :param verify: An optional bool to toggle the Plabook mode between
          provision and verify. False: provision; True: verify. Default is False.
         :param kwargs: An optional keyword arguments.
         :return: object
         """
         return ansible_playbook.AnsiblePlaybook(
-            playbook, self._config, verify, **kwargs
+            playbook,
+            self._config,
+            verify,
+            **kwargs,
         )
 
     def _verify_inventory(self):
-        """
-        Verify the inventory is valid and returns None.
+        """Verify the inventory is valid and returns None.
 
         :return: None
         """
         if not self.inventory:
             msg = "Instances missing from the 'platform' " "section of molecule.yml."
             util.sysexit_with_message(msg)
 
     def _get_config_template(self):
-        """
-        Return a config template string.
+        """Return a config template string.
 
         :return: str
         """
         return """
 {% for section, section_dict in config_options.items() -%}
 [{{ section }}]
 {% for k, v in section_dict.items() -%}
 {{ k }} = {{ v }}
 {% endfor -%}
 {% endfor -%}
 """.strip()
 
     def _vivify(self):
-        """
-        Return an autovivification default dict.
+        """Return an autovivification default dict.
 
         :return: dict
         """
         return collections.defaultdict(self._vivify)
 
     def _default_to_regular(self, d):
         if isinstance(d, collections.defaultdict):
             d = {k: self._default_to_regular(v) for k, v in d.items()}
 
         return d
 
     def _get_plugin_directory(self) -> str:
         return os.path.join(self.directory, "plugins")
 
-    def _get_modules_directories(self) -> List[str]:
+    def _get_modules_directories(self) -> list[str]:
         """Return list of ansilbe module includes directories.
 
         Adds modules directory from molecule and its plugins.
         """
-        paths: List[Optional[str]] = []
+        paths: list[Optional[str]] = []
         if os.environ.get("ANSIBLE_LIBRARY"):
             paths = list(map(util.abs_path, os.environ["ANSIBLE_LIBRARY"].split(":")))
 
         paths.append(
-            util.abs_path(os.path.join(self._get_plugin_directory(), "modules"))
+            util.abs_path(os.path.join(self._get_plugin_directory(), "modules")),
         )
 
         for d in drivers():
             p = d.modules_dir()
             if p:
                 paths.append(p)
         paths.extend(
             [
                 util.abs_path(
-                    os.path.join(self._config.scenario.ephemeral_directory, "library")
+                    os.path.join(self._config.scenario.ephemeral_directory, "library"),
                 ),
                 util.abs_path(os.path.join(self._config.project_directory, "library")),
                 util.abs_path(
                     os.path.join(
                         os.path.expanduser("~"),
                         ".ansible",
                         "plugins",
                         "modules",
-                    )
+                    ),
                 ),
                 "/usr/share/ansible/plugins/modules",
-            ]
+            ],
         )
 
         return [path for path in paths if path is not None]
 
     def _get_filter_plugin_directory(self):
         return util.abs_path(os.path.join(self._get_plugin_directory(), "filter"))
```

### Comparing `molecule-5.0.0a0/src/molecule/provisioner/ansible_playbook.py` & `molecule-5.0.0a1/src/molecule/provisioner/ansible_playbook.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,42 +24,41 @@
 
 from molecule import util
 from molecule.api import MoleculeRuntimeWarning
 
 LOG = logging.getLogger(__name__)
 
 
-class AnsiblePlaybook(object):
+class AnsiblePlaybook:
     """Provisioner Playbook."""
 
-    def __init__(self, playbook, config, verify=False):
-        """
-        Set up the requirements to execute ``ansible-playbook`` and returns \
+    def __init__(self, playbook, config, verify=False) -> None:
+        """Set up the requirements to execute ``ansible-playbook`` and returns \
         None.
 
         :param playbook: A string containing the path to the playbook.
         :param config: An instance of a Molecule config.
         :param verify: An optional bool to toggle the Plabook mode between
          provision and verify. False: provision; True: verify. Default is False.
         :returns: None
         """
         self._ansible_command = None
         self._playbook = playbook
         self._config = config
-        self._cli = {}
+        self._cli = {}  # type: ignore
         if verify:
             self._env = util.merge_dicts(
-                self._config.verifier.env, self._config.config["verifier"]["env"]
+                self._config.verifier.env,
+                self._config.config["verifier"]["env"],
             )
         else:
             self._env = self._config.provisioner.env
 
     def bake(self):
-        """
-        Bake an ``ansible-playbook`` command so it's ready to execute and \
+        """Bake an ``ansible-playbook`` command so it's ready to execute and \
         returns ``None``.
 
         :return: None
         """
         if not self._playbook:
             return
 
@@ -78,15 +77,15 @@
         # custom Ansible arguments can break the creation and destruction
         # processes.
         #
         # If users need to modify the creation of deletion, they can supply
         # custom playbooks and specify them in the scenario configuration.
         if self._config.action not in ["create", "destroy"]:
             ansible_args = list(self._config.provisioner.ansible_args) + list(
-                self._config.ansible_args
+                self._config.ansible_args,
             )
         else:
             ansible_args = []
 
         self._ansible_command = util.BakedCommand(
             cmd=[
                 "ansible-playbook",
@@ -96,25 +95,24 @@
                 self._playbook,  # must always go last
             ],
             cwd=self._config.scenario.directory,
             env=self._env,
         )
 
     def execute(self, action_args=None):
-        """
-        Execute ``ansible-playbook`` and returns a string.
+        """Execute ``ansible-playbook`` and returns a string.
 
         :return: str
         """
         if self._ansible_command is None:
             self.bake()
 
         if not self._playbook:
             LOG.warning("Skipping, %s action has no playbook.", self._config.action)
-            return
+            return None
 
         with warnings.catch_warnings(record=True) as warns:
             warnings.filterwarnings("default", category=MoleculeRuntimeWarning)
             self._config.driver.sanity_checks()
             result = util.run_command(self._ansible_command, debug=self._config.debug)
 
         if result.returncode != 0:
@@ -123,27 +121,25 @@
                 result.returncode,
                 warns=warns,
             )
 
         return result.stdout
 
     def add_cli_arg(self, name, value):
-        """
-        Add argument to CLI passed to ansible-playbook and returns None.
+        """Add argument to CLI passed to ansible-playbook and returns None.
 
         :param name: A string containing the name of argument to be added.
         :param value: The value of argument to be added.
         :return: None
         """
         if value:
             self._cli[name] = value
 
     def add_env_arg(self, name, value):
-        """
-        Add argument to environment passed to ansible-playbook and returns \
+        """Add argument to environment passed to ansible-playbook and returns \
         None.
 
         :param name: A string containing the name of argument to be added.
         :param value: The value of argument to be added.
         :return: None
         """
         self._env[name] = value
```

### Comparing `molecule-5.0.0a0/src/molecule/provisioner/ansible_playbooks.py` & `molecule-5.0.0a1/src/molecule/provisioner/ansible_playbooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Ansible-Playbooks Provisioner Module."""
 
-from __future__ import absolute_import
 
 import logging
 import os
 
 from molecule import util
 
 LOG = logging.getLogger(__name__)
 
 
-class AnsiblePlaybooks(object):
+class AnsiblePlaybooks:
     """A class to act as a module to namespace playbook properties."""
 
-    def __init__(self, config):
-        """
-        Initialize a new namespace class and returns None.
+    def __init__(self, config) -> None:
+        """Initialize a new namespace class and returns None.
 
         :param config: An instance of a Molecule config.
         :return: None
         """
         self._config = config
 
     @property
@@ -67,20 +65,19 @@
 
     @property
     def verify(self):
         return self._get_playbook("verify")
 
     def _get_playbook_directory(self):
         return util.abs_path(
-            os.path.join(self._config.provisioner.directory, "playbooks")
+            os.path.join(self._config.provisioner.directory, "playbooks"),
         )
 
     def _get_playbook(self, section):
-        """
-        Return path to playbook or None if playbook is not needed.
+        """Return path to playbook or None if playbook is not needed.
 
         Return None when there is no playbook configured and when action is
         considered skippable.
         """
         c = self._config.config
         driver_dict = c["provisioner"]["playbooks"].get(self._config.driver.name)
 
@@ -125,28 +122,28 @@
             self._config.driver._path,
             "playbooks",
             self._config.config["provisioner"]["playbooks"][section],
         )
         return path
 
     def _normalize_playbook(self, playbook):
-        """
-        Return current filename to use for a playook by allowing fallbacks.
+        """Return current filename to use for a playook by allowing fallbacks.
 
         Currently used to deprecate use of playbook.yml in favour of converge.yml
         """
         # TODO(ssbarnea): Remove that deprecation fallback in 3.1+
         if not playbook or os.path.isfile(playbook):
             return playbook
 
         pb_rename_map = {"converge.yml": "playbook.yml"}
         basename = os.path.basename(playbook)
         if basename in pb_rename_map:
             fb_playbook = os.path.join(
-                os.path.dirname(playbook), pb_rename_map[basename]
+                os.path.dirname(playbook),
+                pb_rename_map[basename],
             )
             if os.path.isfile(fb_playbook):
                 LOG.warning(
                     "%s was deprecated, rename it to %s",
                     pb_rename_map[basename],
                     basename,
                 )
```

### Comparing `molecule-5.0.0a0/src/molecule/provisioner/base.py` & `molecule-5.0.0a1/src/molecule/provisioner/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,47 +18,43 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Provisioner Base Module."""
 
 import abc
 
 
-class Base(object):
+class Base:
     """Provisioner Base Class."""
 
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, config):
-        """
-        Initialize code for all :ref:`Provisioner` classes.
+    def __init__(self, config) -> None:
+        """Initialize code for all :ref:`Provisioner` classes.
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
 
     @property
     @abc.abstractmethod
     def default_options(self):  # pragma: no cover
-        """
-        Get default CLI arguments provided to ``cmd`` as a dict.
+        """Get default CLI arguments provided to ``cmd`` as a dict.
 
         :return: dict
         """
 
     @property
     @abc.abstractmethod
     def default_env(self):  # pragma: no cover
-        """
-        Get default env variables provided to ``cmd`` as a dict.
+        """Get default env variables provided to ``cmd`` as a dict.
 
         :return: dict
         """
 
     @property
     @abc.abstractmethod
     def name(self):  # pragma: no cover
-        """
-        Name of the provisioner and returns a string.
+        """Name of the provisioner and returns a string.
 
         :returns: str
         """
```

### Comparing `molecule-5.0.0a0/src/molecule/scenario.py` & `molecule-5.0.0a1/src/molecule/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,54 +31,53 @@
 
 from molecule import scenarios, util
 from molecule.constants import RC_TIMEOUT
 
 LOG = logging.getLogger(__name__)
 
 
-class Scenario(object):
+class Scenario:
     """A Molecule scenario."""
 
-    def __init__(self, config):
-        """
-        Initialize a new scenario class and returns None.
+    def __init__(self, config) -> None:
+        """Initialize a new scenario class and returns None.
 
         :param config: An instance of a Molecule config.
         :return: None
         """
         self._lock = None
         self.config = config
-        self._setup()
+        self._setup()  # type: ignore
 
     def _remove_scenario_state_directory(self):
         """Remove scenario cached disk stored state.
 
         :return: None
         """
         directory = str(Path(self.ephemeral_directory).parent)
         LOG.info("Removing %s", directory)
         shutil.rmtree(directory)
 
     def prune(self):
-        """
-        Prune the scenario ephemeral directory files and returns None.
+        """Prune the scenario ephemeral directory files and returns None.
 
         "safe files" will not be pruned, including the ansible configuration
         and inventory used by this scenario, the scenario state file, and
         files declared as "safe_files" in the ``driver`` configuration
         declared in ``molecule.yml``.
 
         :return: None
         """
         LOG.info("Pruning extra files from scenario ephemeral directory")
         safe_files = [
             self.config.provisioner.config_file,
             self.config.provisioner.inventory_file,
             self.config.state.state_file,
-        ] + self.config.driver.safe_files
+            *self.config.driver.safe_files,
+        ]
         files = util.os_walk(self.ephemeral_directory, "*")
         for f in files:
             if not any(sf for sf in safe_files if fnmatch.fnmatch(f, sf)):
                 try:
                     os.remove(f)
                 except OSError as e:
                     if e.errno != errno.ENOENT:
@@ -106,15 +105,17 @@
         if not path:
             project_directory = os.path.basename(self.config.project_directory)
 
             if self.config.is_parallel:
                 project_directory = f"{project_directory}-{self.config._run_uuid}"
 
             project_scenario_directory = os.path.join(
-                self.config.cache_directory, project_directory, self.name
+                self.config.cache_directory,
+                project_directory,
+                self.name,
             )
 
             path = ephemeral_directory(project_scenario_directory)
 
         if os.environ.get("MOLECULE_PARALLEL", False) and not self._lock:
             with open(os.path.join(path, ".lock"), "w") as self._lock:
                 for i in range(1, 5):
@@ -200,26 +201,24 @@
                 raise RuntimeError("Unexpected sequence type {result}.")
         except KeyError:
             # TODO(retr0h): May change this handling in the future.
             pass
         return result
 
     def _setup(self):
-        """
-        Prepare the scenario for Molecule and returns None.
+        """Prepare the scenario for Molecule and returns None.
 
         :return: None
         """
         if not os.path.isdir(self.inventory_directory):
             os.makedirs(self.inventory_directory, exist_ok=True)
 
 
 def ephemeral_directory(path: Optional[str] = None) -> str:
-    """
-    Return temporary directory to be used by molecule.
+    """Return temporary directory to be used by molecule.
 
     Molecule users should not make any assumptions about its location,
     permissions or its content as this may change in future release.
     """
     d = os.getenv("MOLECULE_EPHEMERAL_DIRECTORY")
     if not d:
         d = os.getenv("XDG_CACHE_HOME", os.path.expanduser("~/.cache"))
```

### Comparing `molecule-5.0.0a0/src/molecule/scenarios.py` & `molecule-5.0.0a1/src/molecule/scenarios.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 """Scenarios Module."""
 import logging
-from typing import List
 
 from molecule import util
 
 LOG = logging.getLogger(__name__)
 
 
-class Scenarios(object):
+class Scenarios:
     """The Scenarios groups one or more scenario objects Molecule will execute."""
 
-    def __init__(self, configs, scenario_name=None):
-        """
-        Initialize a new scenarios class and returns None.
+    def __init__(self, configs, scenario_name=None) -> None:
+        """Initialize a new scenarios class and returns None.
 
         :param configs: A list containing Molecule config instances.
         :param scenario_name: A string containing the name of the scenario.
         :return: None
         """
         self._configs = configs
         self._scenario_name = scenario_name
@@ -50,16 +48,15 @@
         """Make object iterable."""
         return self
 
     __next__ = next  # Python 3.X compatibility
 
     @property
     def all(self):
-        """
-        Return a list containing all scenario objects.
+        """Return a list containing all scenario objects.
 
         :return: list
         """
         if self._scenario_name:
             scenarios = self._filter_for_scenario()
             self._verify()
 
@@ -71,48 +68,45 @@
 
     def print_matrix(self):
         msg = "Test matrix"
         LOG.info(msg)
 
         tree = {}
         for scenario in self.all:
-            tree[scenario.name] = [action for action in scenario.sequence]
+            tree[scenario.name] = list(scenario.sequence)
         util.print_as_yaml(tree)
 
-    def sequence(self, scenario_name: str) -> List[str]:
+    def sequence(self, scenario_name: str) -> list[str]:
         for scenario in self.all:
             if scenario.name == scenario_name:
-                return [action for action in scenario.sequence]
+                return list(scenario.sequence)
         raise RuntimeError(f"Unable to find sequence for {scenario_name} scenario.")
 
     def _verify(self):
-        """
-        Verify the specified scenario was found and returns None.
+        """Verify the specified scenario was found and returns None.
 
         :return: None
         """
         scenario_names = [c.scenario.name for c in self._configs]
         if self._scenario_name not in scenario_names:
             msg = f"Scenario '{self._scenario_name}' not found.  Exiting."
             util.sysexit_with_message(msg)
 
     def _filter_for_scenario(self):
-        """
-        Find the scenario matching the provided scenario name and returns a \
+        """Find the scenario matching the provided scenario name and returns a \
         list.
 
         :return: list
         """
         return [
             c.scenario for c in self._configs if c.scenario.name == self._scenario_name
         ]
 
     def _get_matrix(self):
-        """
-        Build a matrix of scenarios with sequence to include and returns a \
+        """Build a matrix of scenarios with sequence to include and returns a \
         dict.
 
         {
             scenario_1: {
                 'subcommand': [
                     'action-1',
                     'action-2',
@@ -140,9 +134,9 @@
                     "prepare": scenario.prepare_sequence,
                     "side_effect": scenario.side_effect_sequence,
                     "syntax": scenario.syntax_sequence,
                     "test": scenario.test_sequence,
                     "verify": scenario.verify_sequence,
                 }
                 for scenario in self.all
-            }
+            },
         )
```

### Comparing `molecule-5.0.0a0/src/molecule/shell.py` & `molecule-5.0.0a1/src/molecule/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,20 +104,23 @@
 @click.option(
     "--env-file",
     "-e",
     default=ENV_FILE,
     help=("The file to read variables from when rendering molecule.yml. " "(.env.yml)"),
 )
 @click.option(
-    "--version", is_flag=True, callback=print_version, expose_value=False, is_eager=True
+    "--version",
+    is_flag=True,
+    callback=print_version,
+    expose_value=False,
+    is_eager=True,
 )
 @click.pass_context
 def main(ctx, debug, verbose, base_config, env_file):  # pragma: no cover
-    """
-    Molecule aids in the development and testing of Ansible roles.
+    """Molecule aids in the development and testing of Ansible roles.
 
     To enable autocomplete for a supported shell execute command below after
     replacing SHELL with either bash, zsh, or fish:
 
         eval "$(_MOLECULE_COMPLETE=SHELL_source molecule)"
     """
     ctx.obj = {}
```

### Comparing `molecule-5.0.0a0/src/molecule/state.py` & `molecule-5.0.0a1/src/molecule/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 
 class InvalidState(Exception):
     """Exception class raised when an error occurs in :class:`.State`."""
 
 
-class State(object):
+class State:
     """A class which manages the state file.
 
     Intended to be used as a singleton throughout a given Molecule config.
     The initial state is serialized to disk if the file does not exist,
     otherwise is deserialized from the existing state file.  Changes made to
     the object are immediately serialized.
 
@@ -54,25 +54,24 @@
 
     !!! note
 
         Currently, it's use is significantly smaller than it was in v1 of
         Molecule.
     """
 
-    def __init__(self, config):
-        """
-        Initialize a new state class and returns None.
+    def __init__(self, config) -> None:
+        """Initialize a new state class and returns None.
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
-        self._state_file = self._get_state_file()
-        self._data = self._get_data()
-        self._write_state_file()
+        self._state_file = self._get_state_file()  # type: ignore
+        self._data = self._get_data()  # type: ignore
+        self._write_state_file()  # type: ignore
 
     def marshal(func):
         def wrapper(self, *args, **kwargs):
             func(self, *args, **kwargs)
             self._write_state_file()
 
         return wrapper
@@ -111,16 +110,15 @@
 
     @marshal  # type: ignore
     def reset(self):
         self._data = self._default_data()
 
     @marshal  # type: ignore
     def change_state(self, key, value):
-        """
-        Change the state of the instance data with the given \
+        """Change the state of the instance data with the given \
         ``key`` and the provided ``value``.
 
         Wrapping with a decorator is probably not necessary.
 
         :param key: A ``str`` containing the key to update
         :param value: A value to change the ``key`` to
         :return: None
```

### Comparing `molecule-5.0.0a0/src/molecule/status.py` & `molecule-5.0.0a1/src/molecule/status.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/conftest.py` & `molecule-5.0.0a1/src/molecule/test/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,46 +34,46 @@
     # Checks if first dict is a subset of the second one
     if isinstance(subset, dict):
         return all(
             key in superset and is_subset(val, superset[key])
             for key, val in subset.items()
         )
 
-    if isinstance(subset, list) or isinstance(subset, set):
+    if isinstance(subset, (list, set)):
         return all(
             any(is_subset(subitem, superitem) for superitem in superset)
             for subitem in subset
         )
 
     # assume that subset is a plain value if none of the above match
     return subset == superset
 
 
-@pytest.fixture
+@pytest.fixture()
 def random_string(l=5):
     return "".join(random.choice(string.ascii_uppercase) for _ in range(l))
 
 
 @contextlib.contextmanager
 def change_dir_to(dir_name):
     cwd = os.getcwd()
     os.chdir(dir_name)
     yield
     os.chdir(cwd)
 
 
-@pytest.fixture
+@pytest.fixture()
 def temp_dir(tmpdir, random_string, request):
     directory = tmpdir.mkdir(random_string)
 
     with change_dir_to(directory.strpath):
         yield directory
 
 
-@pytest.fixture
+@pytest.fixture()
 def resources_folder_path():
     resources_folder_path = os.path.join(os.path.dirname(__file__), "resources")
     return resources_folder_path
 
 
 def molecule_project_directory() -> str:
     return os.getcwd()
@@ -96,15 +96,15 @@
 
 
 def molecule_ephemeral_directory(_fixture_uuid) -> str:
     project_directory = f"test-project-{_fixture_uuid}"
     scenario_name = "test-instance"
 
     return ephemeral_directory(
-        os.path.join("molecule_test", project_directory, scenario_name)
+        os.path.join("molecule_test", project_directory, scenario_name),
     )
 
 
 def pytest_collection_modifyitems(items, config):
     marker = config.getoption("-m")
     is_sharded = False
     shard_id = 0
@@ -118,15 +118,15 @@
         is_sharded = True
     else:
         raise ValueError("shard_{}_of_{} marker is invalid")
     if not is_sharded:
         return
     if not 0 < shard_id <= shards_num:
         raise ValueError(
-            "shard_id must be greater than 0 and not bigger than shards_num"
+            "shard_id must be greater than 0 and not bigger than shards_num",
         )
     for test_counter, item in enumerate(items):
         cur_shard_id = test_counter % shards_num + 1
         marker = getattr(pytest.mark, f"shard_{cur_shard_id}_of_{shards_num}")
         item.add_marker(marker)
     del marker
     print(f"Running sharded test group #{shard_id} out of {shards_num}")
```

### Comparing `molecule-5.0.0a0/src/molecule/test/functional/.ansible-lint` & `molecule-5.0.0a1/src/molecule/test/functional/.ansible-lint`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/functional/conftest.py` & `molecule-5.0.0a1/src/molecule/test/functional/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,18 @@
 
 def _env_vars_exposed(env_vars, env=os.environ):
     """Check if environment variables are exposed and populated."""
     for env_var in env_vars:
         if env_var not in os.environ:
             return False
         return os.environ[env_var] != ""
+    return None
 
 
-@pytest.fixture
+@pytest.fixture()
 def with_scenario(request, scenario_to_test, driver_name, scenario_name, skip_test):
     scenario_directory = os.path.join(
         os.path.dirname(util.abs_path(__file__)),
         os.path.pardir,
         "scenarios",
         scenario_to_test,
     )
@@ -75,15 +76,15 @@
         if scenario_name:
             msg = "CLEANUP: Destroying instances for all scenario(s)"
             LOG.info(msg)
             cmd = ["molecule", "destroy", "--driver-name", driver_name, "--all"]
             assert run_command(cmd).returncode == 0
 
 
-@pytest.fixture
+@pytest.fixture()
 def skip_test(request, driver_name):
     msg_tmpl = "Skipped '{}' not supported"
     support_checks_map = {
         "delegated": lambda: True,
     }
     try:
         check_func = support_checks_map[driver_name]
@@ -235,25 +236,25 @@
     return shutil.which("VBoxManage")
 
 
 @cache
 def supports_docker() -> bool:
     docker = get_docker_executable()
     if docker:
-        result = subprocess.run([docker, "info"], stdout=PIPE, universal_newlines=True)
+        result = subprocess.run([docker, "info"], stdout=PIPE, text=True)
         if result.returncode != 0:
             LOG.error(
                 "Error %s returned from `docker info`: %s",
                 result.returncode,
                 result.stdout,
             )
             return False
         if "BuildahVersion" in result.stdout:
             LOG.error(
-                "podman-docker is unsupported, see https://github.com/ansible-community/molecule/issues/2456"
+                "podman-docker is unsupported, see https://github.com/ansible-community/molecule/issues/2456",
             )
             return False
     return True
 
 
 def min_ansible(version: str) -> bool:
     """Ensure current Ansible is newer than a given a minimal one."""
```

### Comparing `molecule-5.0.0a0/src/molecule/test/functional/test_command.py` & `molecule-5.0.0a1/src/molecule/test/functional/test_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,106 +31,103 @@
     list_with_format_plain,
     run_test,
     verify,
 )
 from molecule.util import run_command
 
 
-@pytest.fixture
+@pytest.fixture()
 def scenario_to_test(request):
     return request.param
 
 
-@pytest.fixture
+@pytest.fixture()
 def scenario_name(request):
     try:
         return request.param
     except AttributeError:
         return None
 
 
-@pytest.fixture
+@pytest.fixture()
 def driver_name(request: FixtureRequest) -> Optional[str]:
     try:
         # https://stackoverflow.com/q/65334215/99834
         return request.param  # type: ignore
     except AttributeError:
         return None
 
 
-@pytest.fixture
+@pytest.fixture()
 def platform_name(request):
     try:
         return request.param
     except AttributeError:
         return None
 
 
-@pytest.mark.extensive
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_check(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "check", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.extensive
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
-@pytest.mark.serial
+@pytest.mark.serial()
 def test_command_cleanup(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "cleanup", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.extensive
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
-@pytest.mark.serial
+@pytest.mark.serial()
 def test_command_converge(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "converge", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.extensive
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
-@pytest.mark.serial
+@pytest.mark.serial()
 def test_command_create(scenario_to_test, with_scenario, scenario_name, tmp_path):
     cmd = ["molecule", "create", "--scenario-name", scenario_name]
     assert run_command(cmd, env=os.environ).returncode == 0
 
     # TODO(ssbarnea): Include these additional checks
-    # role_list = run_command(["ansible-galaxy", "role", "list"], env=os.environ)
-    # assert role_list.returncode == 0, role_list
-    # assert "- molecule.delegated_test, (unknown version)" in role_list.stdout
 
 
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         pytest.param(
             "dependency",
             "delegated",
             "shell",
             id="shell",
         ),
@@ -139,64 +136,64 @@
             "delegated",
             "ansible-galaxy",
             id="galaxy",
         ),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
-@pytest.mark.serial
+@pytest.mark.serial()
 def test_command_dependency(request, scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "dependency", "--scenario-name", scenario_name]
     assert run_command(cmd, echo=True).returncode == 0
 
     # Validate that dependency worked by running converge, which make use
     cmd = ["molecule", "converge", "--scenario-name", scenario_name]
     assert run_command(cmd, echo=True).returncode == 0
 
 
-@pytest.mark.serial
-@pytest.mark.extensive
+@pytest.mark.serial()
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [("driver/delegated", "delegated", "default")],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_destroy(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "destroy", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.serial
-@pytest.mark.extensive
+@pytest.mark.serial()
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_idempotence(scenario_to_test, with_scenario, scenario_name):
     idempotence(scenario_name)
 
 
-@pytest.mark.serial
+@pytest.mark.serial()
 @pytest.mark.parametrize("driver_name", [("delegated")], indirect=["driver_name"])
 def test_command_init_role(temp_dir, driver_name):
     init_role(temp_dir, driver_name)
 
 
-@pytest.mark.serial
+@pytest.mark.serial()
 @pytest.mark.parametrize("driver_name", [("delegated")], indirect=["driver_name"])
 def test_command_init_scenario(temp_dir, driver_name):
     init_scenario(temp_dir, driver_name)
 
 
-@pytest.mark.serial
+@pytest.mark.serial()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, expected",
+    ("scenario_to_test", "driver_name", "expected"),
     [
         (
             "driver/delegated",
             "delegated",
             "instance        delegated       ansible default",
         ),
     ],
@@ -204,87 +201,84 @@
 )
 def test_command_list_with_format_plain(scenario_to_test, with_scenario, expected):
     list_with_format_plain(expected)
 
 
 # @pytest.mark.parametrize(
 #     "scenario_to_test, driver_name, login_args, scenario_name",
-#     [
-#         (
 #             "driver/delegated",
 #             "delegated",
-#             [["instance", ".*instance.*"]],
 #             "default",
 #         ),
 #     ],
-#     indirect=["scenario_to_test", "driver_name", "scenario_name"],
-# )
 # def test_command_login(scenario_to_test, with_scenario, login_args, scenario_name):
-#     login(login_args, scenario_name)
 
 
-@pytest.mark.serial
-@pytest.mark.extensive
+@pytest.mark.serial()
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_prepare(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "create", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
     cmd = ["molecule", "prepare", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.serial
-@pytest.mark.extensive
+@pytest.mark.serial()
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_side_effect(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "side-effect", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.serial
-@pytest.mark.extensive
+@pytest.mark.serial()
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_syntax(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "syntax", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.serial
+@pytest.mark.serial()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_test(scenario_to_test, with_scenario, scenario_name, driver_name):
     run_test(driver_name, scenario_name)
 
 
 def run_test_with_platform_name(
-    driver_name, platform_name, scenario_name="default", parallel=False
+    driver_name,
+    platform_name,
+    scenario_name="default",
+    parallel=False,
 ):
     cmd = [
         "molecule",
         "-vvv",
         "--debug",
         "test",
         "--scenario-name",
@@ -297,59 +291,67 @@
             cmd.append("--all")
         if parallel:
             cmd.append("--parallel")
 
     assert run_command(cmd).returncode == 0
 
 
-@pytest.mark.serial
+@pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name", "platform_name"),
     [
         ("driver/delegated", "delegated", "default", "instance"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name", "platform_name"],
 )
 def test_command_test_with_platform_name(
-    scenario_to_test, with_scenario, scenario_name, driver_name, platform_name
+    scenario_to_test,
+    with_scenario,
+    scenario_name,
+    driver_name,
+    platform_name,
 ):
     run_test_with_platform_name(driver_name, platform_name, scenario_name)
 
 
-@pytest.mark.serial
+@pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
         (
             "driver/delegated_invalid_role_name_with_role_name_check_equals_to_1",
             "delegated",
             "default",
         ),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_test_with_role_name_check_equals_to_1(
-    scenario_to_test, with_scenario, scenario_name, driver_name
+    scenario_to_test,
+    with_scenario,
+    scenario_name,
+    driver_name,
 ):
     run_test(driver_name, scenario_name)
 
 
-@pytest.mark.serial
-@pytest.mark.extensive
+@pytest.mark.serial()
+@pytest.mark.extensive()
 @pytest.mark.parametrize(
-    "scenario_to_test, driver_name, scenario_name",
+    ("scenario_to_test", "driver_name", "scenario_name"),
     [
         ("driver/delegated", "delegated", "default"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_verify(scenario_to_test, with_scenario, scenario_name):
     verify(scenario_name)
 
 
 def test_sample_collection():
     assert (
         run_command(
-            ["molecule", "test"], cwd="src/molecule/test/resources/sample-collection"
+            ["molecule", "test"],
+            cwd="src/molecule/test/resources/sample-collection",
         ).returncode
         == 0
     )
```

### Comparing `molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml` & `molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml` & `molecule-5.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py` & `molecule-5.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Testinfra tests."""
 
 import os
 
 import testinfra.utils.ansible_runner
 
 testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
-    os.environ["MOLECULE_INVENTORY_FILE"]
+    os.environ["MOLECULE_INVENTORY_FILE"],
 ).get_hosts("all")
 
 
 def test_hostname(host):
     """Validate hostname."""
-    assert "instance" == host.check_output("hostname -s")
+    assert host.check_output("hostname -s") == "instance"
 
 
 def test_etc_molecule_directory(host):
     """Validate molecule directory."""
     f = host.file("/etc/molecule")
 
     assert f.is_directory
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/conftest.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,30 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 import pytest
 
 
-@pytest.fixture
+@pytest.fixture()
 def command_patched_ansible_create(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.create")
 
 
-@pytest.fixture
+@pytest.fixture()
 def command_driver_delegated_section_data():
     x = {
         "driver": {
             "name": "delegated",
             "options": {
                 "managed": False,
-                # "login_cmd_template": "docker exec -ti {instance} bash",
-                # "ansible_connection_options": {"ansible_connection": "docker"},
             },
-        }
+        },
     }
     # if "DOCKER_HOST" in os.environ:
     #     x["driver"]["options"]["ansible_docker_extra_args"] = "-H={}".format(
-    #         os.environ["DOCKER_HOST"]
-    #     )
     return x
 
 
-@pytest.fixture
+@pytest.fixture()
 def command_driver_delegated_managed_section_data():
     return {"driver": {"name": "delegated", "managed": True}}
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/init/test_role.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/init/test_role.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 
 import pytest
 
 from molecule.command.init import role
 
 
-@pytest.fixture
+@pytest.fixture()
 def _command_args():
     return {
         "dependency_name": "galaxy",
         "driver_name": "delegated",
         "provisioner_name": "ansible",
         "role_name": "acme.test_role",
         "scenario_name": "default",
         "subcommand": __name__,
         "verifier_name": "ansible",
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_command_args):
     return role.Role(_command_args)
 
 
 def test_execute(temp_dir, _instance, patched_logger_info):
     _instance.execute()
 
@@ -59,11 +59,11 @@
 
 def test_execute_role_exists(temp_dir, _instance, patched_logger_critical):
     _instance.execute()
 
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "The directory test_role exists. Cannot create new role."
     patched_logger_critical.assert_called_once_with(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/init/test_scenario.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/init/test_scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,34 +21,35 @@
 import os
 
 import pytest
 
 from molecule.command.init import scenario
 
 
-@pytest.fixture
+@pytest.fixture()
 def _command_args():
     return {
         "driver_name": "delegated",
         "role_name": "test-role",
         "scenario_name": "test-scenario",
         "subcommand": __name__,
         "verifier_name": "ansible",
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_command_args):
     return scenario.Scenario(_command_args)
 
 
-@pytest.fixture
+@pytest.fixture()
 def invalid_template_dir(resources_folder_path):
     invalid_role_template_path = os.path.join(
-        resources_folder_path, "invalid_scenario_template"
+        resources_folder_path,
+        "invalid_scenario_template",
     )
     return invalid_role_template_path
 
 
 def test_execute(temp_dir, _instance, patched_logger_info):
     _instance.execute()
 
@@ -64,20 +65,23 @@
 
 def test_execute_scenario_exists(temp_dir, _instance, patched_logger_critical):
     _instance.execute()
 
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "The directory molecule/test-scenario exists. " "Cannot create new scenario."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_execute_with_invalid_driver(
-    temp_dir, _instance, _command_args, patched_logger_critical
+    temp_dir,
+    _instance,
+    _command_args,
+    patched_logger_critical,
 ):
     _command_args["driver_name"] = "ec3"
 
     with pytest.raises(KeyError):
         _instance.execute()
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_base.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,60 +32,60 @@
     def execute(self, action_args=None):
         pass
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _base_class(patched_config_validate, config_instance):
     return ExtendedBase
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_base_class, config_instance):
     return _base_class(config_instance)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_base_setup(mocker):
     return mocker.patch("molecule.test.unit.command.test_base.ExtendedBase._setup")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_write_config(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.write_config")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_manage_inventory(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.manage_inventory")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_execute_subcommand(mocker):
     return mocker.patch("molecule.command.base.execute_subcommand")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_execute_scenario(mocker):
     return mocker.patch("molecule.command.base.execute_scenario")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_print_matrix(mocker):
     return mocker.patch("molecule.scenarios.Scenarios.print_matrix")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_prune(mocker):
     return mocker.patch("molecule.scenario.Scenario.prune")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_sysexit(mocker):
     return mocker.patch("molecule.util.sysexit")
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -105,15 +105,17 @@
     assert os.path.isfile(_instance._config.config_file)
 
     _patched_manage_inventory.assert_called_once_with()
     _patched_write_config.assert_called_once_with()
 
 
 def test_execute_cmdline_scenarios(
-    config_instance, _patched_print_matrix, _patched_execute_scenario
+    config_instance,
+    _patched_print_matrix,
+    _patched_execute_scenario,
 ):
     # Ensure execute_cmdline_scenarios runs normally:
     # - scenarios.print_matrix is called, which also indicates Scenarios
     #   was instantiated correctly
     # - execute_scenario is called once, indicating the function correctly
     #   loops over Scenarios.
     scenario_name = None
@@ -122,30 +124,34 @@
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_print_matrix.called_once_with()
     assert _patched_execute_scenario.call_count == 1
 
 
 def test_execute_cmdline_scenarios_prune(
-    config_instance, _patched_prune, _patched_execute_subcommand
+    config_instance,
+    _patched_prune,
+    _patched_execute_subcommand,
 ):
     # Subcommands should be executed and prune *should* run when
     # destroy is 'always'
     scenario_name = "default"
     args = {}
     command_args = {"destroy": "always", "subcommand": "test"}
 
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     assert _patched_execute_subcommand.called
     assert _patched_prune.called
 
 
 def test_execute_cmdline_scenarios_no_prune(
-    config_instance, _patched_prune, _patched_execute_subcommand
+    config_instance,
+    _patched_prune,
+    _patched_execute_subcommand,
 ):
     # Subcommands should be executed but prune *should not* run when
     # destroy is 'never'
     scenario_name = "default"
     args = {}
     command_args = {"destroy": "never", "subcommand": "test"}
 
@@ -180,15 +186,18 @@
     assert _patched_execute_subcommand.call_args_list[0][0][1] == "cleanup"
     assert _patched_execute_subcommand.call_args_list[1][0][1] == "destroy"
     assert _patched_prune.called
     assert _patched_sysexit.called
 
 
 def test_execute_cmdline_scenarios_exit_nodestroy(
-    config_instance, _patched_execute_scenario, _patched_prune, _patched_sysexit
+    config_instance,
+    _patched_execute_scenario,
+    _patched_prune,
+    _patched_sysexit,
 ):
     # Ensure execute_cmdline_scenarios handles errors correctly when 'destroy'
     # is 'always':
     # - destroy subcommand is not run when execute_scenario raises SystemExit
     # - scenario is not pruned
     # - caught SystemExit is reraised
     scenario_name = "default"
@@ -217,29 +226,29 @@
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
     home = os.path.expanduser("~")
     cache_dir = config_instance.runtime.cache_dir
     runtime_roles_path = config_instance.runtime.environ.get("ANSIBLE_ROLES_PATH")
     provisioner_roles_path = config_instance.provisioner.env.get("ANSIBLE_ROLES_PATH")
     runtime_collections_path = config_instance.runtime.environ.get(
-        config_instance.ansible_collections_path
+        config_instance.ansible_collections_path,
     )
     provisioner_collections_path = config_instance.provisioner.env.get(
-        config_instance.ansible_collections_path
+        config_instance.ansible_collections_path,
     )
 
     assert runtime_roles_path.startswith(
         f"{cache_dir}/roles:"
         f"{home}/.ansible/roles:"
         f"/usr/share/ansible/roles:"
-        f"/etc/ansible/roles"
+        f"/etc/ansible/roles",
     )
 
     assert runtime_collections_path.startswith(
-        f"{cache_dir}/collections:" f"{home}/.ansible/collections"
+        f"{cache_dir}/collections:" f"{home}/.ansible/collections",
     )
 
     assert provisioner_roles_path.startswith(f"{cache_dir}/roles")
 
     assert provisioner_collections_path.startswith(f"{cache_dir}/collections")
 
 
@@ -279,50 +288,51 @@
 
 def test_get_configs(config_instance):
     molecule_file = config_instance.molecule_file
     data = config_instance.config
     util.write_file(molecule_file, util.safe_dump(data))
 
     result = base.get_configs({}, {})
-    assert 1 == len(result)
+    assert len(result) == 1
     assert isinstance(result, list)
     assert isinstance(result[0], config.Config)
 
 
 def test_verify_configs(config_instance):
     configs = [config_instance]
 
     assert base._verify_configs(configs) is None
 
 
 def test_verify_configs_raises_with_no_configs(patched_logger_critical):
     with pytest.raises(SystemExit) as e:
         base._verify_configs([])
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "'molecule/*/molecule.yml' glob failed.  Exiting."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_verify_configs_raises_with_duplicate_configs(
-    patched_logger_critical, config_instance
+    patched_logger_critical,
+    config_instance,
 ):
     with pytest.raises(SystemExit) as e:
         configs = [config_instance, config_instance]
         base._verify_configs(configs)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "Duplicate scenario name 'default' found.  Exiting."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_get_subcommand():
-    assert "test_base" == base._get_subcommand(__name__)
+    assert base._get_subcommand(__name__) == "test_base"
 
 
 @pytest.mark.parametrize(
     "shell",
     [
         "bash",
         "zsh",
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_check.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_syntax.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,32 +16,34 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
-from molecule.command import check
+from molecule.command import syntax
 
 
-@pytest.fixture
-def _patched_ansible_check(mocker):
-    return mocker.patch("molecule.provisioner.ansible.Ansible.check")
+@pytest.fixture()
+def _patched_ansible_syntax(mocker):
+    return mocker.patch("molecule.provisioner.ansible.Ansible.syntax")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 def test_execute(
     mocker,
     patched_logger_info,
-    _patched_ansible_check,
+    _patched_ansible_syntax,
     patched_config_validate,
     config_instance,
 ):
-    c = check.Check(config_instance)
-    c.execute()
+    s = syntax.Syntax(config_instance)
+    s.execute()
 
     assert len(patched_logger_info.mock_calls) == 1
     name, args, kwargs = patched_logger_info.mock_calls[0]
     assert "default" in args
-    assert "check" in args
+    assert "syntax" in args
+
+    _patched_ansible_syntax.assert_called_once_with()
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_cleanup.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_cleanup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 
 import pytest
 
 from molecule import util
 from molecule.command import cleanup
 
 
-@pytest.fixture
+@pytest.fixture()
 def _command_provisioner_section_with_cleanup_data():
     return {"provisioner": {"name": "ansible", "playbooks": {"cleanup": "cleanup.yml"}}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_cleanup(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.cleanup")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.mark.parametrize(
-    "config_instance", ["_command_provisioner_section_with_cleanup_data"], indirect=True
+    "config_instance",
+    ["_command_provisioner_section_with_cleanup_data"],
+    indirect=True,
 )
 def test_execute(
     mocker,
     _patched_ansible_cleanup,
     patched_logger_info,
     patched_config_validate,
     config_instance,
@@ -59,15 +61,17 @@
     name, args, kwargs = patched_logger_info.mock_calls[0]
     assert "cleanup" in args
 
     _patched_ansible_cleanup.assert_called_once_with()
 
 
 def test_execute_skips_when_playbook_not_configured(
-    patched_logger_warning, _patched_ansible_cleanup, config_instance
+    patched_logger_warning,
+    _patched_ansible_cleanup,
+    config_instance,
 ):
     cu = cleanup.Cleanup(config_instance)
     cu.execute()
 
     msg = "Skipping, cleanup playbook not configured."
     patched_logger_warning.assert_called_once_with(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_converge.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_converge.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_create.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.command import create
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_create_setup(mocker):
     return mocker.patch("molecule.command.create.Create._setup")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
@@ -43,23 +43,25 @@
     c.execute()
 
     assert len(patched_logger_info.mock_calls) == 1
     name, args, kwargs = patched_logger_info.mock_calls[0]
     assert "default" in args
     assert "converge" in args
 
-    assert "delegated" == config_instance.state.driver
+    assert config_instance.state.driver == "delegated"
 
     command_patched_ansible_create.assert_called_once_with()
 
     assert config_instance.state.created
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["command_driver_delegated_section_data"], indirect=True
+    "config_instance",
+    ["command_driver_delegated_section_data"],
+    indirect=True,
 )
 def test_execute_skips_when_delegated_driver(
     _patched_create_setup,
     patched_logger_warning,
     command_patched_ansible_create,
     config_instance,
 ):
@@ -70,15 +72,17 @@
     patched_logger_warning.assert_called_once_with(msg)
 
     assert not command_patched_ansible_create.called
 
 
 @pytest.mark.skip(reason="create not running for delegated")
 def test_execute_skips_when_instances_already_created(
-    patched_logger_warning, command_patched_ansible_create, config_instance
+    patched_logger_warning,
+    command_patched_ansible_create,
+    config_instance,
 ):
     config_instance.state.change_state("created", True)
     c = create.Create(config_instance)
     c.execute()
 
     msg = "Skipping, instances already created."
     patched_logger_warning.assert_called_once_with(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_dependency.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_destroy.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_destroy.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.command import destroy
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_destroy(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.destroy")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_destroy_setup(mocker):
     return mocker.patch("molecule.command.destroy.Destroy._setup")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
@@ -56,15 +56,17 @@
     _patched_ansible_destroy.assert_called_once_with()
 
     assert not config_instance.state.converged
     assert not config_instance.state.created
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["command_driver_delegated_section_data"], indirect=True
+    "config_instance",
+    ["command_driver_delegated_section_data"],
+    indirect=True,
 )
 def test_execute_skips_when_destroy_strategy_is_never(
     _patched_destroy_setup,
     patched_logger_warning,
     _patched_ansible_destroy,
     config_instance,
 ):
@@ -76,15 +78,17 @@
     msg = "Skipping, '--destroy=never' requested."
     patched_logger_warning.assert_called_once_with(msg)
 
     assert not _patched_ansible_destroy.called
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["command_driver_delegated_section_data"], indirect=True
+    "config_instance",
+    ["command_driver_delegated_section_data"],
+    indirect=True,
 )
 def test_execute_skips_when_delegated_driver(
     _patched_destroy_setup,
     patched_logger_warning,
     _patched_ansible_destroy,
     config_instance,
 ):
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_idempotence.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_idempotence.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 import pytest
 
 from molecule.command import idempotence
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_is_idempotent(mocker):
     return mocker.patch("molecule.command.idempotence.Idempotence._is_idempotent")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(patched_config_validate, config_instance):
     config_instance.state.change_state("converged", True)
 
     return idempotence.Idempotence(config_instance)
 
 
 def test_execute(
@@ -56,21 +56,23 @@
     _patched_is_idempotent.assert_called_once_with("patched-ansible-converge-stdout")
 
     msg = "Idempotence completed successfully."
     patched_logger_info.assert_any_call(msg)
 
 
 def test_execute_raises_when_not_converged(
-    patched_logger_critical, patched_ansible_converge, _instance
+    patched_logger_critical,
+    patched_ansible_converge,
+    _instance,
 ):
     _instance._config.state.change_state("converged", False)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "Instances not converged.  Please converge instances first."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_execute_raises_when_fails_idempotence(
     mocker,
@@ -79,15 +81,15 @@
     _patched_is_idempotent,
     _instance,
 ):
     _patched_is_idempotent.return_value = False
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "Idempotence test failed because of the following tasks:\n"
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_is_idempotent(_instance):
     output = """
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_list.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_list.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_login.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.command import login
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     config_instance.state.change_state("created", True)
 
     return login.Login(config_instance)
 
 
 def test_execute(mocker, _instance):
@@ -36,80 +36,83 @@
     _instance.execute()
 
     m.assert_called_once_with("instance-1")
 
 
 @pytest.mark.skip(reason="needs rewrite after switch to delegated")
 @pytest.mark.parametrize(
-    "config_instance", ["command_driver_delegated_managed_section_data"], indirect=True
+    "config_instance",
+    ["command_driver_delegated_managed_section_data"],
+    indirect=True,
 )
 def test_execute_raises_when_not_created(patched_logger_critical, _instance):
     _instance._config.state.change_state("created", False)
 
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "Instances not created.  Please create instances first."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_get_hostname_does_not_match(patched_logger_critical, _instance):
     _instance._config.command_args = {"host": "invalid"}
     hosts = ["instance-1"]
     with pytest.raises(SystemExit) as e:
         _instance._get_hostname(hosts)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = (
         "There are no hosts that match 'invalid'.  You "
         "can only login to valid hosts."
     )
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_get_hostname_exact_match_with_one_host(_instance):
     _instance._config.command_args = {"host": "instance-1"}
     hosts = ["instance-1"]
 
-    assert "instance-1" == _instance._get_hostname(hosts)
+    assert _instance._get_hostname(hosts) == "instance-1"
 
 
 def test_get_hostname_partial_match_with_one_host(_instance):
     _instance._config.command_args = {"host": "inst"}
     hosts = ["instance-1"]
 
-    assert "instance-1" == _instance._get_hostname(hosts)
+    assert _instance._get_hostname(hosts) == "instance-1"
 
 
 def test_get_hostname_exact_match_with_multiple_hosts(_instance):
     _instance._config.command_args = {"host": "instance-1"}
     hosts = ["instance-1", "instance-2"]
 
-    assert "instance-1" == _instance._get_hostname(hosts)
+    assert _instance._get_hostname(hosts) == "instance-1"
 
 
 def test_get_hostname_partial_match_with_multiple_hosts(_instance):
     _instance._config.command_args = {"host": "foo"}
     hosts = ["foo", "fooo"]
 
-    assert "foo" == _instance._get_hostname(hosts)
+    assert _instance._get_hostname(hosts) == "foo"
 
 
 def test_get_hostname_partial_match_with_multiple_hosts_raises(
-    patched_logger_critical, _instance
+    patched_logger_critical,
+    _instance,
 ):
     _instance._config.command_args = {"host": "inst"}
     hosts = ["instance-1", "instance-2"]
     with pytest.raises(SystemExit) as e:
         _instance._get_hostname(hosts)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = (
         "There are 2 hosts that match 'inst'. "
         "You can only login to one at a time.\n\n"
         "Available hosts:\n"
         "instance-1\n"
         "instance-2"
@@ -118,26 +121,27 @@
 
 
 def test_get_hostname_no_host_flag_specified_on_cli(_instance):
     _instance._config.command_args = {}
     hosts = ["instance-1"]
     _instance._get_hostname(hosts)
 
-    assert "instance-1" == _instance._get_hostname(hosts)
+    assert _instance._get_hostname(hosts) == "instance-1"
 
 
 def test_get_hostname_no_host_flag_specified_on_cli_with_multiple_hosts_raises(
-    patched_logger_critical, _instance
+    patched_logger_critical,
+    _instance,
 ):
     _instance._config.command_args = {}
     hosts = ["instance-1", "instance-2"]
     with pytest.raises(SystemExit) as e:
         _instance._get_hostname(hosts)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = (
         "There are 2 running hosts. Please specify "
         "which with --host.\n\n"
         "Available hosts:\n"
         "instance-1\n"
         "instance-2"
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_matrix.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_prepare.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_prepare.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import pytest
 
 from molecule import util
 from molecule.command import prepare
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_prepare(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.prepare")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
@@ -54,40 +54,47 @@
 
     _patched_ansible_prepare.assert_called_once_with()
 
     assert config_instance.state.prepared
 
 
 def test_execute_skips_when_instances_already_prepared(
-    patched_logger_warning, _patched_ansible_prepare, config_instance
+    patched_logger_warning,
+    _patched_ansible_prepare,
+    config_instance,
 ):
     config_instance.state.change_state("prepared", True)
     p = prepare.Prepare(config_instance)
     p.execute()
 
     msg = "Skipping, instances already prepared."
     patched_logger_warning.assert_called_once_with(msg)
 
     assert not _patched_ansible_prepare.called
 
 
 def test_execute_skips_when_playbook_not_configured(
-    patched_logger_warning, _patched_ansible_prepare, config_instance
+    patched_logger_warning,
+    _patched_ansible_prepare,
+    config_instance,
 ):
     p = prepare.Prepare(config_instance)
     p.execute()
 
     msg = "Skipping, prepare playbook not configured."
     patched_logger_warning.assert_called_once_with(msg)
 
     assert not _patched_ansible_prepare.called
 
 
 def test_execute_when_instances_already_prepared_but_force_provided(
-    mocker, patched_logger_warning, _patched_ansible_prepare, config_instance
+    mocker,
+    patched_logger_warning,
+    _patched_ansible_prepare,
+    config_instance,
 ):
     pb = os.path.join(config_instance.scenario.directory, "prepare.yml")
     util.write_file(pb, "")
 
     config_instance.state.change_state("prepared", True)
     config_instance.command_args = {"force": True}
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_side_effect.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_side_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 
 import pytest
 
 from molecule import util
 from molecule.command import side_effect
 
 
-@pytest.fixture
+@pytest.fixture()
 def _command_provisioner_section_with_side_effect_data():
     return {
         "provisioner": {
             "name": "ansible",
             "playbooks": {"side_effect": "side_effect.yml"},
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_side_effect(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.side_effect")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
@@ -67,15 +67,17 @@
     assert "default" in args
     assert "side_effect" in args
 
     _patched_ansible_side_effect.assert_called_once_with(None)
 
 
 def test_execute_skips_when_playbook_not_configured(
-    patched_logger_warning, _patched_ansible_side_effect, config_instance
+    patched_logger_warning,
+    _patched_ansible_side_effect,
+    config_instance,
 ):
     se = side_effect.SideEffect(config_instance)
     se.execute()
 
     msg = "Skipping, side effect playbook not configured."
     patched_logger_warning.assert_called_once_with(msg)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_syntax.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_verify.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,27 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
-
-from molecule.command import syntax
-
-
-@pytest.fixture
-def _patched_ansible_syntax(mocker):
-    return mocker.patch("molecule.provisioner.ansible.Ansible.syntax")
+from molecule.command import verify
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 def test_execute(
     mocker,
     patched_logger_info,
-    _patched_ansible_syntax,
+    patched_default_verifier,
     patched_config_validate,
     config_instance,
 ):
-    s = syntax.Syntax(config_instance)
-    s.execute()
+    v = verify.Verify(config_instance)
+    v.execute()
 
     assert len(patched_logger_info.mock_calls) == 1
     name, args, kwargs = patched_logger_info.mock_calls[0]
     assert "default" in args
-    assert "syntax" in args
-
-    _patched_ansible_syntax.assert_called_once_with()
+    assert "verify" in args
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_test.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_test.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/command/test_verify.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,15 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from molecule.command import verify
+import pytest
 
+from molecule import shell
 
-# NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
-# config.Config._validate from executing.  Thus preventing odd side-effects
-# throughout patched.assert_called unit tests.
-def test_execute(
-    mocker,
-    patched_logger_info,
-    patched_default_verifier,
-    patched_config_validate,
-    config_instance,
-):
-    v = verify.Verify(config_instance)
-    v.execute()
 
-    assert len(patched_logger_info.mock_calls) == 1
-    name, args, kwargs = patched_logger_info.mock_calls[0]
-    assert "default" in args
-    assert "verify" in args
+def test_shell():
+    with pytest.raises(SystemExit):
+        shell.main()
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/conftest.py` & `molecule-5.0.0a1/src/molecule/test/unit/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import copy
 import functools
 import os
 import shutil
+from collections.abc import Generator
 from pathlib import Path
 from subprocess import CompletedProcess
-from typing import Any, Generator, Tuple
+from typing import Any
 from uuid import uuid4
 
 import pytest
 
 from molecule import config, util
 from molecule.test.conftest import (
     molecule_directory,
@@ -38,63 +39,63 @@
 )
 
 
 def write_molecule_file(filename: str, data: Any) -> None:
     util.write_file(filename, util.safe_dump(data))
 
 
-def os_split(s: str) -> Tuple[str, ...]:
+def os_split(s: str) -> tuple[str, ...]:
     rest, tail = os.path.split(s)
     if rest in ("", os.path.sep):
         return (tail,)
-    return os_split(rest) + (tail,)
+    return (*os_split(rest), tail)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_dependency_galaxy_section_data():
     return {"dependency": {"name": "galaxy"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_driver_section_data():
     return {"driver": {"name": "delegated", "options": {"managed": True}}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_platforms_section_data():
     return {
         "platforms": [
             {"name": "instance-1", "groups": ["foo", "bar"], "children": ["child1"]},
             {"name": "instance-2", "groups": ["baz", "foo"], "children": ["child2"]},
-        ]
+        ],
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_provisioner_section_data():
     return {
         "provisioner": {
             "name": "ansible",
             "options": {"become": True},
             "config_options": {},
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_scenario_section_data():
     return {"scenario": {"name": "default"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_verifier_section_data():
     return {"verifier": {"name": "ansible"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def molecule_data(
     _molecule_dependency_galaxy_section_data,
     _molecule_driver_section_data,
     _molecule_platforms_section_data,
     _molecule_provisioner_section_data,
     _molecule_scenario_section_data,
     _molecule_verifier_section_data,
@@ -107,47 +108,50 @@
         _molecule_scenario_section_data,
         _molecule_verifier_section_data,
     ]
 
     return functools.reduce(lambda x, y: util.merge_dicts(x, y), fixtures)
 
 
-@pytest.fixture
+@pytest.fixture()
 def molecule_directory_fixture(temp_dir):
     return molecule_directory()
 
 
-@pytest.fixture
+@pytest.fixture()
 def molecule_scenario_directory_fixture(molecule_directory_fixture):
     path = molecule_scenario_directory()
     if not os.path.isdir(path):
         os.makedirs(path, exist_ok=True)
 
     return path
 
 
-@pytest.fixture
+@pytest.fixture()
 def molecule_ephemeral_directory_fixture(molecule_scenario_directory_fixture):
     path = molecule_ephemeral_directory(str(uuid4()))
     if not os.path.isdir(path):
         os.makedirs(path, exist_ok=True)
     yield
     shutil.rmtree(str(Path(path).parent))
 
 
-@pytest.fixture
+@pytest.fixture()
 def molecule_file_fixture(
-    molecule_scenario_directory_fixture, molecule_ephemeral_directory_fixture
+    molecule_scenario_directory_fixture,
+    molecule_ephemeral_directory_fixture,
 ):
     return molecule_file()
 
 
-@pytest.fixture
+@pytest.fixture()
 def config_instance(
-    molecule_file_fixture: str, molecule_data, request
+    molecule_file_fixture: str,
+    molecule_data,
+    request,
 ) -> Generator[config.Config, None, None]:
     mdc = copy.deepcopy(molecule_data)
     if hasattr(request, "param"):
         mdc = util.merge_dicts(mdc, request.getfixturevalue(request.param))
     write_molecule_file(molecule_file_fixture, mdc)
 
     _environ = dict(os.environ)
@@ -158,80 +162,83 @@
     os.environ.clear()
     os.environ.update(_environ)
 
 
 # Mocks
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_print_debug(mocker):
     return mocker.patch("molecule.util.print_debug")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_logger_info(mocker):
     return mocker.patch("logging.Logger.info")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_logger_debug(mocker):
     return mocker.patch("logging.Logger.debug")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_logger_warning(mocker):
     return mocker.patch("logging.Logger.warning")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_logger_error(mocker):
     return mocker.patch("logging.Logger.error")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_logger_critical(mocker):
     return mocker.patch("logging.Logger.critical")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_run_command(mocker):
     m = mocker.patch("molecule.util.run_command")
     m.return_value = CompletedProcess(
-        args="foo", returncode=0, stdout="patched-run-command-stdout", stderr=""
+        args="foo",
+        returncode=0,
+        stdout="patched-run-command-stdout",
+        stderr="",
     )
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_ansible_converge(mocker):
     m = mocker.patch("molecule.provisioner.ansible.Ansible.converge")
     m.return_value = "patched-ansible-converge-stdout"
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_add_or_update_vars(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible._add_or_update_vars")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_ansible_galaxy(mocker):
     return mocker.patch("molecule.dependency.ansible_galaxy.AnsibleGalaxy.execute")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_default_verifier(mocker):
     return mocker.patch("molecule.verifier.ansible.Ansible.execute")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_scenario_setup(mocker):
     mocker.patch("molecule.config.Config.env")
 
     return mocker.patch("molecule.scenario.Scenario._setup")
 
 
-@pytest.fixture
+@pytest.fixture()
 def patched_config_validate(mocker):
     return mocker.patch("molecule.config.Config._validate")
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/cookiecutter/test_molecule.py` & `molecule-5.0.0a1/src/molecule/test/unit/cookiecutter/test_molecule.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,45 +27,49 @@
 from molecule.model import schema_v3
 
 
 class CommandBase(base.Base):
     """CommandBase Class."""
 
 
-@pytest.fixture
+@pytest.fixture()
 def _base_class():
     return CommandBase
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_base_class):
     return _base_class()
 
 
-@pytest.fixture
+@pytest.fixture()
 def _role_directory():
     return "."
 
 
-@pytest.fixture
+@pytest.fixture()
 def _command_args():
     return {
         "dependency_name": "galaxy",
         "driver_name": "delegated",
         "provisioner_name": "ansible",
         "scenario_name": "default",
         "role_name": "test-role",
         "verifier_name": "ansible",
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_file(_role_directory):
     return os.path.join(
-        _role_directory, "test-role", "molecule", "default", "molecule.yml"
+        _role_directory,
+        "test-role",
+        "molecule",
+        "default",
+        "molecule.yml",
     )
 
 
 def test_valid(temp_dir, _molecule_file, _role_directory, _command_args, _instance):
     _instance._process_templates("molecule", _command_args, _role_directory)
 
     data = util.safe_load_file(_molecule_file)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py` & `molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,52 +22,50 @@
 
 import pytest
 
 from molecule import config
 from molecule.dependency.ansible_galaxy import collections
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_galaxy_has_requirements_file(mocker):
     m = mocker.patch(
-        (
-            "molecule.dependency.ansible_galaxy.collections."
-            "Collections._has_requirements_file"
-        )
+        "molecule.dependency.ansible_galaxy.collections."
+        "Collections._has_requirements_file",
     )
     m.return_value = True
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def _dependency_section_data():
     return {
         "dependency": {
             "name": "galaxy",
             "options": {"foo": "bar", "v": True, "role-file": "bar.yml"},
             "env": {"FOO": "bar"},
-        }
+        },
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(_dependency_section_data, patched_config_validate, config_instance):
     return collections.Collections(config_instance)
 
 
-@pytest.fixture
+@pytest.fixture()
 def role_file(_instance):
     return os.path.join(_instance._config.scenario.directory, "collections.yml")
 
 
-@pytest.fixture
+@pytest.fixture()
 def roles_path(_instance):
     return os.path.join(_instance._config.scenario.ephemeral_directory, "collections")
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -84,15 +82,15 @@
     assert "MOLECULE_FILE" in env
     assert "MOLECULE_INVENTORY_FILE" in env
     assert "MOLECULE_SCENARIO_DIRECTORY" in env
     assert "MOLECULE_INSTANCE_CONFIG" in env
 
 
 def test_name_property(_instance):
-    assert "galaxy" == _instance.name
+    assert _instance.name == "galaxy"
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
@@ -120,15 +118,15 @@
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_env_property(_instance):
-    assert "bar" == _instance.env["FOO"]
+    assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_collections_bake(_instance, role_file, roles_path):
     _instance.bake()
     args = [
         "ansible-galaxy",
@@ -152,28 +150,33 @@
     patched_logger_info,
     _instance,
 ):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
     role_directory = os.path.join(
-        _instance._config.scenario.directory, _instance.options["collections-path"]
+        _instance._config.scenario.directory,
+        _instance.options["collections-path"],
     )
     assert os.path.isdir(role_directory)
 
     patched_run_command.assert_called_once_with(
-        "patched-command", debug=False, check=True
+        "patched-command",
+        debug=False,
+        check=True,
     )
 
     msg = "Dependency completed successfully."
     patched_logger_info.assert_called_once_with(msg)
 
 
 def test_execute_does_not_execute_when_disabled(
-    patched_run_command, patched_logger_warning, _instance
+    patched_run_command,
+    patched_logger_warning,
+    _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
@@ -201,30 +204,33 @@
     role_file,
     _patched_ansible_galaxy_has_requirements_file,
     roles_path,
 ):
     _instance.execute()
     assert _instance._sh_command is not None
 
-    assert 1 == patched_run_command.call_count
+    assert patched_run_command.call_count == 1
 
 
 def test_collections_executes_catches_and_exits_return_code(
-    patched_run_command, _patched_ansible_galaxy_has_requirements_file, _instance
+    patched_run_command,
+    _patched_ansible_galaxy_has_requirements_file,
+    _instance,
 ):
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
 
 def test_setup(_instance):
     role_directory = os.path.join(
-        _instance._config.scenario.directory, _instance.options["collections-path"]
+        _instance._config.scenario.directory,
+        _instance.options["collections-path"],
     )
     assert not os.path.isdir(role_directory)
 
     _instance._setup()
 
     assert os.path.isdir(role_directory)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py` & `molecule-5.0.0a1/src/molecule/test/unit/dependency/ansible_galaxy/test_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,49 +22,49 @@
 
 import pytest
 
 from molecule import config
 from molecule.dependency.ansible_galaxy import roles
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_galaxy_has_requirements_file(mocker):
     m = mocker.patch(
-        ("molecule.dependency.ansible_galaxy.roles." "Roles._has_requirements_file")
+        "molecule.dependency.ansible_galaxy.roles." "Roles._has_requirements_file",
     )
     m.return_value = True
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def _dependency_section_data():
     return {
         "dependency": {
             "name": "galaxy",
             "options": {"foo": "bar", "v": True, "requirements-file": "foo.yml"},
             "env": {"FOO": "bar"},
-        }
+        },
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(_dependency_section_data, patched_config_validate, config_instance):
     return roles.Roles(config_instance)
 
 
-@pytest.fixture
+@pytest.fixture()
 def role_file(_instance):
     return os.path.join(_instance._config.scenario.directory, "requirements.yml")
 
 
-@pytest.fixture
+@pytest.fixture()
 def roles_path(_instance):
     return os.path.join(_instance._config.scenario.ephemeral_directory, "roles")
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -81,15 +81,15 @@
     assert "MOLECULE_FILE" in env
     assert "MOLECULE_INVENTORY_FILE" in env
     assert "MOLECULE_SCENARIO_DIRECTORY" in env
     assert "MOLECULE_INSTANCE_CONFIG" in env
 
 
 def test_name_property(_instance):
-    assert "galaxy" == _instance.name
+    assert _instance.name == "galaxy"
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
@@ -117,15 +117,15 @@
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_env_property(_instance):
-    assert "bar" == _instance.env["FOO"]
+    assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_galaxy_bake(_instance, role_file, roles_path):
     _instance.bake()
     args = [
         "ansible-galaxy",
@@ -148,28 +148,33 @@
     patched_logger_info,
     _instance,
 ):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
     role_directory = os.path.join(
-        _instance._config.scenario.directory, _instance.options["roles-path"]
+        _instance._config.scenario.directory,
+        _instance.options["roles-path"],
     )
     assert os.path.isdir(role_directory)
 
     patched_run_command.assert_called_once_with(
-        "patched-command", debug=False, check=True
+        "patched-command",
+        debug=False,
+        check=True,
     )
 
     msg = "Dependency completed successfully."
     patched_logger_info.assert_called_once_with(msg)
 
 
 def test_execute_does_not_execute_when_disabled(
-    patched_run_command, patched_logger_warning, _instance
+    patched_run_command,
+    patched_logger_warning,
+    _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
@@ -197,30 +202,33 @@
     role_file,
     _patched_ansible_galaxy_has_requirements_file,
     roles_path,
 ):
     _instance.execute()
     assert _instance._sh_command is not None
 
-    assert 1 == patched_run_command.call_count
+    assert patched_run_command.call_count == 1
 
 
 def test_galaxy_executes_catches_and_exits_return_code(
-    patched_run_command, _patched_ansible_galaxy_has_requirements_file, _instance
+    patched_run_command,
+    _patched_ansible_galaxy_has_requirements_file,
+    _instance,
 ):
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
 
 def test_setup(_instance):
     role_directory = os.path.join(
-        _instance._config.scenario.directory, _instance.options["roles-path"]
+        _instance._config.scenario.directory,
+        _instance.options["roles-path"],
     )
     assert not os.path.isdir(role_directory)
 
     _instance._setup()
 
     assert os.path.isdir(role_directory)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/dependency/test_shell.py` & `molecule-5.0.0a1/src/molecule/test/unit/dependency/test_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import pytest
 
 from molecule import config
 from molecule.dependency import shell
 
 
-@pytest.fixture
+@pytest.fixture()
 def _dependency_section_data():
     return {
         "dependency": {
             "name": "shell",
             "command": "ls -l -a /tmp",
             "options": {"foo": "bar"},
             "env": {"FOO": "bar"},
-        }
+        },
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(_dependency_section_data, patched_config_validate, config_instance):
     return shell.Shell(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -59,15 +59,15 @@
     assert "MOLECULE_INVENTORY_FILE" in _instance.default_env
     assert "MOLECULE_SCENARIO_DIRECTORY" in _instance.default_env
     assert "MOLECULE_INSTANCE_CONFIG" in _instance.default_env
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_name_property(_instance):
-    assert "shell" == _instance.name
+    assert _instance.name == "shell"
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
@@ -83,31 +83,35 @@
     x = {"foo": "bar"}
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_env_property(_instance):
-    assert "bar" == _instance.env["FOO"]
+    assert _instance.env["FOO"] == "bar"
 
 
 def test_execute(patched_run_command, patched_logger_info, _instance):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
     patched_run_command.assert_called_once_with(
-        "patched-command", debug=False, check=True
+        "patched-command",
+        debug=False,
+        check=True,
     )
 
     msg = "Dependency completed successfully."
     patched_logger_info.assert_called_once_with(msg)
 
 
 def test_execute_does_not_execute_when_disabled(
-    patched_run_command, patched_logger_warning, _instance
+    patched_run_command,
+    patched_logger_warning,
+    _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
@@ -115,15 +119,15 @@
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_execute_bakes(patched_run_command, _instance):
     _instance.execute()
     assert _instance._sh_command is not None
 
-    assert 1 == patched_run_command.call_count
+    assert patched_run_command.call_count == 1
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_dep_executes_catches_and_exits_return_code(patched_run_command, _instance):
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/driver/test_delegated.py` & `molecule-5.0.0a1/src/molecule/test/unit/driver/test_delegated.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,39 +23,39 @@
 import pytest
 
 from molecule import config
 from molecule.driver import delegated
 from molecule.test.conftest import is_subset
 
 
-@pytest.fixture
+@pytest.fixture()
 def _driver_managed_section_data():
     return {
         "driver": {
             "name": "delegated",
             "options": {
                 "managed": True,
             },
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _driver_unmanaged_section_data():
     return {
         "driver": {
             "name": "delegated",
             "options": {
                 "managed": False,
             },
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     return delegated.Delegated(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -64,39 +64,45 @@
     assert {
         "connection": "ansible",
         "ansible-inventory": _instance._config.provisioner.inventory_directory,
     } == _instance.testinfra_options
 
 
 def test_name_property(_instance):
-    assert "delegated" == _instance.name
+    assert _instance.name == "delegated"
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_unmanaged_section_data"], indirect=True
+    "config_instance",
+    ["_driver_unmanaged_section_data"],
+    indirect=True,
 )
 def test_options_property(_instance):
     x = {
         "managed": False,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_managed_section_data"], indirect=True
+    "config_instance",
+    ["_driver_managed_section_data"],
+    indirect=True,
 )
 def test_options_property_when_managed(_instance):
     x = {"managed": True}
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_managed_section_data"], indirect=True
+    "config_instance",
+    ["_driver_managed_section_data"],
+    indirect=True,
 )
 def test_login_cmd_template_property_when_managed(_instance):
     x = (
         "ssh {address} -l {user} -p {port} -i {identity_file} "
         "-o UserKnownHostsFile=/dev/null "
         "-o ControlMaster=auto "
         "-o ControlPersist=60s "
@@ -122,22 +128,26 @@
 
 
 def test_managed_property(_instance):
     assert _instance.managed
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_unmanaged_section_data"], indirect=True
+    "config_instance",
+    ["_driver_unmanaged_section_data"],
+    indirect=True,
 )
 def test_default_ssh_connection_options_property(_instance):
     assert [] == _instance.default_ssh_connection_options
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_managed_section_data"], indirect=True
+    "config_instance",
+    ["_driver_managed_section_data"],
+    indirect=True,
 )
 def test_default_ssh_connection_options_property_when_managed(_instance):
     x = [
         "-o UserKnownHostsFile=/dev/null",
         "-o ControlMaster=auto",
         "-o ControlPersist=60s",
         "-o ForwardX11=no",
@@ -146,22 +156,26 @@
         "-o StrictHostKeyChecking=no",
     ]
 
     assert x == _instance.default_ssh_connection_options
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_unmanaged_section_data"], indirect=True
+    "config_instance",
+    ["_driver_unmanaged_section_data"],
+    indirect=True,
 )
 def test_login_options(_instance):
     assert {"instance": "foo"} == _instance.login_options("foo")
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_managed_section_data"], indirect=True
+    "config_instance",
+    ["_driver_managed_section_data"],
+    indirect=True,
 )
 def test_login_options_when_managed(mocker, _instance):
     m = mocker.patch("molecule.driver.delegated.Delegated._get_instance_config")
     m.return_value = {
         "instance": "foo",
         "address": "172.16.0.2",
         "user": "cloud-user",
@@ -180,31 +194,35 @@
         "become_pass": "password",
         "identity_file": "/foo/bar",
     }
     assert x == _instance.login_options("foo")
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_unmanaged_section_data"], indirect=True
+    "config_instance",
+    ["_driver_unmanaged_section_data"],
+    indirect=True,
 )
 def test_ansible_connection_options(_instance):
     x = {}
 
     assert is_subset(x, _instance.ansible_connection_options("foo"))
 
 
 @pytest.mark.xfail(reason="Needs rewrite since switch to delegated")
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_managed_section_data"], indirect=True
+    "config_instance",
+    ["_driver_managed_section_data"],
+    indirect=True,
 )
 def test_ansible_connection_options_when_managed(mocker, _instance):
     assert _instance.managed is True
 
     ssh_case_data = mocker.patch(
-        "molecule.driver.delegated.Delegated._get_instance_config"
+        "molecule.driver.delegated.Delegated._get_instance_config",
     )
     ssh_case_data.return_value = {
         "instance": "foo",
         "address": "172.16.0.2",
         "user": "cloud-user",
         "port": 22,
         "become_method": "su",
@@ -230,15 +248,15 @@
             "-o StrictHostKeyChecking=no"
         ),
     }
 
     assert ssh_expected_data == _instance.ansible_connection_options("foo")
 
     winrm_case_data = mocker.patch(
-        "molecule.driver.delegated.Delegated._get_instance_config"
+        "molecule.driver.delegated.Delegated._get_instance_config",
     )
     winrm_case_data.return_value = {
         "instance": "foo",
         "address": "172.16.0.2",
         "user": "cloud-user",
         "port": 5896,
         "connection": "winrm",
@@ -251,50 +269,55 @@
         "ansible_connection": "winrm",
     }
 
     assert winrm_expected_data == _instance.ansible_connection_options("foo")
 
 
 def test_ansible_connection_options_handles_missing_instance_config_managed(
-    mocker, _instance
+    mocker,
+    _instance,
 ):
     m = mocker.patch("molecule.util.safe_load_file")
     m.side_effect = IOError
 
     assert {} == _instance.ansible_connection_options("foo")
 
 
 def test_ansible_connection_options_handles_missing_results_key_when_managed(
-    mocker, _instance
+    mocker,
+    _instance,
 ):
     m = mocker.patch("molecule.util.safe_load_file")
     m.side_effect = StopIteration
 
     assert {} == _instance.ansible_connection_options("foo")
 
 
 def test_instance_config_property(_instance):
     x = os.path.join(
-        _instance._config.scenario.ephemeral_directory, "instance_config.yml"
+        _instance._config.scenario.ephemeral_directory,
+        "instance_config.yml",
     )
 
     assert x == _instance.instance_config
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_unmanaged_section_data"], indirect=True
+    "config_instance",
+    ["_driver_unmanaged_section_data"],
+    indirect=True,
 )
 def test_ssh_connection_options_property(_instance):
     assert [] == _instance.ssh_connection_options
 
 
 def test_status(mocker, _instance):
     result = _instance.status()
 
-    assert 2 == len(result)
+    assert len(result) == 2
 
     assert result[0].instance_name == "instance-1"
     assert result[0].driver_name == "delegated"
     assert result[0].provisioner_name == "ansible"
     assert result[0].scenario_name == "default"
     assert result[0].created == "false"
     assert result[0].converged == "false"
@@ -304,33 +327,36 @@
     assert result[1].provisioner_name == "ansible"
     assert result[1].scenario_name == "default"
     assert result[1].created == "false"
     assert result[1].converged == "false"
 
 
 def test_created(_instance):
-    assert "false" == _instance._created()
+    assert _instance._created() == "false"
 
 
-@pytest.fixture
+@pytest.fixture()
 def _driver_options_managed_section_data():
     return {"driver": {"options": {"managed": False}}}
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_driver_options_managed_section_data"], indirect=True
+    "config_instance",
+    ["_driver_options_managed_section_data"],
+    indirect=True,
 )
 def test_created_unknown_when_managed_false(
-    _driver_options_managed_section_data, _instance
+    _driver_options_managed_section_data,
+    _instance,
 ):
-    assert "unknown" == _instance._created()
+    assert _instance._created() == "unknown"
 
 
 def test_property(_instance):
-    assert "false" == _instance._converged()
+    assert _instance._converged() == "false"
 
 
 def test_get_instance_config(mocker, _instance):
     m = mocker.patch("molecule.util.safe_load_file")
     m.return_value = [{"instance": "foo"}, {"instance": "bar"}]
 
     x = {"instance": "foo"}
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/conftest.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,43 +22,40 @@
 import os
 
 import pytest
 
 from molecule import util
 
 
-@pytest.fixture
+@pytest.fixture()
 def _molecule_file():
     return os.path.join(
         os.path.dirname(__file__),
         os.path.pardir,
         os.path.pardir,
         os.path.pardir,
         "resources",
         "molecule.yml",
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def _config(_molecule_file, request):
     with open(_molecule_file) as f:
         d = util.safe_load(f)
     if hasattr(request, "param"):
         if isinstance(request.getfixturevalue(request.param), str):
             d2 = util.safe_load(request.getfixturevalue(request.param))
         else:
             d2 = request.getfixturevalue(request.param)
-        # print(100, d)
-        # print(200, d2)
         d = util.merge_dicts(d, d2)
-        # print(300, d)
 
     return d
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_platforms_delegated_section_data():
     return """
 ---
 platforms:
   - name: instance
 """.strip()
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_dependency_section.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_dependency_section.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,51 +19,53 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.model import schema_v3
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_dependency_section_data():
     return {
         "dependency": {
             "name": "galaxy",
             "enabled": True,
             "options": {"foo": "bar"},
             "env": {"FOO": "foo", "FOO_BAR": "foo_bar"},
-        }
+        },
     }
 
 
 @pytest.mark.parametrize("_config", ["_model_dependency_section_data"], indirect=True)
 def test_dependency(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_dependency_errors_section_data():
     return {"dependency": {"name": 0}}
 
 
 @pytest.mark.parametrize(
-    "_config", ["_model_dependency_errors_section_data"], indirect=True
+    "_config",
+    ["_model_dependency_errors_section_data"],
+    indirect=True,
 )
 def test_dependency_has_errors(_config):
     x = ["0 is not one of ['galaxy', 'shell']"]
 
     assert x == schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_dependency_allows_galaxy_section_data():
     return {"dependency": {"name": "galaxy"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_dependency_allows_shell_section_data():
     return {"dependency": {"name": "shell"}}
 
 
 @pytest.mark.parametrize(
     "_config",
     [
@@ -72,19 +74,21 @@
     ],
     indirect=True,
 )
 def test_dependency_allows_shell_name(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_dependency_shell_errors_section_data():
     return {"dependency": {"name": "shell", "command": None}}
 
 
 @pytest.mark.parametrize(
-    "_config", ["_model_dependency_shell_errors_section_data"], indirect=True
+    "_config",
+    ["_model_dependency_shell_errors_section_data"],
+    indirect=True,
 )
 def test_dependency_shell_has_errors(_config):
     x = ["None is not of type 'string'"]
 
     assert x == schema_v3.validate(_config)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_driver_section.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_driver_section.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,47 +19,47 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.model import schema_v3
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_section_data():
     return {
         "driver": {
             "name": "delegated",
             "provider": {"name": None},
             "options": {"managed": True},
             "ssh_connection_options": ["foo", "bar"],
             "safe_files": ["foo", "bar"],
-        }
+        },
     }
 
 
 @pytest.mark.parametrize("_config", ["_model_driver_section_data"], indirect=True)
 def test_driver(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_errors_section_data():
     return {
         "driver": {
             "name": 0,
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_errors_section_data_no_prefix():
     return {
         "driver": {
             "name": "random_name",
-        }
+        },
     }
 
 
 @pytest.mark.parametrize(
     "_config",
     [
         "_model_driver_errors_section_data",
@@ -75,47 +75,49 @@
         # add single quotes for string
         driver_name = f"'{driver_name}'"
 
     error_msg = [" ".join((driver_name, base_error_msg))]
     assert error_msg == schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_provider_name_nullable_section_data():
     return {"driver": {"provider": {"name": None}}}
 
 
 @pytest.mark.parametrize(
-    "_config", ["_model_driver_provider_name_nullable_section_data"], indirect=True
+    "_config",
+    ["_model_driver_provider_name_nullable_section_data"],
+    indirect=True,
 )
 def test_driver_provider_name_nullable(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_allows_delegated_section_data():
     return {"driver": {"name": "delegated"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_allows_molecule_section_data1():
     return {"driver": {"name": "molecule-test_driver.name"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_allows_molecule_section_data2():
     return {"driver": {"name": "molecule_test_driver.name"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_allows_custom_section_data1():
     return {"driver": {"name": "custom-test_driver.name"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_driver_allows_custom_section_data2():
     return {"driver": {"name": "custom_test_driver.name"}}
 
 
 ###
 @pytest.mark.parametrize(
     "_config",
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_platforms_section.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,47 +14,33 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-import pytest
-
 from molecule.model import schema_v3
+from molecule.util import run_command
 
 
-@pytest.mark.parametrize(
-    "_config", ["_model_platforms_delegated_section_data"], indirect=True
-)
-def test_platforms_delegated(_config):
+def test_base_config(_config):
     assert not schema_v3.validate(_config)
 
 
-# todo: https://github.com/json-schema-org/json-schema-vocabularies/issues/22
-# @pytest.mark.parametrize(
-#     "_config", ["_model_platforms_delegated_section_data"], indirect=True
-# )
-# def test_platforms_unique_names(_config):
-#     instance_name = _config["platforms"][0]["name"]
-#     _config["platforms"] += [{"name": instance_name}]  # duplicate platform name
-
-#     expected_validation_errors = {
-#         "platforms": [
-#             {
-#                 0: [{"name": [f"'{instance_name}' is not unique"]}],
-#                 1: [{"name": [f"'{instance_name}' is not unique"]}],
-#             }
-#         ]
-#     }
-
-#     assert expected_validation_errors == schema_v3.validate(_config)
-
-
-# def test_platforms_driver_name_required(_config):
-#     if "platforms" in _config:
-#         del _config["platforms"][0]["name"]
-#     else:
-#         _config["platforms"] = [{"foo": "bar"}]
-#     x = {"platforms": [{0: [{"name": ["required field"]}]}]}
-
-#     assert x == schema_v3.validate(_config)
+def test_molecule_schema():
+    cmd = [
+        "check-jsonschema",
+        "-v",
+        "--schemafile",
+        "src/molecule/data/molecule.json",
+        "src/molecule/test/resources/schema_instance_files/valid/molecule.yml",
+    ]
+    assert run_command(cmd).returncode == 0
+
+    cmd = [
+        "check-jsonschema",
+        "-v",
+        "--schemafile",
+        "src/molecule/data/driver.json",
+        "src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml",
+    ]
+    assert run_command(cmd).returncode != 0
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_provisioner_section.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_provisioner_section.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.model import schema_v3
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_provisioner_section_data():
     return {
         "provisioner": {
             "name": "ansible",
             "log": True,
             "config_options": {"foo": "bar"},
             "connection_options": {"foo": "bar"},
@@ -44,44 +44,48 @@
                 "create": "foo.yml",
                 "converge": "bar.yml",
                 "destroy": "baz.yml",
                 "prepare": "qux.yml",
                 "side_effect": "quux.yml",
                 "foo": {"foo": "bar"},
             },
-        }
+        },
     }
 
 
 @pytest.mark.parametrize("_config", ["_model_provisioner_section_data"], indirect=True)
 def test_provisioner(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_provisioner_errors_section_data():
     return {
         "provisioner": {
             "name": 0,
-        }
+        },
     }
 
 
 @pytest.mark.parametrize(
-    "_config", ["_model_provisioner_errors_section_data"], indirect=True
+    "_config",
+    ["_model_provisioner_errors_section_data"],
+    indirect=True,
 )
 def test_provisioner_has_errors(_config):
     x = ["0 is not one of ['ansible']"]
 
     assert x == schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_provisioner_allows_ansible_section_data():
     return {"provisioner": {"name": "ansible"}}
 
 
 @pytest.mark.parametrize(
-    "_config", [("_model_provisioner_allows_ansible_section_data")], indirect=True
+    "_config",
+    [("_model_provisioner_allows_ansible_section_data")],
+    indirect=True,
 )
 def test_provisioner_allows_name(_config):
     assert not schema_v3.validate(_config)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_scenario_section.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_scenario_section.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,38 +19,40 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.model import schema_v3
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_scenario_section_data():
     return {
         "scenario": {
             "name": "foo",
             "check_sequence": ["check"],
             "converge_sequence": ["converge"],
             "create_sequence": ["create"],
             "destroy_sequence": ["destroy"],
             "test_sequence": ["test"],
-        }
+        },
     }
 
 
 @pytest.mark.parametrize("_config", ["_model_scenario_section_data"], indirect=True)
 def test_scenario(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_scenario_errors_section_data():
     return {"scenario": {"name": 0}}
 
 
 @pytest.mark.parametrize(
-    "_config", ["_model_scenario_errors_section_data"], indirect=True
+    "_config",
+    ["_model_scenario_errors_section_data"],
+    indirect=True,
 )
 def test_scenario_has_errors(_config):
     x = ["0 is not of type 'string'"]
 
     assert x == schema_v3.validate(_config)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_schema.py` & `molecule-5.0.0a1/src/molecule/test/unit/command/test_check.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,12 +14,34 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from molecule.model import schema_v3
+import pytest
 
+from molecule.command import check
 
-def test_base_config(_config):
-    assert not schema_v3.validate(_config)
+
+@pytest.fixture()
+def _patched_ansible_check(mocker):
+    return mocker.patch("molecule.provisioner.ansible.Ansible.check")
+
+
+# NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
+# config.Config._validate from executing.  Thus preventing odd side-effects
+# throughout patched.assert_called unit tests.
+def test_execute(
+    mocker,
+    patched_logger_info,
+    _patched_ansible_check,
+    patched_config_validate,
+    config_instance,
+):
+    c = check.Check(config_instance)
+    c.execute()
+
+    assert len(patched_logger_info.mock_calls) == 1
+    name, args, kwargs = patched_logger_info.mock_calls[0]
+    assert "default" in args
+    assert "check" in args
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/model/v2/test_verifier_section.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_verifier_section.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,57 +19,59 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.model import schema_v3
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_verifier_section_data():
     return {
         "verifier": {
             "name": "testinfra",
             "enabled": True,
             "directory": "foo",
             "options": {"foo": "bar"},
             "env": {"FOO": "foo", "FOO_BAR": "foo_bar"},
             "additional_files_or_dirs": ["foo"],
-        }
+        },
     }
 
 
 @pytest.mark.parametrize("_config", ["_model_verifier_section_data"], indirect=True)
 def test_verifier(_config):
     assert not schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_verifier_errors_section_data():
     return {
         "verifier": {
             "name": 0,
-        }
+        },
     }
 
 
 @pytest.mark.parametrize(
-    "_config", ["_model_verifier_errors_section_data"], indirect=True
+    "_config",
+    ["_model_verifier_errors_section_data"],
+    indirect=True,
 )
 def test_verifier_has_errors(_config):
     x = ["0 is not one of ['ansible', 'goss', 'inspec', 'testinfra']"]
 
     assert x == schema_v3.validate(_config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_verifier_allows_testinfra_section_data():
     return {"verifier": {"name": "testinfra"}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _model_verifier_allows_ansible_section_data():
     return {"verifier": {"name": "ansible"}}
 
 
 @pytest.mark.parametrize(
     "_config",
     [
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/provisioner/test_ansible.py` & `molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,38 +25,38 @@
 import pytest
 
 from molecule import config, util
 from molecule.provisioner import ansible, ansible_playbooks
 from molecule.test.unit.conftest import os_split
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_playbook(mocker):
     m = mocker.patch("molecule.provisioner.ansible_playbook.AnsiblePlaybook")
     m.return_value.execute.return_value = b"patched-ansible-playbook-stdout"
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_write_inventory(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible._write_inventory")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_remove_vars(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible._remove_vars")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_link_or_update_vars(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible._link_or_update_vars")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _provisioner_section_data():
     return {
         "provisioner": {
             "name": "ansible",
             "config_options": {"defaults": {"foo": "bar"}},
             "connection_options": {"foo": "bar"},
             "options": {"foo": "bar", "become": True, "v": True},
@@ -67,30 +67,30 @@
                 "ANSIBLE_FILTER_PLUGINS": "foo/bar",
             },
             "inventory": {
                 "hosts": {
                     "all": {
                         "hosts": {"extra-host-01": {}},
                         "children": {"extra-group": {"hosts": ["extra-host-01"]}},
-                    }
+                    },
                 },
                 "host_vars": {
                     "instance-1": [{"foo": "bar"}],
                     "localhost": [{"foo": "baz"}],
                 },
                 "group_vars": {
                     "example_group1": [{"foo": "bar"}],
                     "example_group2": [{"foo": "bar"}],
                 },
             },
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_provisioner_section_data, config_instance):
     return ansible.Ansible(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -131,19 +131,21 @@
     assert "ANSIBLE_CONFIG" in _instance.env
     assert "ANSIBLE_ROLES_PATH" in _instance.env
     assert "ANSIBLE_LIBRARY" in _instance.env
     assert "ANSIBLE_FILTER_PLUGINS" in _instance.env
 
 
 def test_name_property(_instance):
-    assert "ansible" == _instance.name
+    assert _instance.name == "ansible"
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_config_options_property(_instance):
     x = {
         "defaults": {
             "ansible_managed": "Ansible managed: Do NOT edit this file manually!",
             "display_failed_stderr": True,
             "foo": "bar",
@@ -159,15 +161,17 @@
         },
     }
 
     assert x == _instance.config_options
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_options_property(_instance):
     x = {"become": True, "foo": "bar", "v": True, "skip-tags": "molecule-notest,notest"}
 
     assert x == _instance.options
 
 
@@ -187,36 +191,40 @@
         "skip-tags": "molecule-notest,notest",
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_env_property(_instance):
     x = _instance._config.provisioner.config_file
 
     assert x == _instance.env["ANSIBLE_CONFIG"]
-    assert "bar" == _instance.env["FOO"]
+    assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_env_appends_env_property(_instance):
     os.environ["ANSIBLE_ROLES_PATH"] = ""
 
     expected = [
         util.abs_path(os.path.join(_instance._config.runtime.cache_dir, "roles")),
         util.abs_path(
-            os.path.join(_instance._config.scenario.ephemeral_directory, "roles")
+            os.path.join(_instance._config.scenario.ephemeral_directory, "roles"),
         ),
         util.abs_path(
-            os.path.join(_instance._config.project_directory, os.path.pardir)
+            os.path.join(_instance._config.project_directory, os.path.pardir),
         ),
         util.abs_path(os.path.join(os.path.expanduser("~"), ".ansible", "roles")),
         "/usr/share/ansible/roles",
         "/etc/ansible/roles",
         util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
     ]
 
@@ -225,50 +233,54 @@
 
     roles_path_list = _instance.env["ANSIBLE_ROLES_PATH"].split(":")
 
     assert roles_path_list == expected
 
     x = _instance._get_modules_directories()
     x.append(
-        util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar"))
+        util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
     )
     assert x == _instance.env["ANSIBLE_LIBRARY"].split(":")
 
     x = [
         _instance._get_filter_plugin_directory(),
         util.abs_path(
             os.path.join(
-                _instance._config.scenario.ephemeral_directory, "plugins", "filter"
-            )
+                _instance._config.scenario.ephemeral_directory,
+                "plugins",
+                "filter",
+            ),
         ),
         util.abs_path(
-            os.path.join(_instance._config.project_directory, "plugins", "filter")
+            os.path.join(_instance._config.project_directory, "plugins", "filter"),
         ),
         util.abs_path(
-            os.path.join(os.path.expanduser("~"), ".ansible", "plugins", "filter")
+            os.path.join(os.path.expanduser("~"), ".ansible", "plugins", "filter"),
         ),
         "/usr/share/ansible/plugins/filter",
         util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
     ]
     assert x == _instance.env["ANSIBLE_FILTER_PLUGINS"].split(":")
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_env_appends_env_property_with_os_env(_instance):
     os.environ["ANSIBLE_ROLES_PATH"] = "/foo/bar:/foo/baz"
 
     expected = [
         util.abs_path(os.path.join(_instance._config.runtime.cache_dir, "roles")),
         util.abs_path(
-            os.path.join(_instance._config.scenario.ephemeral_directory, "roles")
+            os.path.join(_instance._config.scenario.ephemeral_directory, "roles"),
         ),
         util.abs_path(
-            os.path.join(_instance._config.project_directory, os.path.pardir)
+            os.path.join(_instance._config.project_directory, os.path.pardir),
         ),
         util.abs_path(os.path.join(os.path.expanduser("~"), ".ansible", "roles")),
         "/usr/share/ansible/roles",
         "/etc/ansible/roles",
         "/foo/bar",
         "/foo/baz",
         util.abs_path(os.path.join(_instance._config.scenario.directory, "foo", "bar")),
@@ -279,40 +291,46 @@
 
     roles_path_list = _instance.env["ANSIBLE_ROLES_PATH"].split(":")
 
     assert roles_path_list == expected
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_host_vars_property(_instance):
     x = {"instance-1": [{"foo": "bar"}], "localhost": [{"foo": "baz"}]}
 
     assert x == _instance.host_vars
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_group_vars_property(_instance):
     x = {"example_group1": [{"foo": "bar"}], "example_group2": [{"foo": "bar"}]}
 
     assert x == _instance.group_vars
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_hosts_property(_instance):
     hosts = {
         "all": {
             "hosts": {"extra-host-01": {}},
             "children": {"extra-group": {"hosts": ["extra-host-01"]}},
-        }
+        },
     }
 
     assert hosts == _instance.hosts
 
 
 def test_links_property(_instance):
     assert {} == _instance.links
@@ -321,15 +339,16 @@
 def test_inventory_directory_property(_instance):
     x = os.path.join(_instance._config.scenario.ephemeral_directory, "inventory")
     assert x == _instance.inventory_directory
 
 
 def test_inventory_file_property(_instance):
     x = os.path.join(
-        _instance._config.scenario.inventory_directory, "ansible_inventory.yml"
+        _instance._config.scenario.inventory_directory,
+        "ansible_inventory.yml",
     )
 
     assert x == _instance.inventory_file
 
 
 def test_config_file_property(_instance):
     x = os.path.join(_instance._config.scenario.ephemeral_directory, "ansible.cfg")
@@ -341,15 +360,15 @@
     assert isinstance(_instance.playbooks, ansible_playbooks.AnsiblePlaybooks)
 
 
 def test_directory_property(_instance):
     result = _instance.directory
     parts = os_split(result)
 
-    assert ("molecule", "provisioner", "ansible") == parts[-3:]
+    assert parts[-3:] == ("molecule", "provisioner", "ansible")
 
 
 def test_playbooks_cleaned_property_is_optional(_instance):
     assert _instance.playbooks.cleanup is None
 
 
 def test_playbooks_converge_property(_instance):
@@ -362,111 +381,132 @@
     assert _instance.playbooks.side_effect is None
 
 
 def test_check(_instance, mocker, _patched_ansible_playbook):
     _instance.check()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.converge, _instance._config, False
+        _instance._config.provisioner.playbooks.converge,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.add_cli_arg.assert_called_once_with(
-        "check", True
+        "check",
+        True,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_converge(_instance, mocker, _patched_ansible_playbook):
     result = _instance.converge()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.converge, _instance._config, False
+        _instance._config.provisioner.playbooks.converge,
+        _instance._config,
+        False,
     )
     # NOTE(retr0h): This is not the true return type.  This is a mock return
     #               which didn't go through str.decode().
     assert result == b"patched-ansible-playbook-stdout"
 
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_converge_with_playbook(_instance, mocker, _patched_ansible_playbook):
     result = _instance.converge("playbook")
 
     _patched_ansible_playbook.assert_called_once_with(
-        "playbook", _instance._config, False
+        "playbook",
+        _instance._config,
+        False,
     )
     # NOTE(retr0h): This is not the true return type.  This is a mock return
     #               which didn't go through str.decode().
     assert result == b"patched-ansible-playbook-stdout"
 
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_cleanup(_instance, mocker, _patched_ansible_playbook):
     _instance.cleanup()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.cleanup, _instance._config, False
+        _instance._config.provisioner.playbooks.cleanup,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_destroy(_instance, mocker, _patched_ansible_playbook):
     _instance.destroy()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.destroy, _instance._config, False
+        _instance._config.provisioner.playbooks.destroy,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_side_effect(_instance, mocker, _patched_ansible_playbook):
     _instance.side_effect()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.side_effect, _instance._config, False
+        _instance._config.provisioner.playbooks.side_effect,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_create(_instance, mocker, _patched_ansible_playbook):
     _instance.create()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.create, _instance._config, False
+        _instance._config.provisioner.playbooks.create,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_prepare(_instance, mocker, _patched_ansible_playbook):
     _instance.prepare()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.prepare, _instance._config, False
+        _instance._config.provisioner.playbooks.prepare,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_syntax(_instance, mocker, _patched_ansible_playbook):
     _instance.syntax()
 
     _patched_ansible_playbook.assert_called_once_with(
-        _instance._config.provisioner.playbooks.converge, _instance._config, False
+        _instance._config.provisioner.playbooks.converge,
+        _instance._config,
+        False,
     )
     _patched_ansible_playbook.return_value.add_cli_arg.assert_called_once_with(
-        "syntax-check", True
+        "syntax-check",
+        True,
     )
     _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_verify(_instance, mocker, _patched_ansible_playbook):
     _instance.verify()
 
     if _instance._config.provisioner.playbooks.verify:
         _patched_ansible_playbook.assert_called_once_with(
-            _instance._config.provisioner.playbooks.verify, _instance._config
+            _instance._config.provisioner.playbooks.verify,
+            _instance._config,
         )
         _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
 def test_write_config(temp_dir, _instance):
     _instance.write_config()
 
@@ -502,15 +542,17 @@
     _patched_write_inventory.assert_called_once_with()
     _patched_remove_vars.assert_called_once_with()
     assert not patched_add_or_update_vars.called
     _patched_link_or_update_vars.assert_called_once_with()
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_add_or_update_vars(_instance):
     inventory_dir = _instance._config.scenario.inventory_directory
 
     host_vars_directory = os.path.join(inventory_dir, "host_vars")
     host_vars = os.path.join(host_vars_directory, "instance-1")
 
@@ -532,15 +574,17 @@
 
     hosts = os.path.join(inventory_dir, "hosts")
     assert os.path.isfile(hosts)
     assert util.safe_load_file(hosts) == _instance.hosts
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_add_or_update_vars_without_host_vars(_instance):
     c = _instance._config.config
     c["provisioner"]["inventory"]["host_vars"] = {}
     inventory_dir = _instance._config.scenario.inventory_directory
 
     host_vars_directory = os.path.join(inventory_dir, "host_vars")
@@ -582,15 +626,17 @@
 
     assert not os.path.isdir(host_vars_directory)
     assert not os.path.isdir(group_vars_directory)
     assert not os.path.isfile(hosts)
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_remove_vars(_instance):
     inventory_dir = _instance._config.scenario.inventory_directory
 
     hosts = os.path.join(inventory_dir, "hosts")
     host_vars_directory = os.path.join(inventory_dir, "host_vars")
     host_vars = os.path.join(host_vars_directory, "instance-1")
@@ -661,58 +707,60 @@
 def test_link_vars_raises_when_source_not_found(_instance, patched_logger_critical):
     c = _instance._config.config
     c["provisioner"]["inventory"]["links"] = {"foo": "../bar"}
 
     with pytest.raises(SystemExit) as e:
         _instance._link_or_update_vars()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     source = os.path.join(_instance._config.scenario.directory, os.path.pardir, "bar")
     msg = f"The source path '{source}' does not exist."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_verify_inventory(_instance):
     _instance._verify_inventory()
 
 
 def test_verify_inventory_raises_when_missing_hosts(
-    temp_dir, patched_logger_critical, _instance
+    temp_dir,
+    patched_logger_critical,
+    _instance,
 ):
     _instance._config.config["platforms"] = []
     with pytest.raises(SystemExit) as e:
         _instance._verify_inventory()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "Instances missing from the 'platform' section of molecule.yml."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_vivify(_instance):
     d = _instance._vivify()
     d["bar"]["baz"] = "qux"
 
-    assert "qux" == str(d["bar"]["baz"])
+    assert str(d["bar"]["baz"]) == "qux"
 
 
 def test_default_to_regular(_instance):
     d = collections.defaultdict()
     assert isinstance(d, collections.defaultdict)
 
     d = _instance._default_to_regular(d)
     assert isinstance(d, dict)
 
 
 def test_get_plugin_directory(_instance):
     result = _instance._get_plugin_directory()
     parts = os_split(result)
 
-    assert ("molecule", "provisioner", "ansible", "plugins") == parts[-4:]
+    assert parts[-4:] == ("molecule", "provisioner", "ansible", "plugins")
 
 
 def test_get_modules_directories_default(_instance, monkeypatch):
     monkeypatch.delenv("ANSIBLE_LIBRARY", raising=False)
 
     paths = _instance._get_modules_directories()
 
@@ -753,15 +801,15 @@
 
 def test_absolute_path_for(_instance):
     env = {"foo": "foo:bar"}
     x = ":".join(
         [
             os.path.join(_instance._config.scenario.directory, "foo"),
             os.path.join(_instance._config.scenario.directory, "bar"),
-        ]
+        ],
     )
 
     assert x == _instance._absolute_path_for(env, "foo")
 
 
 def test_absolute_path_for_raises_with_missing_key(_instance):
     env = {"foo": "foo:bar"}
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/provisioner/test_ansible_playbook.py` & `molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbook.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,75 +22,79 @@
 
 import pytest
 
 from molecule import config
 from molecule.provisioner import ansible_playbook
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     _instance = ansible_playbook.AnsiblePlaybook("playbook", config_instance)
 
     return _instance
 
 
-@pytest.fixture
+@pytest.fixture()
 def _provisioner_section_data():
     return {"provisioner": {"name": "ansible", "env": {"FOO": "bar"}}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _verifier_section_data():
     return {"verifier": {"name": "ansible", "env": {"FOO": "bar"}}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _provisioner_verifier_section_data():
     return {
         "provisioner": {"name": "ansible", "env": {"FOO": "bar"}},
         "verifier": {"name": "ansible", "env": {"FOO": "baz"}},
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance_for_verifier_env(config_instance):
     _instance = ansible_playbook.AnsiblePlaybook("playbook", config_instance, True)
     return _instance
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_section_data"],
+    indirect=True,
 )
 def test_env_in_provision(_instance_for_verifier_env):
-    assert "bar" == _instance_for_verifier_env._env["FOO"]
+    assert _instance_for_verifier_env._env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
 def test_env_in_verifier(_instance_for_verifier_env):
-    assert "bar" == _instance_for_verifier_env._env["FOO"]
+    assert _instance_for_verifier_env._env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_provisioner_verifier_section_data"], indirect=True
+    "config_instance",
+    ["_provisioner_verifier_section_data"],
+    indirect=True,
 )
 def test_env_in_verify_override_provision(_instance_for_verifier_env):
-    assert "baz" == _instance_for_verifier_env._env["FOO"]
+    assert _instance_for_verifier_env._env["FOO"] == "baz"
 
 
-@pytest.fixture
+@pytest.fixture()
 def _inventory_directory(_instance):
     return _instance._config.provisioner.inventory_directory
 
 
 def test_ansible_command_private_member(_instance):
     assert _instance._ansible_command is None
 
 
 def test_ansible_playbook_private_member(_instance):
-    assert "playbook" == _instance._playbook
+    assert _instance._playbook == "playbook"
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
 def test_bake(_inventory_directory, _instance):
@@ -108,15 +112,16 @@
         pb,
     ]
 
     assert _instance._ansible_command.cmd == args
 
 
 def test_bake_removes_non_interactive_options_from_non_converge_playbooks(
-    _inventory_directory, _instance
+    _inventory_directory,
+    _instance,
 ):
     _instance.bake()
 
     args = [
         "ansible-playbook",
         "--inventory",
         _inventory_directory,
@@ -184,15 +189,15 @@
 
 
 def test_execute(patched_run_command, _instance):
     _instance._ansible_command = "patched-command"
     result = _instance.execute()
 
     patched_run_command.assert_called_once_with("patched-command", debug=False)
-    assert "patched-run-command-stdout" == result
+    assert result == "patched-run-command-stdout"
 
 
 def test_execute_bakes(_inventory_directory, patched_run_command, _instance):
     _instance.execute()
 
     assert _instance._ansible_command is not None
 
@@ -201,21 +206,21 @@
         "--inventory",
         _inventory_directory,
         "--skip-tags",
         "molecule-notest,notest",
         "playbook",
     ]
 
-    # result = str(patched_run_command.mock_calls[0][1][0]).split()
-
     assert _instance._ansible_command.cmd == args
 
 
 def test_execute_bakes_with_ansible_args(
-    _inventory_directory, patched_run_command, _instance
+    _inventory_directory,
+    patched_run_command,
+    _instance,
 ):
     _instance._config.ansible_args = ("-o", "--syntax-check")
     _instance.execute()
 
     assert _instance._ansible_command is not None
 
     args = [
@@ -231,32 +236,37 @@
         "playbook",
     ]
 
     assert _instance._ansible_command.cmd == args
 
 
 def test_executes_catches_and_exits_return_code(
-    patched_run_command, patched_logger_critical, _instance
+    patched_run_command,
+    patched_logger_critical,
+    _instance,
 ):
     patched_run_command.side_effect = [
         CompletedProcess(
-            args="ansible-playbook", returncode=1, stdout="out", stderr="err"
-        )
+            args="ansible-playbook",
+            returncode=1,
+            stdout="out",
+            stderr="err",
+        ),
     ]
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
 
 def test_add_cli_arg(_instance):
     assert {} == _instance._cli
 
     _instance.add_cli_arg("foo", "bar")
     assert {"foo": "bar"} == _instance._cli
 
 
 def test_add_env_arg(_instance):
     assert "foo" not in _instance._env
 
     _instance.add_env_arg("foo", "bar")
-    assert "bar" == _instance._env["foo"]
+    assert _instance._env["foo"] == "bar"
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/provisioner/test_ansible_playbooks.py` & `molecule-5.0.0a1/src/molecule/test/unit/provisioner/test_ansible_playbooks.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 import pytest
 
 from molecule import util
 from molecule.provisioner import ansible_playbooks
 from molecule.test.unit.conftest import os_split
 
 
-@pytest.fixture
+@pytest.fixture()
 def _provisioner_section_data():
     return {"provisioner": {"name": "ansible", "options": {}, "config_options": {}}}
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_provisioner_section_data, config_instance):
     return ansible_playbooks.AnsiblePlaybooks(config_instance)
 
 
 def test_cleanup_property_is_optional(_instance):
     assert _instance._config.provisioner.playbooks.cleanup is None
 
@@ -86,52 +86,54 @@
     util.write_file(x, "")
 
     assert x == _instance._get_playbook("create")
 
 
 @pytest.mark.skip(reason="create not running for delegated")
 def test_get_playbook_returns_bundled_driver_playbook_when_local_not_found(
-    tmpdir, _instance
+    tmpdir,
+    _instance,
 ):
     x = os.path.join(_instance._get_playbook_directory(), "delegated", "create.yml")
 
     assert x == _instance._get_playbook("create")
 
 
-@pytest.fixture
+@pytest.fixture()
 def _provisioner_driver_section_data():
     return {
         "provisioner": {
             "name": "ansible",
             "playbooks": {
                 "create": "create.yml",
             },
-        }
+        },
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _provisioner_driver_playbook_key_missing_section_data():
     return {
         "provisioner": {
             "name": "ansible",
             "playbooks": {
                 "side_effect": "side_effect.yml",
             },
-        }
+        },
     }
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_driver_playbook_key_missing_section_data"],
     indirect=True,
 )
 def test_get_ansible_playbook_with_driver_key_when_playbook_key_missing(
-    tmpdir, _instance
+    tmpdir,
+    _instance,
 ):
     x = os.path.join(_instance._config.scenario.directory, "side_effect.yml")
     util.write_file(x, "")
 
     assert x == _instance._get_playbook("side_effect")
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_api.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_config.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,25 +50,25 @@
     config_instance.args = {"env_file": ".env"}
     result = config_instance.env_file
 
     assert util.abs_path(config_instance.args.get("env_file")) == result
 
 
 def test_subcommand_property(config_instance):
-    assert "test" == config_instance.subcommand
+    assert config_instance.subcommand == "test"
 
 
 def test_action_property(config_instance):
     assert config_instance.action is None
 
 
 def test_action_setter(config_instance):
     config_instance.action = "foo"
 
-    assert "foo" == config_instance.action
+    assert config_instance.action == "foo"
 
 
 def test_init_calls_validate(patched_config_validate, config_instance):
     patched_config_validate.assert_called_once_with()
 
 
 def test_project_directory_property(config_instance):
@@ -81,27 +81,29 @@
     assert x == config_instance.molecule_directory
 
 
 def test_dependency_property(config_instance):
     assert isinstance(config_instance.dependency, ansible_galaxy.AnsibleGalaxy)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _config_dependency_shell_section_data():
     return {"dependency": {"name": "shell", "command": "bin/command"}}
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_config_dependency_shell_section_data"], indirect=True
+    "config_instance",
+    ["_config_dependency_shell_section_data"],
+    indirect=True,
 )
 def test_dependency_property_is_shell(config_instance):
     assert isinstance(config_instance.dependency, shell.Shell)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _config_driver_delegated_section_data():
     return {"driver": {"name": "delegated", "options": {"managed": False}}}
 
 
 def test_env(config_instance):
     config_instance.args = {"env_file": ".env"}
     x = {
@@ -148,36 +150,37 @@
 def test_get_driver_name_from_state_file(config_instance, mocker):
     config_instance.state.change_state("driver", "state-driver")
 
     with pytest.raises(SystemExit):
         config_instance._get_driver_name()
 
     mocker.patch("molecule.api.drivers", return_value=["state-driver"])
-    assert "state-driver" == config_instance._get_driver_name()
+    assert config_instance._get_driver_name() == "state-driver"
 
 
 def test_get_driver_name_from_cli(config_instance):
     config_instance.command_args = {"driver_name": "cli-driver"}
 
-    assert "cli-driver" == config_instance._get_driver_name()
+    assert config_instance._get_driver_name() == "cli-driver"
 
 
 def test_get_driver_name(config_instance):
-    assert "delegated" == config_instance._get_driver_name()
+    assert config_instance._get_driver_name() == "delegated"
 
 
 def test_get_driver_name_raises_when_different_driver_used(
-    patched_logger_critical, config_instance
+    patched_logger_critical,
+    config_instance,
 ):
     config_instance.state.change_state("driver", "foo")
     config_instance.command_args = {"driver_name": "bar"}
     with pytest.raises(SystemExit) as e:
         config_instance._get_driver_name()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = (
         "Instance(s) were created with the 'foo' driver, "
         "but the subcommand is using 'bar' driver."
     )
 
     patched_logger_critical.assert_called_once_with(msg)
@@ -251,34 +254,37 @@
     string = "foo: ${NONE-$HOME}"
     x = f"foo: {os.environ['HOME']}"
 
     assert x == config_instance._interpolate(string, os.environ, None)
 
 
 def test_interpolate_raises_on_failed_interpolation(
-    patched_logger_critical, config_instance
+    patched_logger_critical,
+    config_instance,
 ):
     string = "$6$8I5Cfmpr$kGZB"
 
     with pytest.raises(SystemExit) as e:
         config_instance._interpolate(string, os.environ, None)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = (
         f"parsing config file '{config_instance.molecule_file}'.\n\n"
         "Invalid placeholder in string: line 1, col 1\n"
         "$6$8I5Cfmpr$kGZB"
     )
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_get_defaults(config_instance, mocker):
     mocker.patch.object(
-        config_instance, "molecule_file", "/path/to/test_scenario_name/molecule.yml"
+        config_instance,
+        "molecule_file",
+        "/path/to/test_scenario_name/molecule.yml",
     )
     defaults = config_instance._get_defaults()
     assert defaults["scenario"]["name"] == "test_scenario_name"
 
 
 def test_validate(mocker, config_instance, patched_logger_debug):
     m = mocker.patch("molecule.model.schema_v3.validate")
@@ -288,34 +294,36 @@
 
     assert patched_logger_debug.call_count == 1
 
     m.assert_called_with(config_instance.config)
 
 
 def test_validate_exists_when_validation_fails(
-    mocker, patched_logger_critical, config_instance
+    mocker,
+    patched_logger_critical,
+    config_instance,
 ):
     m = mocker.patch("molecule.model.schema_v3.validate")
     m.return_value = "validation errors"
 
     with pytest.raises(SystemExit) as e:
         config_instance._validate()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = f"Failed to validate {config_instance.molecule_file}\n\nvalidation errors"
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_molecule_directory():
-    assert "/foo/bar/molecule" == config.molecule_directory("/foo/bar")
+    assert config.molecule_directory("/foo/bar") == "/foo/bar/molecule"
 
 
 def test_molecule_file():
-    assert "/foo/bar/molecule.yml" == config.molecule_file("/foo/bar")
+    assert config.molecule_file("/foo/bar") == "/foo/bar/molecule.yml"
 
 
 def test_set_env_from_file(config_instance):
     config_instance.args = {"env_file": ".env"}
     contents = {"foo": "bar", "BAZ": "zzyzx"}
     env_file = config_instance.args.get("env_file")
     util.write_file(env_file, util.safe_dump(contents))
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_interpolation.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_interpolation.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 #    under the License.
 
 import pytest
 
 from molecule import interpolation
 
 
-@pytest.fixture
+@pytest.fixture()
 def _mock_env():
     return {
         "FOO": "foo",
         "BAR": "",
         "DEPENDENCY_NAME": "galaxy",
         "VERIFIER_NAME": "ansible",
         "MOLECULE_SCENARIO_NAME": "default",
     }
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_mock_env):
     return interpolation.Interpolator(interpolation.TemplateWithDefaults, _mock_env)
 
 
 def test_escaped_interpolation(_instance):
-    assert "${foo}" == _instance.interpolate("$${foo}")
+    assert _instance.interpolate("$${foo}") == "${foo}"
 
 
 def test_invalid_interpolation(_instance):
     with pytest.raises(interpolation.InvalidInterpolation):
         _instance.interpolate("${")
     with pytest.raises(interpolation.InvalidInterpolation):
         _instance.interpolate("$}")
@@ -51,43 +51,50 @@
     with pytest.raises(interpolation.InvalidInterpolation):
         _instance.interpolate("${foo }")
     with pytest.raises(interpolation.InvalidInterpolation):
         _instance.interpolate("${foo!}")
 
 
 def test_interpolate_missing_no_default(_instance):
-    assert "This  var" == _instance.interpolate("This ${missing} var")
-    assert "This  var" == _instance.interpolate("This ${BAR} var")
+    assert _instance.interpolate("This ${missing} var") == "This  var"
+    assert _instance.interpolate("This ${BAR} var") == "This  var"
 
 
 def test_interpolate_with_value(_instance):
-    assert "This foo var" == _instance.interpolate("This $FOO var")
-    assert "This foo var" == _instance.interpolate("This ${FOO} var")
+    assert _instance.interpolate("This $FOO var") == "This foo var"
+    assert _instance.interpolate("This ${FOO} var") == "This foo var"
 
 
 def test_interpolate_missing_with_default(_instance):
-    assert "ok def" == _instance.interpolate("ok ${missing:-def}")
-    assert "ok def" == _instance.interpolate("ok ${missing-def}")
-    assert "ok /non:-alphanumeric" == _instance.interpolate(
-        "ok ${BAR:-/non:-alphanumeric}"
+    assert _instance.interpolate("ok ${missing:-def}") == "ok def"
+    assert _instance.interpolate("ok ${missing-def}") == "ok def"
+    assert (
+        _instance.interpolate(
+            "ok ${BAR:-/non:-alphanumeric}",
+        )
+        == "ok /non:-alphanumeric"
     )
 
 
 def test_interpolate_with_empty_and_default_value(_instance):
-    assert "ok def" == _instance.interpolate("ok ${BAR:-def}")
-    assert "ok " == _instance.interpolate("ok ${BAR-def}")
+    assert _instance.interpolate("ok ${BAR:-def}") == "ok def"
+    assert _instance.interpolate("ok ${BAR-def}") == "ok "
 
 
 def test_interpolate_interpolates_MOLECULE_strings(_instance):
-    assert "default" == _instance.interpolate("$MOLECULE_SCENARIO_NAME")
+    assert _instance.interpolate("$MOLECULE_SCENARIO_NAME") == "default"
 
 
 def test_interpolate_does_not_interpolate_MOLECULE_strings(_instance):
-    assert "foo $MOLECULE_SCENARIO_NAME" == _instance.interpolate(
-        "foo $MOLECULE_SCENARIO_NAME", keep_string="MOLECULE_"
+    assert (
+        _instance.interpolate(
+            "foo $MOLECULE_SCENARIO_NAME",
+            keep_string="MOLECULE_",
+        )
+        == "foo $MOLECULE_SCENARIO_NAME"
     )
 
 
 def test_interpolate_with_molecule_yaml(_instance):
     data = """
 ---
 dependency:
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_logger.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from __future__ import print_function
 
 import logging
 
 import pytest
 
 from molecule.command.base import Base
 from molecule.console import should_do_markup
@@ -33,27 +32,27 @@
 class Dummy(Base):
     """ExtendedBase Class."""
 
     def execute(self, action_args=None):
         return True
 
 
-@pytest.fixture
+@pytest.fixture()
 def _dummy_class(patched_config_validate, config_instance):
     return Dummy
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(_dummy_class, config_instance, _patched_logger_env):
     # _patched_logger_env included here to ensure pytest runs it first
     get_section_loggers.cache_clear()
     return _dummy_class(config_instance)
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_logger_env(request, monkeypatch):
     """Parametrize tests with and without CI env vars."""
     envvars = {"CI": None, "GITHUB_ACTIONS": None, "GITLAB_CI": None, "TRAVIS": None}
     envvars.update(request.param[1])
     for envvar, value in envvars.items():
         if value is None:
             monkeypatch.delenv(envvar, raising=False)
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_platforms.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_platforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule import platforms
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     return platforms.Platforms(config_instance)
 
 
 def test_instances_property(_instance):
     x = [
         {"groups": ["foo", "bar"], "name": "instance-1", "children": ["child1"]},
         {"groups": ["baz", "foo"], "name": "instance-2", "children": ["child2"]},
     ]
 
     assert x == _instance.instances
 
 
-@pytest.fixture
+@pytest.fixture()
 def platform_name(request, config_instance):
     return platforms.Platforms(config_instance, platform_name=request.param)
 
 
 @pytest.mark.parametrize("platform_name", ["instance-1"], indirect=True)
 def test_instances_property_with_platform_name_instance_1(platform_name):
     x = [
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_scenario.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from molecule import config, scenario, util
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(patched_config_validate, config_instance):
     return scenario.Scenario(config_instance)
 
 
 def test_prune(_instance):
     e_dir = _instance.ephemeral_directory
     # prune data also includes files in the scenario inventory dir,
@@ -80,15 +80,15 @@
 
 
 def test_init_calls_setup(patched_scenario_setup, _instance):
     patched_scenario_setup.assert_called_once_with()
 
 
 def test_name_property(_instance):
-    assert "default" == _instance.name
+    assert _instance.name == "default"
 
 
 def test_directory_property(molecule_scenario_directory_fixture, _instance):
     assert molecule_scenario_directory_fixture == _instance.directory
 
 
 def test_ephemeral_directory_property(_instance):
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_scenarios.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_scenarios.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #  Copyright (c) 2015-2018 Cisco Systems, Inc.
-# -*- coding: utf-8 -*-
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to
 #  deal in the Software without restriction, including without limitation the
 #  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 #  sell copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -24,59 +23,59 @@
 import pytest
 
 from molecule import config, scenario, scenarios
 from molecule.console import console
 from molecule.text import chomp, strip_ansi_escape
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     config_instance_1 = copy.deepcopy(config_instance)
 
     config_instance_2 = copy.deepcopy(config_instance)
     config_instance_2.config["scenario"]["name"] = "foo"
 
     return scenarios.Scenarios([config_instance_1, config_instance_2])
 
 
 def test_configs_private_member(_instance):
-    assert 2 == len(_instance._configs)
+    assert len(_instance._configs) == 2
     assert isinstance(_instance._configs[0], config.Config)
     assert isinstance(_instance._configs[1], config.Config)
 
 
 def test_scenario_name_private_member(_instance):
     assert _instance._scenario_name is None
 
 
 def test_scenarios_private_member(_instance):
-    assert 2 == len(_instance._scenarios)
+    assert len(_instance._scenarios) == 2
     assert isinstance(_instance._scenarios[0], scenario.Scenario)
     assert isinstance(_instance._scenarios[1], scenario.Scenario)
 
 
 def test_scenarios_iterator(_instance):
-    s = [scenario for scenario in _instance]
+    s = list(_instance)
 
-    assert "default" == s[0].name
-    assert "foo" == s[1].name
+    assert s[0].name == "default"
+    assert s[1].name == "foo"
 
 
 def test_all_property(_instance):
     result = _instance.all
 
-    assert 2 == len(result)
-    assert "default" == result[0].name
-    assert "foo" == result[1].name
+    assert len(result) == 2
+    assert result[0].name == "default"
+    assert result[1].name == "foo"
 
 
 def test_all_filters_on_scenario_name_property(_instance):
     _instance._scenario_name = "default"
 
-    assert 1 == len(_instance.all)
+    assert len(_instance.all) == 1
 
 
 def test_print_matrix(capsys, _instance):
     with console.capture() as capture:
         _instance.print_matrix()
     result = chomp(strip_ansi_escape(capture.get()))
 
@@ -117,25 +116,25 @@
 
 
 def test_verify_raises_when_scenario_not_found(_instance, patched_logger_critical):
     _instance._scenario_name = "invalid"
     with pytest.raises(SystemExit) as e:
         _instance._verify()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     msg = "Scenario 'invalid' not found.  Exiting."
     patched_logger_critical.assert_called_once_with(msg)
 
 
 def test_filter_for_scenario(_instance):
     _instance._scenario_name = "default"
     result = _instance._filter_for_scenario()
-    assert 1 == len(result)
-    assert "default" == result[0].name
+    assert len(result) == 1
+    assert result[0].name == "default"
 
     _instance._scenario_name = "invalid"
     result = _instance._filter_for_scenario()
     assert [] == result
 
 
 def test_get_matrix(_instance):
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_scenarios_ordered.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_scenarios_ordered.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #  Copyright (c) 2018 Marc Dequènes (Duck) <duck@redhat.com>
-# -*- coding: utf-8 -*-
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to
 #  deal in the Software without restriction, including without limitation the
 #  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 #  sell copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -22,39 +21,42 @@
 import copy
 
 import pytest
 
 from molecule import scenarios
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     config_instance_1 = copy.deepcopy(config_instance)
     config_instance_1.config["scenario"]["name"] = "two"
     config_instance_1.molecule_file = config_instance_1.molecule_file.replace(
-        "default", "02_foo"
+        "default",
+        "02_foo",
     )
 
     config_instance_2 = copy.deepcopy(config_instance)
     config_instance_2.config["scenario"]["name"] = "one"
     config_instance_2.molecule_file = config_instance_2.molecule_file.replace(
-        "default", "01_foo"
+        "default",
+        "01_foo",
     )
 
     config_instance_3 = copy.deepcopy(config_instance)
     config_instance_3.config["scenario"]["name"] = "three"
     config_instance_3.molecule_file = config_instance_3.molecule_file.replace(
-        "default", "03_foo"
+        "default",
+        "03_foo",
     )
 
     return scenarios.Scenarios(
-        [config_instance_1, config_instance_2, config_instance_3]
+        [config_instance_1, config_instance_2, config_instance_3],
     )
 
 
 def test_all_ordered(_instance):
     result = _instance.all
 
-    assert 3 == len(result)
-    assert "one" == result[0].name
-    assert "two" == result[1].name
-    assert "three" == result[2].name
+    assert len(result) == 3
+    assert result[0].name == "one"
+    assert result[1].name == "two"
+    assert result[2].name == "three"
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_shell.py` & `molecule-5.0.0a1/src/molecule/test/unit/model/v2/test_platforms_section.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,13 +16,30 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
-from molecule import shell
+from molecule.model import schema_v3
 
 
-def test_shell():
-    with pytest.raises(SystemExit):
-        shell.main()
+@pytest.mark.parametrize(
+    "_config",
+    ["_model_platforms_delegated_section_data"],
+    indirect=True,
+)
+def test_platforms_delegated(_config):
+    assert not schema_v3.validate(_config)
+
+
+# todo: https://github.com/json-schema-org/json-schema-vocabularies/issues/22
+# @pytest.mark.parametrize(
+# def test_platforms_unique_names(_config):
+
+#         "platforms": [
+#                 0: [{"name": [f"'{instance_name}' is not unique"]}],
+#                 1: [{"name": [f"'{instance_name}' is not unique"]}],
+
+
+# def test_platforms_driver_name_required(_config):
+#     if "platforms" in _config:
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_state.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 
 import pytest
 
 from molecule import state, util
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance(config_instance):
     return state.State(config_instance)
 
 
 def test_state_file_property(_instance):
     x = os.path.join(_instance._config.scenario.ephemeral_directory, "state.yml")
 
@@ -86,15 +86,15 @@
 
     assert _instance.created
 
 
 def test_change_state_driver(_instance):
     _instance.change_state("driver", "foo")
 
-    assert "foo" == _instance.driver
+    assert _instance.driver == "foo"
 
 
 def test_change_state_prepared(_instance):
     _instance.change_state("prepared", True)
 
     assert _instance.prepared
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_status.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.status import Status
 
 
-@pytest.fixture
+@pytest.fixture()
 def _instance():
     s = Status(
         instance_name=None,
         driver_name=None,
         provisioner_name=None,
         scenario_name=None,
         created=None,
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/test_util.py` & `molecule-5.0.0a1/src/molecule/test/unit/test_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
-from __future__ import print_function
 
 import binascii
 import io
 import os
 import warnings
 from pathlib import Path
 
@@ -72,61 +71,61 @@
     assert result == expected
 
 
 def test_sysexit():
     with pytest.raises(SystemExit) as e:
         util.sysexit()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
 
 def test_sysexit_with_custom_code():
     with pytest.raises(SystemExit) as e:
         util.sysexit(2)
 
-    assert 2 == e.value.code
+    assert e.value.code == 2
 
 
 def test_sysexit_with_message(patched_logger_critical):
     with pytest.raises(SystemExit) as e:
         util.sysexit_with_message("foo")
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     patched_logger_critical.assert_called_once_with("foo")
 
 
 def test_sysexit_with_warns(patched_logger_critical, patched_logger_warning):
     with pytest.raises(SystemExit) as e:
         with warnings.catch_warnings(record=True) as warns:
             warnings.filterwarnings("default", category=MoleculeRuntimeWarning)
             warnings.warn("xxx", category=IncompatibleMoleculeRuntimeWarning)
 
         util.sysexit_with_message("foo", warns=warns)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
     patched_logger_critical.assert_called_once_with("foo")
     patched_logger_warning.assert_called_once_with("xxx")
 
 
 def test_sysexit_with_message_and_custom_code(patched_logger_critical):
     with pytest.raises(SystemExit) as e:
         util.sysexit_with_message("foo", 2)
 
-    assert 2 == e.value.code
+    assert e.value.code == 2
 
     patched_logger_critical.assert_called_once_with("foo")
 
 
 def test_run_command():
     cmd = ["ls"]
     x = util.run_command(cmd)
 
-    assert 0 == x.returncode
+    assert x.returncode == 0
 
 
 def test_run_command_with_debug(mocker, patched_print_debug):
     env = {"ANSIBLE_FOO": "foo", "MOLECULE_BAR": "bar"}
     util.run_command(["ls"], debug=True, env=env)
     x = [
         mocker.call("ANSIBLE ENVIRONMENT", "ANSIBLE_FOO: foo\n"),
@@ -166,22 +165,22 @@
     mol_dir = molecule_directory()
     for scenario in scenarios:
         scenario_directory = os.path.join(mol_dir, scenario)
         molecule_file = get_molecule_file(scenario_directory)
         os.makedirs(scenario_directory, exist_ok=True)
         util.write_file(molecule_file, "")
 
-    result = [f for f in util.os_walk(mol_dir, "molecule.yml")]
-    assert 3 == len(result)
+    result = list(util.os_walk(mol_dir, "molecule.yml"))
+    assert len(result) == 3
 
 
 def test_render_template():
     template = "{{ foo }} = {{ bar }}"
 
-    assert "foo = bar" == util.render_template(template, foo="foo", bar="bar")
+    assert util.render_template(template, foo="foo", bar="bar") == "foo = bar"
 
 
 def test_write_file(temp_dir):
     dest_file = os.path.join(temp_dir.strpath, "test_util_write_file.tmp")
     contents = binascii.b2a_hex(os.urandom(15)).decode("utf-8")
     util.write_file(dest_file, contents)
     with util.open_file(dest_file) as stream:
@@ -233,15 +232,15 @@
 ---
 %foo:
 """.strip()
 
     with pytest.raises(SystemExit) as e:
         util.safe_load(data)
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
 
 
 def test_safe_load_file(temp_dir):
     path = os.path.join(temp_dir.strpath, "foo")
     util.write_file(path, "foo: bar")
 
     assert {"foo": "bar"} == util.safe_load_file(path)
@@ -257,15 +256,15 @@
         except NameError:
             file_types = io.IOBase
 
         assert isinstance(stream, file_types)
 
 
 def test_instance_with_scenario_name():
-    assert "foo-bar" == util.instance_with_scenario_name("foo", "bar")
+    assert util.instance_with_scenario_name("foo", "bar") == "foo-bar"
 
 
 def test_verbose_flag():
     options = {"verbose": True, "v": True}
 
     assert ["-v"] == util.verbose_flag(options)
     # pylint: disable=use-implicit-booleaness-not-comparison
@@ -310,23 +309,23 @@
 
 def test_abs_path_with_none_path():
     assert util.abs_path(None) is None
 
 
 # pylint: disable=use-dict-literal
 @pytest.mark.parametrize(
-    "a,b,x",
+    ("a", "b", "x"),
     [
         # Base of recursion scenarios
-        (dict(key=1), dict(key=2), dict(key=2)),
-        (dict(key={}), dict(key=2), dict(key=2)),
-        (dict(key=1), dict(key={}), dict(key={})),
+        ({"key": 1}, {"key": 2}, {"key": 2}),
+        ({"key": {}}, {"key": 2}, {"key": 2}),
+        ({"key": 1}, {"key": {}}, {"key": {}}),
         # Recursive scenario
-        (dict(a=dict(x=1)), dict(a=dict(x=2)), dict(a=dict(x=2))),
-        (dict(a=dict(x=1)), dict(a=dict(y=2)), dict(a=dict(x=1, y=2))),
+        ({"a": {"x": 1}}, {"a": {"x": 2}}, {"a": {"x": 2}}),
+        ({"a": {"x": 1}}, {"a": {"y": 2}}, {"a": {"x": 1, "y": 2}}),
         # example taken from python-anyconfig/anyconfig/__init__.py
         (
             {"b": [{"c": 0}, {"c": 2}], "d": {"e": "aaa", "f": 3}},
             {"a": 1, "b": [{"c": 3}], "d": {"e": "bbb"}},
             {"a": 1, "b": [{"c": 3}], "d": {"e": "bbb", "f": 3}},
         ),
     ],
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/verifier/test_ansible.py` & `molecule-5.0.0a1/src/molecule/test/unit/verifier/test_ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 import pytest
 
 from molecule import config
 from molecule.verifier import ansible
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_ansible_verify(mocker):
     m = mocker.patch("molecule.provisioner.ansible.Ansible.verify")
     m.return_value = "patched-ansible-verify-stdout"
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def _verifier_section_data():
     return {"verifier": {"name": "ansible", "env": {"FOO": "bar"}}}
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(_verifier_section_data, patched_config_validate, config_instance):
     return ansible.Ansible(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -40,19 +40,19 @@
     assert "MOLECULE_INVENTORY_FILE" in _instance.default_env
     assert "MOLECULE_SCENARIO_DIRECTORY" in _instance.default_env
     assert "MOLECULE_INSTANCE_CONFIG" in _instance.default_env
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
 def test_env_property(_instance):
-    assert "bar" == _instance.env["FOO"]
+    assert _instance.env["FOO"] == "bar"
 
 
 def test_name_property(_instance):
-    assert "ansible" == _instance.name
+    assert _instance.name == "ansible"
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 def test_directory_property(_instance):
@@ -85,15 +85,17 @@
     patched_logger_info.assert_any_call(msg)
 
     msg = "Verifier completed successfully."
     patched_logger_info.assert_any_call(msg)
 
 
 def test_execute_does_not_execute(
-    patched_ansible_converge, patched_logger_warning, _instance
+    patched_ansible_converge,
+    patched_logger_warning,
+    _instance,
 ):
     _instance._config.config["verifier"]["enabled"] = False
     _instance.execute()
 
     assert not patched_ansible_converge.called
 
     msg = "Skipping, verifier is disabled."
```

### Comparing `molecule-5.0.0a0/src/molecule/test/unit/verifier/test_testinfra.py` & `molecule-5.0.0a1/src/molecule/test/unit/verifier/test_testinfra.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,48 +23,48 @@
 
 import pytest
 
 from molecule import config, util
 from molecule.verifier import testinfra
 
 
-@pytest.fixture
+@pytest.fixture()
 def _patched_testinfra_get_tests(mocker):
     m = mocker.patch("molecule.verifier.testinfra.Testinfra._get_tests")
     m.return_value = ["foo.py", "bar.py"]
 
     return m
 
 
-@pytest.fixture
+@pytest.fixture()
 def _verifier_section_data():
     return {
         "verifier": {
             "name": "testinfra",
             "options": {"foo": "bar", "v": True, "verbose": True},
             "additional_files_or_dirs": ["file1.py", "file2.py", "match*.py", "dir/*"],
             "env": {"FOO": "bar"},
-        }
+        },
     }
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-@pytest.fixture
+@pytest.fixture()
 def _instance(patched_config_validate, config_instance):
     return testinfra.Testinfra(config_instance)
 
 
-@pytest.fixture
+@pytest.fixture()
 def inventory_file(_instance):
     return _instance._config.provisioner.inventory_file
 
 
-@pytest.fixture
+@pytest.fixture()
 def inventory_directory(_instance):
     return _instance._config.provisioner.inventory_directory
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
@@ -89,15 +89,17 @@
         "p": "no:cacheprovider",
     }
 
     assert x == _instance.default_options
 
 
 def test_default_options_property_updates_sudo(
-    inventory_directory, _instance, _patched_testinfra_get_tests
+    inventory_directory,
+    _instance,
+    _patched_testinfra_get_tests,
 ):
     _instance._config.args = {"sudo": True}
     x = {
         "connection": "ansible",
         "ansible-inventory": inventory_directory,
         "sudo": True,
         "p": "no:cacheprovider",
@@ -130,45 +132,47 @@
 
     x = [file1_file, file2_file, match1_file, match2_file, test_subdir_file]
     assert sorted(x) == sorted(_instance.additional_files_or_dirs)
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
 def test_env_property(_instance):
-    assert "bar" == _instance.env["FOO"]
+    assert _instance.env["FOO"] == "bar"
     assert "ANSIBLE_CONFIG" in _instance.env
     assert "ANSIBLE_ROLES_PATH" in _instance.env
     assert "ANSIBLE_LIBRARY" in _instance.env
     assert "ANSIBLE_FILTER_PLUGINS" in _instance.env
 
 
 def test_name_property(_instance):
-    assert "testinfra" == _instance.name
+    assert _instance.name == "testinfra"
 
 
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 def test_directory_property(_instance):
     parts = _instance.directory.split(os.path.sep)
 
     assert ["molecule", "default", "tests"] == parts[-3:]
 
 
-@pytest.fixture
+@pytest.fixture()
 def _verifier_testinfra_directory_section_data():
     return {"verifier": {"name": "testinfra", "directory": "/tmp/foo/bar"}}
 
 
 @pytest.mark.parametrize(
-    "config_instance", ["_verifier_testinfra_directory_section_data"], indirect=True
+    "config_instance",
+    ["_verifier_testinfra_directory_section_data"],
+    indirect=True,
 )
 def test_directory_property_overridden(_instance):
-    assert "/tmp/foo/bar" == _instance.directory
+    assert _instance.directory == "/tmp/foo/bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
 def test_options_property(inventory_directory, _instance):
     x = {
         "connection": "ansible",
         "ansible-inventory": inventory_directory,
@@ -234,45 +238,51 @@
     calls = [call(msg), call(msg2)]
     patched_logger_info.assert_has_calls(calls)
 
     assert "pytest" in patched_run_command.call_args[0][0].cmd
 
 
 def test_execute_does_not_execute(
-    patched_run_command, patched_logger_warning, _instance
+    patched_run_command,
+    patched_logger_warning,
+    _instance,
 ):
     _instance._config.config["verifier"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, verifier is disabled."
     patched_logger_warning.assert_called_once_with(msg)
 
 
 def test_does_not_execute_without_tests(
-    patched_run_command, patched_logger_warning, _instance
+    patched_run_command,
+    patched_logger_warning,
+    _instance,
 ):
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, no tests found."
     patched_logger_warning.assert_called_once_with(msg)
 
 
 def test_execute_bakes(patched_run_command, _patched_testinfra_get_tests, _instance):
     _instance.execute()
 
     assert _instance._testinfra_command is not None
 
-    assert 1 == patched_run_command.call_count
+    assert patched_run_command.call_count == 1
 
 
 def test_testinfra_executes_catches_and_exits_return_code(
-    patched_run_command, _patched_testinfra_get_tests, _instance
+    patched_run_command,
+    _patched_testinfra_get_tests,
+    _instance,
 ):
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
-    assert 1 == e.value.code
+    assert e.value.code == 1
```

### Comparing `molecule-5.0.0a0/src/molecule/text.py` & `molecule-5.0.0a1/src/molecule/text.py`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/src/molecule/util.py` & `molecule-5.0.0a1/src/molecule/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 """Molecule Utils Module."""
 
-from __future__ import print_function
 
 import contextlib
 import copy
 import fnmatch
 import logging
 import os
 import re
 import sys
+from collections.abc import Iterable, MutableMapping
 from dataclasses import dataclass
 from subprocess import CalledProcessError, CompletedProcess
-from typing import Any, Dict, Iterable, List, MutableMapping, NoReturn, Optional, Union
+from typing import Any, NoReturn, Optional, Union
 from warnings import WarningMessage
 
 import jinja2
 import yaml
 from ansible_compat.ports import cache
 from rich.syntax import Syntax
 
@@ -44,37 +44,37 @@
 LOG = logging.getLogger(__name__)
 
 
 class SafeDumper(yaml.SafeDumper):
     """SafeDumper YAML Class."""
 
     def increase_indent(self, flow=False, indentless=False):
-        return super(SafeDumper, self).increase_indent(flow, False)
+        return super().increase_indent(flow, False)
 
 
 def print_debug(title: str, data: str) -> None:
     """Print debug information."""
     console.print(f"DEBUG: {title}:\n{data}")
 
 
-def print_environment_vars(env: Optional[Dict[str, str]]) -> None:
-    """
-    Print ``Ansible`` and ``Molecule`` environment variables and returns None.
+def print_environment_vars(env: Optional[dict[str, str]]) -> None:
+    """Print ``Ansible`` and ``Molecule`` environment variables and returns None.
 
     :param env: A dict containing the shell's environment as collected by
     ``os.environ``.
     :return: None
     """
     if env:
         ansible_env = {k: v for (k, v) in env.items() if "ANSIBLE_" in k}
         print_debug("ANSIBLE ENVIRONMENT", safe_dump(ansible_env, explicit_start=False))
 
         molecule_env = {k: v for (k, v) in env.items() if "MOLECULE_" in k}
         print_debug(
-            "MOLECULE ENVIRONMENT", safe_dump(molecule_env, explicit_start=False)
+            "MOLECULE ENVIRONMENT",
+            safe_dump(molecule_env, explicit_start=False),
         )
 
         combined_env = ansible_env.copy()
         combined_env.update(molecule_env)
         print_debug(
             "SHELL REPLAY",
             " ".join([f"{k}={v}" for (k, v) in sorted(combined_env.items())]),
@@ -102,48 +102,47 @@
     detail: Optional[MutableMapping] = None,
     warns: Iterable[WarningMessage] = (),
 ) -> None:
     """Exit with an error message."""
     # detail is usually a multi-line string which is not suitable for normal
     # logger.
     if detail:
-        if isinstance(detail, dict):
-            detail_str = safe_dump(detail)
-        else:
-            detail_str = str(detail)
+        detail_str = safe_dump(detail) if isinstance(detail, dict) else str(detail)
         print(detail_str)
     LOG.critical(msg)
 
     for warn in warns:
         LOG.warning(warn.__dict__["message"].args[0])
     sysexit(code)
 
 
 def run_command(
-    cmd, env=None, debug=False, echo=False, quiet=False, check=False, cwd=None
+    cmd,
+    env=None,
+    debug=False,
+    echo=False,
+    quiet=False,
+    check=False,
+    cwd=None,
 ) -> CompletedProcess:
-    """
-    Execute the given command and returns None.
+    """Execute the given command and returns None.
 
     :param cmd: :
         - a string or list of strings (similar to subprocess.run)
         - a BakedCommand object (
     :param debug: An optional bool to toggle debug output.
     """
     args = []
     if cmd.__class__.__name__ == "Command":
         raise RuntimeError(
             "Molecule 3.2.0 dropped use of sh library, update plugin code to use new API. "
-            "See https://github.com/ansible-community/molecule/issues/2678"
+            "See https://github.com/ansible-community/molecule/issues/2678",
         )
     elif cmd.__class__.__name__ == "BakedCommand":
-        if cmd.env and env:
-            env = dict(cmd.env, **env)
-        else:
-            env = cmd.env or env
+        env = dict(cmd.env, **env) if cmd.env and env else cmd.env or env
         args = cmd.cmd
     else:
         args = cmd
 
     if debug:
         print_environment_vars(env)
 
@@ -179,16 +178,15 @@
     t = jinja2.Environment()
     t = t.from_string(template)
 
     return t.render(kwargs)
 
 
 def write_file(filename: str, content: str, header: Optional[str] = None) -> None:
-    """
-    Write a file with the given filename and content and returns None.
+    """Write a file with the given filename and content and returns None.
 
     :param filename: A string containing the target filename.
     :param content: A string containing the data to be written.
     :param header: A header, if None it will use default header.
     :return: None
     """
     if header is None:
@@ -200,68 +198,66 @@
 
 def molecule_prepender(content: str) -> str:
     """Return molecule identification header."""
     return MOLECULE_HEADER + "\n\n" + content
 
 
 def file_prepender(filename: str) -> None:
-    """
-    Prepend an informational header on files managed by Molecule and returns \
+    """Prepend an informational header on files managed by Molecule and returns \
     None.
 
     :param filename: A string containing the target filename.
     :return: None
     """
     with open_file(filename, "r+") as f:
         content = f.read()
         f.seek(0, 0)
         f.write(molecule_prepender(content))
 
 
 def safe_dump(data: Any, explicit_start=True) -> str:
-    """
-    Dump the provided data to a YAML document and returns a string.
+    """Dump the provided data to a YAML document and returns a string.
 
     :param data: A string containing an absolute path to the file to parse.
     :return: str
     """
     return yaml.dump(
-        data, Dumper=SafeDumper, default_flow_style=False, explicit_start=explicit_start
+        data,
+        Dumper=SafeDumper,
+        default_flow_style=False,
+        explicit_start=explicit_start,
     )
 
 
-def safe_load(string) -> Dict:
-    """
-    Parse the provided string returns a dict.
+def safe_load(string) -> dict:
+    """Parse the provided string returns a dict.
 
     :param string: A string to be parsed.
     :return: dict
     """
     try:
         return yaml.safe_load(string) or {}
     except yaml.scanner.ScannerError as e:
         sysexit_with_message(str(e))
     return {}
 
 
 def safe_load_file(filename: str):
-    """
-    Parse the provided YAML file and returns a dict.
+    """Parse the provided YAML file and returns a dict.
 
     :param filename: A string containing an absolute path to the file to parse.
     :return: dict
     """
     with open_file(filename) as stream:
         return safe_load(stream)
 
 
 @contextlib.contextmanager
 def open_file(filename, mode="r"):
-    """
-    Open the provide file safely and returns a file type.
+    """Open the provide file safely and returns a file type.
 
     :param filename: A string containing an absolute path to the file to open.
     :param mode: A string describing the way in which the file will be used.
     :return: file type
     """
     with open(filename, mode) as stream:
         yield stream
@@ -272,15 +268,15 @@
     return f"{instance_name}-{scenario_name}"
 
 
 def verbose_flag(options):
     """Return computed verbosity flag."""
     verbose = "v"
     verbose_flag = []
-    for i in range(0, 3):
+    for _i in range(0, 3):
         if options.get(verbose):
             verbose_flag = [f"-{verbose}"]
             del options[verbose]
             if options.get("verbose"):
                 del options["verbose"]
             break
         verbose = verbose + "v"
@@ -297,16 +293,15 @@
     """Return absolute path."""
     if path:
         return os.path.abspath(path)
     return None
 
 
 def merge_dicts(a: MutableMapping, b: MutableMapping) -> MutableMapping:
-    """
-    Merge the values of b into a and returns a new dict.
+    """Merge the values of b into a and returns a new dict.
 
     This function uses the same algorithm as Ansible's `combine(recursive=True)` filter.
 
     :param a: the target dictionary
     :param b: the dictionary to import
     :return: dict
     """
@@ -384,44 +379,44 @@
 
     if normalized_value in BOOLEANS_TRUE:
         return True
     elif normalized_value in BOOLEANS_FALSE or not strict:
         return False
 
     raise TypeError(
-        f"The value '{value!s}' is not a valid boolean.  Valid booleans include: {', '.join(repr(i) for i in BOOLEANS)!s}"
+        f"The value '{value!s}' is not a valid boolean.  Valid booleans include: {', '.join(repr(i) for i in BOOLEANS)!s}",
     )
 
 
 @dataclass
 class BakedCommand:
     """Define a subprocess command to be executed."""
 
-    cmd: Union[str, List[str]]
-    env: Optional[Dict]
+    cmd: Union[str, list[str]]
+    env: Optional[dict]
     cwd: Optional[str] = None
     stdout: Any = None
     stderr: Any = None
 
 
-def dict2args(data: Dict) -> List[str]:
+def dict2args(data: dict) -> list[str]:
     """Convert a dictionary of options to command like arguments."""
     result = []
     # keep sorting in order to achieve a predictable behavior
     for k, v in sorted(data.items()):
         if v is not False:
             prefix = "-" if len(k) == 1 else "--"
             result.append(f"{prefix}{k}".replace("_", "-"))
             if v is not True:
                 # { foo: True } should produce --foo without any values
                 result.append(v)
     return result
 
 
-def bool2args(data: bool) -> List[str]:
+def bool2args(data: bool) -> list[str]:
     """Convert a boolean value to command line argument (flag)."""
     return []
 
 
 def print_as_yaml(data: Any) -> None:
     """Render python object as yaml on console."""
     result = Syntax(safe_dump(data), "yaml")
```

### Comparing `molecule-5.0.0a0/src/molecule/verifier/ansible.py` & `molecule-5.0.0a1/src/molecule/verifier/ansible.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 from molecule import util
 from molecule.api import Verifier
 
 log = logging.getLogger(__name__)
 
 
 class Ansible(Verifier):
-    """
-    `Ansible`_ is the default test verifier.
+    """`Ansible`_ is the default test verifier.
 
     Molecule executes a playbook (`verify.yml`) located in the role's
     `scenario.directory`.
 
     ``` yaml
         verifier:
           name: ansible
@@ -87,9 +86,9 @@
         log.info(msg)
 
     def schema(self):
         return {
             "verifier": {
                 "type": "dict",
                 "schema": {"name": {"type": "string", "allowed": ["ansible"]}},
-            }
+            },
         }
```

### Comparing `molecule-5.0.0a0/src/molecule/verifier/base.py` & `molecule-5.0.0a1/src/molecule/verifier/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,67 +22,61 @@
 import abc
 import os
 
 import molecule
 from molecule import util
 
 
-class Verifier(object):
+class Verifier:
     """Verifier Base Class."""
 
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, config=None):
-        """
-        Initialize code for all :ref:`Verifier` classes.
+    def __init__(self, config=None) -> None:
+        """Initialize code for all :ref:`Verifier` classes.
 
         :param config: An instance of a Molecule config.
         :returns: None
         """
         self._config = config
 
     @property
     @abc.abstractmethod
     def name(self):  # pragma: no cover
-        """
-        Name of the verifier and returns a string.
+        """Name of the verifier and returns a string.
 
         :returns: str
         """
 
     @property
     @abc.abstractmethod
     def default_options(self):  # pragma: no cover
-        """
-        Get default CLI arguments provided to ``cmd`` as a dict.
+        """Get default CLI arguments provided to ``cmd`` as a dict.
 
         :return: dict
         """
 
     @property
     @abc.abstractmethod
     def default_env(self):  # pragma: no cover
-        """
-        Get default env variables provided to ``cmd`` as a dict.
+        """Get default env variables provided to ``cmd`` as a dict.
 
         :return: dict
         """
 
     @abc.abstractmethod
     def execute(self, action_args=None):  # pragma: no cover
-        """
-        Execute ``cmd`` and returns None.
+        """Execute ``cmd`` and returns None.
 
         :return: None
         """
 
     @abc.abstractmethod
     def schema(self):  # pragma: no cover
-        """
-        Return validation schema.
+        """Return validation schema.
 
         :return: None
         """
 
     @property
     def enabled(self):
         return self._config.config["verifier"]["enabled"]
@@ -93,47 +87,49 @@
             self._config.scenario.directory,
             self._config.config["verifier"].get("directory", "tests"),
         )
 
     @property
     def options(self):
         return util.merge_dicts(
-            self.default_options, self._config.config["verifier"]["options"]
+            self.default_options,
+            self._config.config["verifier"]["options"],
         )
 
     @property
     def env(self):
         return util.merge_dicts(
-            self.default_env, self._config.config["verifier"]["env"]
+            self.default_env,
+            self._config.config["verifier"]["env"],
         )
 
     def __eq__(self, other):
         """Implement equality comparison."""
         return str(self) == str(other)
 
     def __lt__(self, other):
         """Implement lower than comparison."""
         return str.__lt__(str(self), str(other))
 
     def __hash__(self):
         """Implement hashing."""
         return self.name.__hash__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return readable string representation of object."""
         return self.name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Return detailed string representation of object."""
         return self.name
 
     def template_dir(self):
         p = os.path.abspath(
             os.path.join(
                 os.path.dirname(molecule.__file__),
                 "cookiecutter",
                 "scenario",
                 "verifier",
                 self.name,
-            )
+            ),
         )
         return p
```

### Comparing `molecule-5.0.0a0/src/molecule/verifier/testinfra.py` & `molecule-5.0.0a1/src/molecule/verifier/testinfra.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 from molecule import util
 from molecule.api import Verifier
 
 LOG = logging.getLogger(__name__)
 
 
 class Testinfra(Verifier):
-    """
-    `Testinfra`_ is no longer the default test verifier since version 3.0.
+    """`Testinfra`_ is no longer the default test verifier since version 3.0.
 
     Additional options can be passed to ``testinfra`` through the options
     dict.  Any option set in this section will override the defaults.
 
     !!! note
 
         Molecule will remove any options matching '^[v]+$', and pass ``-vvv``
@@ -84,24 +83,23 @@
             - ../path/to/test_1.py
             - ../path/to/test_2.py
             - ../path/to/directory/*
     ```
     .. _`Testinfra`: https://testinfra.readthedocs.io
     """
 
-    def __init__(self, config=None):
-        """
-        Set up the requirements to execute ``testinfra`` and returns None.
+    def __init__(self, config=None) -> None:
+        """Set up the requirements to execute ``testinfra`` and returns None.
 
         :param config: An instance of a Molecule config.
         :return: None
         """
-        super(Testinfra, self).__init__(config)
+        super().__init__(config)
         self._testinfra_command = None
-        self._tests = []
+        self._tests = []  # type: ignore
 
     @property
     def name(self):
         return "testinfra"
 
     @property
     def default_options(self):
@@ -143,16 +141,15 @@
             glob_list = glob.glob(glob_path)
             if glob_list:
                 files_list.extend(glob_list)
 
         return files_list
 
     def bake(self):
-        """
-        Bake a ``testinfra`` command so it's ready to execute and returns None.
+        """Bake a ``testinfra`` command so it's ready to execute and returns None.
 
         :return: None
         """
         options = self.options
         verbose_flag = util.verbose_flag(options)
         args = verbose_flag
 
@@ -186,43 +183,42 @@
         if result.returncode == 0:
             msg = "Verifier completed successfully."
             LOG.info(msg)
         else:
             util.sysexit(result.returncode)
 
     def _get_tests(self, action_args=None):
-        """
-        Walk the verifier's directory for tests and returns a list.
+        """Walk the verifier's directory for tests and returns a list.
 
         :return: list
         """
         if action_args:
             tests = []
             for arg in action_args:
-                args_tests = [
-                    filename
-                    for filename in util.os_walk(
+                args_tests = list(
+                    util.os_walk(
                         os.path.join(self._config.scenario.directory, arg),
                         "test_*.py",
                         followlinks=True,
-                    )
-                ]
+                    ),
+                )
                 tests.extend(args_tests)
             return sorted(tests)
         else:
             return sorted(
-                [
-                    filename
-                    for filename in util.os_walk(
-                        self.directory, "test_*.py", followlinks=True
-                    )
-                ]
-                + self.additional_files_or_dirs
+                list(
+                    util.os_walk(
+                        self.directory,
+                        "test_*.py",
+                        followlinks=True,
+                    ),
+                )
+                + self.additional_files_or_dirs,
             )
 
     def schema(self):
         return {
             "verifier": {
                 "type": "dict",
                 "schema": {"name": {"type": "string", "allowed": ["testinfra"]}},
-            }
+            },
         }
```

### Comparing `molecule-5.0.0a0/src/molecule.egg-info/PKG-INFO` & `molecule-5.0.0a1/src/molecule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 5.0.0a0
+Version: 5.0.0a1
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
```

### Comparing `molecule-5.0.0a0/src/molecule.egg-info/SOURCES.txt` & `molecule-5.0.0a1/src/molecule.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 .ansible.cfg
 .codespellrc
-.flake8
 .git_archival.txt
 .gitattributes
 .gitignore
 .npmrc
 .packit.yaml
 .pre-commit-config.yaml
-.pylintrc
 .readthedocs.yml
 .yamllint
 DCO_1_1.md
 LICENSE
 MANIFEST.in
 README.md
 bindep.txt
@@ -33,14 +31,16 @@
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/security_bug_report.md
 .github/workflows/ack.yml
 .github/workflows/push.yml
 .github/workflows/release.yml
 .github/workflows/tox.yml
+.vscode/extensions.json
+.vscode/settings.json
 docs/ci.md
 docs/configuration.md
 docs/contributing.md
 docs/examples.md
 docs/faq.md
 docs/getting-started.md
 docs/index.md
@@ -112,14 +112,15 @@
 src/molecule/cookiecutter/scenario/driver/delegated/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
 src/molecule/cookiecutter/scenario/verifier/ansible/cookiecutter.json
 src/molecule/cookiecutter/scenario/verifier/ansible/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/verify.yml
 src/molecule/cookiecutter/scenario/verifier/testinfra/cookiecutter.json
 src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/conftest.py
 src/molecule/cookiecutter/scenario/verifier/testinfra/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/{{cookiecutter.verifier_directory}}/test_default.py
 src/molecule/data/__init__.py
+src/molecule/data/driver.json
 src/molecule/data/molecule.json
 src/molecule/dependency/__init__.py
 src/molecule/dependency/base.py
 src/molecule/dependency/shell.py
 src/molecule/dependency/ansible_galaxy/__init__.py
 src/molecule/dependency/ansible_galaxy/base.py
 src/molecule/dependency/ansible_galaxy/collections.py
@@ -149,14 +150,16 @@
 src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
 src/molecule/test/resources/roles/molecule/meta/main.yml
 src/molecule/test/resources/roles/molecule/tasks/main.yml
 src/molecule/test/resources/sample-collection/galaxy.yml
 src/molecule/test/resources/sample-collection/molecule/default/converge.yml
 src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
 src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+src/molecule/test/resources/schema_instance_files/valid/molecule.yml
 src/molecule/test/resources/templates/cookiecutter.json
 src/molecule/test/resources/templates/{{cookiecutter.repo_name}}/template.yml
 src/molecule/test/scenarios/.flake8
 src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
 src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
 src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
 src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
@@ -274,21 +277,8 @@
 src/molecule/verifier/ansible.py
 src/molecule/verifier/base.py
 src/molecule/verifier/testinfra.py
 tools/get-version.sh
 tools/opts.txt
 tools/smoketest.sh
 tools/test-setup.sh
-tools/update-version.sh
-tools/test-schema/.mocharc.json
-tools/test-schema/package-lock.json
-tools/test-schema/package.json
-tools/test-schema/tsconfig.json
-tools/test-schema/f/molecule.json
-tools/test-schema/negative_test/molecule/platforms_children/molecule.yml
-tools/test-schema/negative_test/molecule/platforms_children/molecule.yml.md
-tools/test-schema/negative_test/molecule/platforms_networks/molecule.yml
-tools/test-schema/negative_test/molecule/platforms_networks/molecule.yml.md
-tools/test-schema/src/schema.spec.ts
-tools/test-schema/test/molecule/cluster/molecule.yml
-tools/test-schema/test/molecule/default/molecule.yml
-tools/test-schema/test/molecule/vagrant/molecule.yml
+tools/update-version.sh
```

### Comparing `molecule-5.0.0a0/src/molecule.egg-info/requires.txt` & `molecule-5.0.0a1/src/molecule.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/tools/test-setup.sh` & `molecule-5.0.0a1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-5.0.0a0/tox.ini` & `molecule-5.0.0a1/tox.ini`

 * *Files identical despite different names*

