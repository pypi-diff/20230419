# Comparing `tmp/jupyverse-0.1.3.tar.gz` & `tmp/jupyverse-0.1.4.tar.gz`

## Comparing `jupyverse-0.1.3.tar` & `jupyverse-0.1.4.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    58946 2020-02-02 00:00:00.000000 jupyverse-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.3/config.yaml
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 jupyverse-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.3/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.3/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.3/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 jupyverse-0.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.3/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.3/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.3/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.3/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/plugins/yjs.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.3/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse/py.typed
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupyverse-0.1.3/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/fps_contents/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0    10716 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/fps_terminals/models.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/fps_yjs/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    15573 2020-02-02 00:00:00.000000 jupyverse-0.1.3/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/test_kernels.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.3/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.3/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.3/README.md
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 jupyverse-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 jupyverse-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    60173 2020-02-02 00:00:00.000000 jupyverse-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.4/config.yaml
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 jupyverse-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.4/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/README.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_kernels.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.4/README.md
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 jupyverse-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyverse-0.1.4/PKG-INFO
```

### Comparing `jupyverse-0.1.3/.pre-commit-config.yaml` & `jupyverse-0.1.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.1.3/CHANGELOG.md` & `jupyverse-0.1.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.4
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.3...a42f7c4d0e951d620108afb4ca25e57da5bae2a1))
+
+### Merged PRs
+
+- Move routes to jupyverse_api [#293](https://github.com/jupyter-server/jupyverse/pull/293) ([@davidbrochart](https://github.com/davidbrochart))
+- Add microservices doc, move CLI to jupyverse_api [#292](https://github.com/jupyter-server/jupyverse/pull/292) ([@davidbrochart](https://github.com/davidbrochart))
+- Don't ignore types for fief_client [#290](https://github.com/jupyter-server/jupyverse/pull/290) ([@davidbrochart](https://github.com/davidbrochart))
+- Update README [#288](https://github.com/jupyter-server/jupyverse/pull/288) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-06&to=2023-04-18&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-06..2023-04-18&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-04-06..2023-04-18&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.3
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.2...b5faf93e3296d855c7ebeda0c25e9861400ad469))
 
 ### Merged PRs
 
 - Add fps-lab and fps-frontend dependencies to jupyverse [#287](https://github.com/jupyter-server/jupyverse/pull/287) ([@davidbrochart](https://github.com/davidbrochart))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-06&to=2023-04-06&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-06..2023-04-06&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.2
 
 No merged PRs
 
 ## 0.1.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.0.50...254a3dfd5f6851e2e79406fab934c8361399ffb6))
```

### Comparing `jupyverse-0.1.3/CONTRIBUTING.md` & `jupyverse-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/config.yaml` & `jupyverse-0.1.4/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/mkdocs.yml` & `jupyverse-0.1.4/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 nav:
 - Overview: index.md
 - install.md
 - Usage:
   - usage/single_user.md
   - usage/multi_user.md
+  - usage/microservices.md
 - Plugins:
   - 'auth': plugins/auth.md
   - 'contents': plugins/contents.md
   - 'frontend': plugins/frontend.md
   - 'lab': plugins/lab.md
   - 'jupyterlab': plugins/jupyterlab.md
   - 'retrolab': plugins/retrolab.md
```

### Comparing `jupyverse-0.1.3/.devcontainer/devcontainer.json` & `jupyverse-0.1.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/.github/workflows/check-release.yml` & `jupyverse-0.1.4/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/binder/jupyter_notebook_config.py` & `jupyverse-0.1.4/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/docs/index.md` & `jupyverse-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/docs/install.md` & `jupyverse-0.1.4/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/docs/jupyter.svg` & `jupyverse-0.1.4/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/docs/plugins/auth.md` & `jupyverse-0.1.4/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/docs/usage/multi_user.md` & `jupyverse-0.1.4/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/docs/usage/single_user.md` & `jupyverse-0.1.4/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse/cli.py` & `jupyverse-0.1.4/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse/static/favicon.ico` & `jupyverse-0.1.4/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse_api/COPYING.md` & `jupyverse-0.1.4/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse_api/pyproject.toml` & `jupyverse-0.1.4/jupyverse_api/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,29 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pydantic >=1.10.6,<2",
+  "fastapi >=0.95.0,<1",
+  "rich-click >=1.6.1,<2",
+  "asphalt >=4.11.0,<5",
+  "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
 
 [project.license]
 text = "BSD 3-Clause License"
 
 [project.urls]
-Source = "https://github.com/jupyter-server/jupyverse/api"
+Source = "https://github.com/jupyter-server/jupyverse/jupyverse_api"
+
+[project.scripts]
+jupyverse = "jupyverse_api.cli:main"
 
 [project.entry-points."asphalt.components"]
 app = "jupyverse_api.main:AppComponent"
 jupyverse = "jupyverse_api.main:JupyverseComponent"
 
 [project.entry-points."jupyverse.components"]
 app = "jupyverse_api.main:AppComponent"
```

### Comparing `jupyverse-0.1.3/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.1.4/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.1.3/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.1.4/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.1.4/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.1.4/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth/COPYING.md` & `jupyverse-0.1.4/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth/pyproject.toml` & `jupyverse-0.1.4/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth/fps_auth/backends.py` & `jupyverse-0.1.4/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth/fps_auth/config.py` & `jupyverse-0.1.4/plugins/auth/fps_auth/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     mode: str = "token"
     token: str = uuid4().hex
     global_email: str = "guest@jupyter.com"
     cookie_secure: bool = False  # FIXME: should default to True, and set to False for tests
     clear_users: bool = False
     test: bool = False
     login_url: Optional[str] = None
+    directory: Optional[str] = None
```

### Comparing `jupyverse-0.1.3/plugins/auth/fps_auth/db.py` & `jupyverse-0.1.4/plugins/auth/fps_auth/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     create_db_and_tables: Any
     get_async_session: Any
     get_user_db: Any
     secret: Any
 
 
 def get_db(auth_config: _AuthConfig) -> Res:
-    jupyter_dir = Path.home() / ".local" / "share" / "jupyter"
+    jupyter_dir = (
+        Path.home() / ".local" / "share" / "jupyter"
+        if auth_config.directory is None
+        else Path(auth_config.directory)
+    )
     jupyter_dir.mkdir(parents=True, exist_ok=True)
     name = "jupyverse"
     if auth_config.test:
         name += "_test"
     secret_path = jupyter_dir / f"{name}_secret"
     userdb_path = jupyter_dir / f"{name}_users.db"
```

### Comparing `jupyverse-0.1.3/plugins/auth/fps_auth/main.py` & `jupyverse-0.1.4/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth/fps_auth/routes.py` & `jupyverse-0.1.4/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth_fief/COPYING.md` & `jupyverse-0.1.4/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth_fief/pyproject.toml` & `jupyverse-0.1.4/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 from fastapi import Depends, HTTPException, Request, Response, WebSocket, status
 from fastapi.security import APIKeyCookie
-from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo  # type: ignore
-from fief_client.integrations.fastapi import FiefAuth  # type: ignore
+from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo
+from fief_client.integrations.fastapi import FiefAuth
 from jupyverse_api.auth import User
 
 from .config import _AuthFiefConfig
 
 
 class Backend:
     def __init__(self, auth_fief_config: _AuthFiefConfig):
```

### Comparing `jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Dict, List
 
 from fastapi import APIRouter, Depends, Query, Request, Response
 from fastapi.responses import RedirectResponse
-from fief_client import FiefAccessTokenInfo  # type: ignore
+from fief_client import FiefAccessTokenInfo
 from jupyverse_api import Router
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 
 from .backend import Backend
 from .config import _AuthFiefConfig
```

### Comparing `jupyverse-0.1.3/plugins/contents/COPYING.md` & `jupyverse-0.1.4/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/contents/pyproject.toml` & `jupyverse-0.1.4/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.1.4/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/contents/fps_contents/routes.py` & `jupyverse-0.1.4/plugins/contents/fps_contents/routes.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,157 +3,142 @@
 import shutil
 from datetime import datetime
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Union, cast
 
 from anyio import open_file
-from fastapi import APIRouter, Depends, HTTPException, Response
-from jupyverse_api.app import App
-from jupyverse_api.auth import Auth, User
-from jupyverse_api.contents import Contents, Content, SaveContent
+from fastapi import HTTPException, Response
+from jupyverse_api.auth import User
+from jupyverse_api.contents import Contents
+from jupyverse_api.contents.models import (
+    Checkpoint,
+    Content,
+    CreateContent,
+    RenameContent,
+    SaveContent,
+)
 from starlette.requests import Request
 
 from .fileid import FileIdManager
-from .models import Checkpoint, CreateContent, RenameContent
 
 
 class _Contents(Contents):
-    def __init__(self, app: App, auth: Auth):
-        super().__init__(app=app)
-
-        router = APIRouter()
-
-        @router.post(
-            "/api/contents/{path:path}/checkpoints",
-            status_code=201,
-        )
-        async def create_checkpoint(
-            path, user: User = Depends(auth.current_user(permissions={"contents": ["write"]}))
-        ):
-            src_path = Path(path)
+    async def create_checkpoint(
+        self,
+        path,
+        user: User,
+    ):
+        src_path = Path(path)
+        dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
+        try:
+            dst_path.parent.mkdir(exist_ok=True)
+            shutil.copyfile(src_path, dst_path)
+        except Exception:
+            # FIXME: return error code?
+            return []
+        mtime = get_file_modification_time(dst_path)
+        return Checkpoint(**{"id": "checkpoint", "last_modified": mtime})
+
+    async def create_content(
+        self,
+        path: Optional[str],
+        request: Request,
+        user: User,
+    ):
+        create_content = CreateContent(**(await request.json()))
+        content_path = Path(create_content.path)
+        if create_content.type == "notebook":
+            available_path = get_available_path(content_path / "Untitled.ipynb")
+            async with await open_file(available_path, "w") as f:
+                await f.write(
+                    json.dumps({"cells": [], "metadata": {}, "nbformat": 4, "nbformat_minor": 5})
+                )
+            src_path = available_path
             dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
             try:
                 dst_path.parent.mkdir(exist_ok=True)
                 shutil.copyfile(src_path, dst_path)
             except Exception:
                 # FIXME: return error code?
-                return []
-            mtime = get_file_modification_time(dst_path)
-            return Checkpoint(**{"id": "checkpoint", "last_modified": mtime})
-
-        @router.post(
-            "/api/contents{path:path}",
-            status_code=201,
-        )
-        async def create_content(
-            path: Optional[str],
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            create_content = CreateContent(**(await request.json()))
-            content_path = Path(create_content.path)
-            if create_content.type == "notebook":
-                available_path = get_available_path(content_path / "Untitled.ipynb")
-                async with await open_file(available_path, "w") as f:
-                    await f.write(
-                        json.dumps(
-                            {"cells": [], "metadata": {}, "nbformat": 4, "nbformat_minor": 5}
-                        )
-                    )
-                src_path = available_path
-                dst_path = (
-                    Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
-                )
-                try:
-                    dst_path.parent.mkdir(exist_ok=True)
-                    shutil.copyfile(src_path, dst_path)
-                except Exception:
-                    # FIXME: return error code?
-                    pass
-            elif create_content.type == "directory":
-                name = "Untitled Folder"
-                available_path = get_available_path(content_path / name, sep=" ")
-                available_path.mkdir(parents=True, exist_ok=True)
+                pass
+        elif create_content.type == "directory":
+            name = "Untitled Folder"
+            available_path = get_available_path(content_path / name, sep=" ")
+            available_path.mkdir(parents=True, exist_ok=True)
+        else:
+            assert create_content.ext is not None
+            available_path = get_available_path(content_path / ("untitled" + create_content.ext))
+            open(available_path, "w").close()
+
+        return await self.read_content(available_path, False)
+
+    async def get_root_content(
+        self,
+        content: int,
+        user: User,
+    ):
+        return await self.read_content("", bool(content))
+
+    async def get_checkpoint(
+        self,
+        path,
+        user: User,
+    ):
+        src_path = Path(path)
+        dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
+        if not dst_path.exists():
+            return []
+        mtime = get_file_modification_time(dst_path)
+        return [Checkpoint(**{"id": "checkpoint", "last_modified": mtime})]
+
+    async def get_content(
+        self,
+        path: str,
+        content: int,
+        user: User,
+    ):
+        return await self.read_content(path, bool(content))
+
+    async def save_content(
+        self,
+        path,
+        request: Request,
+        response: Response,
+        user: User,
+    ):
+        content = SaveContent(**(await request.json()))
+        try:
+            await self.write_content(content)
+        except Exception:
+            raise HTTPException(status_code=404, detail=f"Error saving {content.path}")
+        return await self.read_content(content.path, False)
+
+    async def delete_content(
+        self,
+        path,
+        user: User,
+    ):
+        p = Path(path)
+        if p.exists():
+            if p.is_dir():
+                shutil.rmtree(p)
             else:
-                assert create_content.ext is not None
-                available_path = get_available_path(
-                    content_path / ("untitled" + create_content.ext)
-                )
-                open(available_path, "w").close()
-
-            return await self.read_content(available_path, False)
-
-        @router.get("/api/contents")
-        async def get_root_content(
-            content: int,
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
-        ):
-            return await self.read_content("", bool(content))
-
-        @router.get("/api/contents/{path:path}/checkpoints")
-        async def get_checkpoint(
-            path, user: User = Depends(auth.current_user(permissions={"contents": ["read"]}))
-        ):
-            src_path = Path(path)
-            dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
-            if not dst_path.exists():
-                return []
-            mtime = get_file_modification_time(dst_path)
-            return [Checkpoint(**{"id": "checkpoint", "last_modified": mtime})]
-
-        @router.get("/api/contents/{path:path}")
-        async def get_content(
-            path: str,
-            content: int = 0,
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
-        ):
-            return await self.read_content(path, bool(content))
-
-        @router.put("/api/contents/{path:path}")
-        async def save_content(
-            path,
-            request: Request,
-            response: Response,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            content = SaveContent(**(await request.json()))
-            try:
-                await self.write_content(content)
-            except Exception:
-                raise HTTPException(status_code=404, detail=f"Error saving {content.path}")
-            return await self.read_content(content.path, False)
-
-        @router.delete(
-            "/api/contents/{path:path}",
-            status_code=204,
-        )
-        async def delete_content(
-            path,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            p = Path(path)
-            if p.exists():
-                if p.is_dir():
-                    shutil.rmtree(p)
-                else:
-                    p.unlink()
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
-
-        @router.patch("/api/contents/{path:path}")
-        async def rename_content(
-            path,
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            rename_content = RenameContent(**(await request.json()))
-            Path(path).rename(rename_content.path)
-            return await self.read_content(rename_content.path, False)
+                p.unlink()
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        self.include_router(router)
+    async def rename_content(
+        self,
+        path,
+        request: Request,
+        user: User,
+    ):
+        rename_content = RenameContent(**(await request.json()))
+        Path(path).rename(rename_content.path)
+        return await self.read_content(rename_content.path, False)
 
     async def read_content(
         self, path: Union[str, Path], get_content: bool, as_json: bool = False
     ) -> Content:
         if isinstance(path, str):
             path = Path(path)
         content: Optional[Union[str, Dict, List[Dict]]] = None
```

### Comparing `jupyverse-0.1.3/plugins/frontend/COPYING.md` & `jupyverse-0.1.4/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/frontend/pyproject.toml` & `jupyverse-0.1.4/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/jupyterlab/COPYING.md` & `jupyverse-0.1.4/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.1.4/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from http import HTTPStatus
 from pathlib import Path
 
 import jupyterlab as jupyterlab_module  # type: ignore
-from fastapi import APIRouter, Depends, Response
+from fastapi import Response
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.frontend import FrontendConfig
 from jupyverse_api.jupyterlab import JupyterLab, JupyterLabConfig
 from jupyverse_api.lab import Lab
@@ -21,93 +21,90 @@
         self,
         app: App,
         jupyterlab_config: JupyterLabConfig,
         auth: Auth,
         frontend_config: FrontendConfig,
         lab: Lab,
     ) -> None:
-        super().__init__(app)
+        super().__init__(app, auth)
 
-        router = APIRouter()
-        self.prefix_dir, federated_extensions = lab.init_router(router, "lab")
-        extensions_dir = self.prefix_dir / "share" / "jupyter" / "labextensions"
+        self.jupyterlab_config = jupyterlab_config
+        self.frontend_config = frontend_config
+        self.lab = lab
+        lab.redirect_after_root = "lab"
+
+        extensions_dir = lab.prefix_dir / "share" / "jupyter" / "labextensions"
         self.federated_extensions, self.disabled_extension = lab.get_federated_extensions(
             extensions_dir
         )
         jupyterlab_dir = Path(jupyterlab_module.__file__).parents[1]
 
         if jupyterlab_config.dev_mode:
             self.static_lab_dir = jupyterlab_dir / "dev_mode" / "static"
         else:
-            self.static_lab_dir = self.prefix_dir / "share" / "jupyter" / "lab" / "static"
+            self.static_lab_dir = lab.prefix_dir / "share" / "jupyter" / "lab" / "static"
 
         self.mount(
             "/static/lab",
             StaticFiles(directory=self.static_lab_dir),
             name="static",
         )
 
-        @router.get("/lab")
-        async def get_lab(
-            user: User = Depends(auth.current_user()),
-        ):
-            return HTMLResponse(
-                self.get_index(
-                    "default",
-                    frontend_config.collaborative,
-                    jupyterlab_config.dev_mode,
-                    frontend_config.base_url,
-                )
+    async def get_lab(
+        self,
+        user: User,
+    ):
+        return HTMLResponse(
+            self.get_index(
+                "default",
+                self.frontend_config.collaborative,
+                self.jupyterlab_config.dev_mode,
+                self.frontend_config.base_url,
             )
+        )
 
-        @router.get("/lab/tree/{path:path}")
-        async def load_workspace(
-            path,
-        ):
-            return HTMLResponse(
-                self.get_index(
-                    "default",
-                    frontend_config.collaborative,
-                    jupyterlab_config.dev_mode,
-                    frontend_config.base_url,
-                )
+    async def load_workspace(
+        self,
+        path,
+    ):
+        return HTMLResponse(
+            self.get_index(
+                "default",
+                self.frontend_config.collaborative,
+                self.jupyterlab_config.dev_mode,
+                self.frontend_config.base_url,
             )
-
-        @router.get("/lab/api/workspaces/{name}")
-        async def get_workspace_data(user: User = Depends(auth.current_user())):
-            if user:
-                return json.loads(user.workspace)
-            return {}
-
-        @router.put(
-            "/lab/api/workspaces/{name}",
-            status_code=204,
         )
-        async def set_workspace(
-            request: Request,
-            user: User = Depends(auth.current_user()),
-            user_update=Depends(auth.update_user),
-        ):
-            workspace = (await request.body()).decode("utf-8")
-            await user_update({"workspace": workspace})
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        @router.get("/lab/workspaces/{name}", response_class=HTMLResponse)
-        async def get_workspace(
-            name,
-            user: User = Depends(auth.current_user()),
-        ):
-            return self.get_index(
-                name,
-                frontend_config.collaborative,
-                jupyterlab_config.dev_mode,
-                frontend_config.base_url,
-            )
+    async def get_workspace_data(self, user: User):
+        if user:
+            return json.loads(user.workspace)
+        return {}
+
+    async def set_workspace(
+        self,
+        request: Request,
+        user: User,
+        user_update,
+    ):
+        workspace = (await request.body()).decode("utf-8")
+        await user_update({"workspace": workspace})
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        self.include_router(router)
+    async def get_workspace(
+        self,
+        name,
+        user: User,
+    ):
+        return self.get_index(
+            name,
+            self.frontend_config.collaborative,
+            self.jupyterlab_config.dev_mode,
+            self.frontend_config.base_url,
+        )
 
     def get_index(self, workspace, collaborative, dev_mode, base_url="/"):
         for path in (self.static_lab_dir).glob("main.*.js"):
             main_id = path.name.split(".")[1]
             break
         vendor_id = None
         for path in (self.static_lab_dir).glob("vendors-node_modules_whatwg-fetch_fetch_js.*.js"):
@@ -145,17 +142,19 @@
             "listingsUrl": "/lab/api/listings",
             "mathjaxConfig": "TeX-AMS-MML_HTMLorMML-full,Safe",
             "mode": "multiple-document",
             "notebookVersion": "[1, 9, 0]",
             "quitButton": True,
             "settingsUrl": "/lab/api/settings",
             "store_id": 0,
-            "schemasDir": (self.prefix_dir / "share" / "jupyter" / "lab" / "schemas").as_posix(),
+            "schemasDir": (
+                self.lab.prefix_dir / "share" / "jupyter" / "lab" / "schemas"
+            ).as_posix(),
             "terminalsAvailable": True,
-            "themesDir": (self.prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
+            "themesDir": (self.lab.prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
             "themesUrl": "/lab/api/themes",
             "token": "4e2804532de366abc81e32ab0c6bf68a73716fafbdbb2098",
             "translationsApiUrl": "/lab/api/translations",
             "treePath": "",
             "workspace": workspace,
             "treeUrl": "/lab/tree",
             "workspacesApiUrl": "/lab/api/workspaces",
```

### Comparing `jupyverse-0.1.3/plugins/kernels/COPYING.md` & `jupyverse-0.1.4/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/pyproject.toml` & `jupyverse-0.1.4/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         ctx: Context,
     ) -> AsyncGenerator[None, Optional[BaseException]]:
         ctx.add_resource(self.kernels_config, types=KernelsConfig)
 
         app = await ctx.request_resource(App)
         auth = await ctx.request_resource(Auth)  # type: ignore
         frontend_config = await ctx.request_resource(FrontendConfig)
-        yjs = await ctx.request_resource(Yjs)
+        yjs = (
+            await ctx.request_resource(Yjs)  # type: ignore
+            if self.kernels_config.require_yjs
+            else None
+        )
 
         kernels = _Kernels(app, self.kernels_config, auth, frontend_config, yjs)
         ctx.add_resource(kernels, types=Kernels)
 
         if self.kernels_config.connection_path is not None:
             path = Path(self.kernels_config.connection_path)
             task = asyncio.create_task(kernels.watch_connection_files(path))
```

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/routes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
-import sys
 import uuid
 from http import HTTPStatus
 from pathlib import Path
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Optional, Set, Tuple
 
-from fastapi import APIRouter, Depends, HTTPException, Response
+from fastapi import HTTPException, Response
 from fastapi.responses import FileResponse
 from starlette.requests import Request
 from watchfiles import Change, awatch
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.kernels import Kernels, KernelsConfig
 from jupyverse_api.kernels.models import CreateSession, Execution, Kernel, Notebook, Session
 from jupyverse_api.frontend import FrontendConfig
@@ -28,294 +27,287 @@
 class _Kernels(Kernels):
     def __init__(
         self,
         app: App,
         kernels_config: KernelsConfig,
         auth: Auth,
         frontend_config: FrontendConfig,
-        yjs: Yjs,
+        yjs: Optional[Yjs],
     ) -> None:
-        super().__init__(app)
+        super().__init__(app=app, auth=auth)
+        self.kernels_config = kernels_config
+        self.frontend_config = frontend_config
+        self.yjs = yjs
 
-        router = APIRouter()
-
-        kernelspecs: dict = {}
+        self.kernelspecs: dict = {}
         self.kernel_id_to_connection_file: Dict[str, str] = {}
-        sessions: Dict[str, Session] = {}
-        Path(sys.prefix)
+        self.sessions: Dict[str, Session] = {}
+        self.kernels = kernels
 
-        @router.get("/api/kernelspecs")
-        async def get_kernelspecs(
-            user: User = Depends(auth.current_user(permissions={"kernelspecs": ["read"]})),
-        ):
-            for search_path in kernelspec_dirs():
-                for path in Path(search_path).glob("*/kernel.json"):
-                    with open(path) as f:
-                        spec = json.load(f)
-                    name = path.parent.name
-                    resources = {
-                        f.stem: f"{frontend_config.base_url}kernelspecs/{name}/{f.name}"
-                        for f in path.parent.iterdir()
-                        if f.is_file() and f.name != "kernel.json"
-                    }
-                    kernelspecs[name] = {"name": name, "spec": spec, "resources": resources}
-            return {"default": kernels_config.default_kernel, "kernelspecs": kernelspecs}
-
-        @router.get("/kernelspecs/{kernel_name}/{file_name}")
-        async def get_kernelspec(
-            kernel_name,
-            file_name,
-            user: User = Depends(auth.current_user()),
-        ):
-            for search_path in kernelspec_dirs():
-                file_path = Path(search_path) / kernel_name / file_name
-                if file_path.exists():
-                    return FileResponse(file_path)
-            raise HTTPException(
-                status_code=404, detail=f"Kernelspec {kernel_name}/{file_name} not found"
-            )
+    async def get_kernelspecs(
+        self,
+        user: User,
+    ):
+        for search_path in kernelspec_dirs():
+            for path in Path(search_path).glob("*/kernel.json"):
+                with open(path) as f:
+                    spec = json.load(f)
+                name = path.parent.name
+                resources = {
+                    f.stem: f"{self.frontend_config.base_url}kernelspecs/{name}/{f.name}"
+                    for f in path.parent.iterdir()
+                    if f.is_file() and f.name != "kernel.json"
+                }
+                self.kernelspecs[name] = {"name": name, "spec": spec, "resources": resources}
+        return {"default": self.kernels_config.default_kernel, "kernelspecs": self.kernelspecs}
 
-        @router.get("/api/kernels")
-        async def get_kernels(
-            user: User = Depends(auth.current_user(permissions={"kernels": ["read"]})),
-        ):
-            results = []
-            for kernel_id, kernel in kernels.items():
-                if kernel["server"]:
-                    connections = kernel["server"].connections
-                    last_activity = kernel["server"].last_activity["date"]
-                    execution_state = kernel["server"].last_activity["execution_state"]
-                else:
-                    connections = 0
-                    last_activity = ""
-                    execution_state = "idle"
-                results.append(
-                    {
-                        "id": kernel_id,
-                        "name": kernel["name"],
-                        "connections": connections,
-                        "last_activity": last_activity,
-                        "execution_state": execution_state,
-                    }
-                )
-            return results
+    async def get_kernelspec(
+        self,
+        kernel_name,
+        file_name,
+        user: User,
+    ):
+        for search_path in kernelspec_dirs():
+            file_path = Path(search_path) / kernel_name / file_name
+            if file_path.exists():
+                return FileResponse(file_path)
 
-        @router.delete("/api/sessions/{session_id}", status_code=204)
-        async def delete_session(
-            session_id: str,
-            user: User = Depends(auth.current_user(permissions={"sessions": ["write"]})),
-        ):
-            kernel_id = sessions[session_id].kernel.id
-            kernel_server = kernels[kernel_id]["server"]
-            await kernel_server.stop()
-            del kernels[kernel_id]
-            if kernel_id in self.kernel_id_to_connection_file:
-                del self.kernel_id_to_connection_file[kernel_id]
-            del sessions[session_id]
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
-
-        @router.patch("/api/sessions/{session_id}")
-        async def rename_session(
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"sessions": ["write"]})),
-        ):
-            rename_session = await request.json()
-            session_id = rename_session.pop("id")
-            for key, value in rename_session.items():
-                setattr(sessions[session_id], key, value)
-            return sessions[session_id]
-
-        @router.get("/api/sessions")
-        async def get_sessions(
-            user: User = Depends(auth.current_user(permissions={"sessions": ["read"]})),
-        ):
-            for session in sessions.values():
-                kernel_id = session.kernel.id
-                kernel_server = kernels[kernel_id]["server"]
-                session.kernel.last_activity = kernel_server.last_activity["date"]
-                session.kernel.execution_state = kernel_server.last_activity["execution_state"]
-            return list(sessions.values())
-
-        @router.post(
-            "/api/sessions",
-            status_code=201,
-            response_model=Session,
+        raise HTTPException(
+            status_code=404, detail=f"Kernelspec {kernel_name}/{file_name} not found"
         )
-        async def create_session(
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"sessions": ["write"]})),
-        ):
-            create_session = CreateSession(**(await request.json()))
-            kernel_id = create_session.kernel.id
-            kernel_name = create_session.kernel.name
-            if kernel_name is not None:
-                # launch a new ("internal") kernel
-                kernel_server = KernelServer(
-                    kernelspec_path=Path(find_kernelspec(kernel_name)).as_posix(),
-                    kernel_cwd=str(Path(create_session.path).parent),
-                )
-                kernel_id = str(uuid.uuid4())
-                kernels[kernel_id] = {"name": kernel_name, "server": kernel_server, "driver": None}
-                await kernel_server.start()
-            elif kernel_id is not None:
-                # external kernel
-                kernel_name = kernels[kernel_id]["name"]
-                kernel_server = KernelServer(
-                    connection_file=self.kernel_id_to_connection_file[kernel_id],
-                    write_connection_file=False,
-                )
-                kernels[kernel_id]["server"] = kernel_server
-                await kernel_server.start(launch_kernel=False)
-            else:
-                return
-            session_id = str(uuid.uuid4())
-            session = Session(
-                id=session_id,
-                path=create_session.path,
-                name=create_session.name,
-                type=create_session.type,
-                kernel=Kernel(
-                    id=kernel_id,
-                    name=kernel_name,
-                    connections=kernel_server.connections,
-                    last_activity=kernel_server.last_activity["date"],
-                    execution_state=kernel_server.last_activity["execution_state"],
-                ),
-                notebook=Notebook(
-                    path=create_session.path,
-                    name=create_session.name,
-                ),
-            )
-            sessions[session_id] = session
-            return session
 
-        @router.post("/api/kernels/{kernel_id}/interrupt")
-        async def interrupt_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            if kernel_id in kernels:
-                kernel = kernels[kernel_id]
-                kernel["server"].interrupt()
-                result = {
+    async def get_kernels(
+        self,
+        user: User,
+    ):
+        results = []
+        for kernel_id, kernel in kernels.items():
+            if kernel["server"]:
+                connections = kernel["server"].connections
+                last_activity = kernel["server"].last_activity["date"]
+                execution_state = kernel["server"].last_activity["execution_state"]
+            else:
+                connections = 0
+                last_activity = ""
+                execution_state = "idle"
+            results.append(
+                {
                     "id": kernel_id,
                     "name": kernel["name"],
-                    "connections": kernel["server"].connections,
-                    "last_activity": kernel["server"].last_activity["date"],
-                    "execution_state": kernel["server"].last_activity["execution_state"],
+                    "connections": connections,
+                    "last_activity": last_activity,
+                    "execution_state": execution_state,
                 }
-                return result
+            )
+        return results
 
-        @router.post("/api/kernels/{kernel_id}/restart")
-        async def restart_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            if kernel_id in kernels:
-                kernel = kernels[kernel_id]
-                await kernel["server"].restart()
-                result = {
-                    "id": kernel_id,
-                    "name": kernel["name"],
-                    "connections": kernel["server"].connections,
-                    "last_activity": kernel["server"].last_activity["date"],
-                    "execution_state": kernel["server"].last_activity["execution_state"],
-                }
-                return result
+    async def delete_session(
+        self,
+        session_id: str,
+        user: User,
+    ):
+        kernel_id = self.sessions[session_id].kernel.id
+        kernel_server = kernels[kernel_id]["server"]
+        await kernel_server.stop()
+        del kernels[kernel_id]
+        if kernel_id in self.kernel_id_to_connection_file:
+            del self.kernel_id_to_connection_file[kernel_id]
+        del self.sessions[session_id]
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        @router.post("/api/kernels/{kernel_id}/execute")
-        async def execute_cell(
-            request: Request,
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            r = await request.json()
-            execution = Execution(**r)
-            if kernel_id in kernels:
-                ynotebook = yjs.YDocWebSocketHandler.websocket_server.get_room(
-                    execution.document_id
-                ).document
-                cell = ynotebook.get_cell(execution.cell_idx)
-                cell["outputs"] = []
-
-                kernel = kernels[kernel_id]
-                if not kernel["driver"]:
-                    kernel["driver"] = driver = KernelDriver(
-                        kernelspec_path=Path(find_kernelspec(kernel["name"])).as_posix(),
-                        write_connection_file=False,
-                        connection_file=kernel["server"].connection_file_path,
-                    )
-                    await driver.connect()
-                driver = kernel["driver"]
-
-                await driver.execute(cell)
-                ynotebook.set_cell(execution.cell_idx, cell)
-
-        @router.get("/api/kernels/{kernel_id}")
-        async def get_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["read"]})),
-        ):
-            if kernel_id in kernels:
-                kernel = kernels[kernel_id]
-                result = {
-                    "id": kernel_id,
-                    "name": kernel["name"],
-                    "connections": kernel["server"].connections,
-                    "last_activity": kernel["server"].last_activity["date"],
-                    "execution_state": kernel["server"].last_activity["execution_state"],
-                }
-                return result
+    async def rename_session(
+        self,
+        request: Request,
+        user: User,
+    ):
+        rename_session = await request.json()
+        session_id = rename_session.pop("id")
+        for key, value in rename_session.items():
+            setattr(self.sessions[session_id], key, value)
+        return self.sessions[session_id]
 
-        @router.delete("/api/kernels/{kernel_id}", status_code=204)
-        async def shutdown_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            if kernel_id in kernels:
-                await kernels[kernel_id]["server"].stop()
-                del kernels[kernel_id]
-            for session_id in [k for k, v in sessions.items() if v.kernel.id == kernel_id]:
-                del sessions[session_id]
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
-
-        @router.websocket("/api/kernels/{kernel_id}/channels")
-        async def kernel_channels(
-            kernel_id,
-            session_id,
-            websocket_permissions=Depends(
-                auth.websocket_auth(permissions={"kernels": ["execute"]})
-            ),
-        ):
-            if websocket_permissions is None:
-                return
-            websocket, permissions = websocket_permissions
-            subprotocol = (
-                "v1.kernel.websocket.jupyter.org"
-                if "v1.kernel.websocket.jupyter.org" in websocket["subprotocols"]
-                else None
+    async def get_sessions(
+        self,
+        user: User,
+    ):
+        for session in self.sessions.values():
+            kernel_id = session.kernel.id
+            kernel_server = kernels[kernel_id]["server"]
+            session.kernel.last_activity = kernel_server.last_activity["date"]
+            session.kernel.execution_state = kernel_server.last_activity["execution_state"]
+        return list(self.sessions.values())
+
+    async def create_session(
+        self,
+        request: Request,
+        user: User,
+    ):
+        create_session = CreateSession(**(await request.json()))
+        kernel_id = create_session.kernel.id
+        kernel_name = create_session.kernel.name
+        if kernel_name is not None:
+            # launch a new ("internal") kernel
+            kernel_server = KernelServer(
+                kernelspec_path=Path(find_kernelspec(kernel_name)).as_posix(),
+                kernel_cwd=str(Path(create_session.path).parent),
             )
-            await websocket.accept(subprotocol=subprotocol)
-            accepted_websocket = AcceptedWebSocket(websocket, subprotocol)
-            if kernel_id in kernels:
-                kernel_server = kernels[kernel_id]["server"]
-                if kernel_server is None:
-                    # this is an external kernel
-                    # kernel is already launched, just start a kernel server
-                    kernel_server = KernelServer(
-                        connection_file=kernel_id,
-                        write_connection_file=False,
-                    )
-                    await kernel_server.start(launch_kernel=False)
-                    kernels[kernel_id]["server"] = kernel_server
-                await kernel_server.serve(accepted_websocket, session_id, permissions)
+            kernel_id = str(uuid.uuid4())
+            kernels[kernel_id] = {"name": kernel_name, "server": kernel_server, "driver": None}
+            await kernel_server.start()
+        elif kernel_id is not None:
+            # external kernel
+            kernel_name = kernels[kernel_id]["name"]
+            kernel_server = KernelServer(
+                connection_file=self.kernel_id_to_connection_file[kernel_id],
+                write_connection_file=False,
+            )
+            kernels[kernel_id]["server"] = kernel_server
+            await kernel_server.start(launch_kernel=False)
+        else:
+            return
+        session_id = str(uuid.uuid4())
+        session = Session(
+            id=session_id,
+            path=create_session.path,
+            name=create_session.name,
+            type=create_session.type,
+            kernel=Kernel(
+                id=kernel_id,
+                name=kernel_name,
+                connections=kernel_server.connections,
+                last_activity=kernel_server.last_activity["date"],
+                execution_state=kernel_server.last_activity["execution_state"],
+            ),
+            notebook=Notebook(
+                path=create_session.path,
+                name=create_session.name,
+            ),
+        )
+        self.sessions[session_id] = session
+        return session
 
-        self.include_router(router)
+    async def interrupt_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            kernel = kernels[kernel_id]
+            kernel["server"].interrupt()
+            result = {
+                "id": kernel_id,
+                "name": kernel["name"],
+                "connections": kernel["server"].connections,
+                "last_activity": kernel["server"].last_activity["date"],
+                "execution_state": kernel["server"].last_activity["execution_state"],
+            }
+            return result
 
-        self.kernels = kernels
+    async def restart_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            kernel = kernels[kernel_id]
+            await kernel["server"].restart()
+            result = {
+                "id": kernel_id,
+                "name": kernel["name"],
+                "connections": kernel["server"].connections,
+                "last_activity": kernel["server"].last_activity["date"],
+                "execution_state": kernel["server"].last_activity["execution_state"],
+            }
+            return result
+
+    async def execute_cell(
+        self,
+        request: Request,
+        kernel_id,
+        user: User,
+    ):
+        if self.yjs is None:
+            raise RuntimeError("Cannot execute without a Yjs plugin.")
+
+        r = await request.json()
+        execution = Execution(**r)
+        if kernel_id in kernels:
+            ynotebook = self.yjs.websocket_server.get_room(execution.document_id).document
+            cell = ynotebook.get_cell(execution.cell_idx)
+            cell["outputs"] = []
+
+            kernel = kernels[kernel_id]
+            if not kernel["driver"]:
+                kernel["driver"] = driver = KernelDriver(
+                    kernelspec_path=Path(find_kernelspec(kernel["name"])).as_posix(),
+                    write_connection_file=False,
+                    connection_file=kernel["server"].connection_file_path,
+                )
+                await driver.connect()
+            driver = kernel["driver"]
+
+            await driver.execute(cell)
+            ynotebook.set_cell(execution.cell_idx, cell)
+
+    async def get_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            kernel = kernels[kernel_id]
+            result = {
+                "id": kernel_id,
+                "name": kernel["name"],
+                "connections": kernel["server"].connections,
+                "last_activity": kernel["server"].last_activity["date"],
+                "execution_state": kernel["server"].last_activity["execution_state"],
+            }
+            return result
+
+    async def shutdown_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            await kernels[kernel_id]["server"].stop()
+            del kernels[kernel_id]
+        for session_id in [k for k, v in self.sessions.items() if v.kernel.id == kernel_id]:
+            del self.sessions[session_id]
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
+
+    async def kernel_channels(
+        self,
+        kernel_id,
+        session_id,
+        websocket_permissions,
+    ):
+        if websocket_permissions is None:
+            return
+        websocket, permissions = websocket_permissions
+        subprotocol = (
+            "v1.kernel.websocket.jupyter.org"
+            if "v1.kernel.websocket.jupyter.org" in websocket["subprotocols"]
+            else None
+        )
+        await websocket.accept(subprotocol=subprotocol)
+        accepted_websocket = AcceptedWebSocket(websocket, subprotocol)
+        if kernel_id in kernels:
+            kernel_server = kernels[kernel_id]["server"]
+            if kernel_server is None:
+                # this is an external kernel
+                # kernel is already launched, just start a kernel server
+                kernel_server = KernelServer(
+                    connection_file=kernel_id,
+                    write_connection_file=False,
+                )
+                await kernel_server.start(launch_kernel=False)
+                kernels[kernel_id]["server"] = kernel_server
+            await kernel_server.serve(accepted_websocket, session_id, permissions)
 
     async def watch_connection_files(self, path: Path) -> None:
         # first time scan, treat everything as added files
         initial_changes = {(Change.added, str(p)) for p in path.iterdir()}
         await self.process_connection_files(initial_changes)
         # then, on every change
         async for changes in awatch(path):
```

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/lab/COPYING.md` & `jupyverse-0.1.4/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/lab/pyproject.toml` & `jupyverse-0.1.4/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/lab/fps_lab/main.py` & `jupyverse-0.1.4/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/COPYING.md` & `jupyverse-0.1.4/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/pyproject.toml` & `jupyverse-0.1.4/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/routes.py` & `jupyverse-0.1.4/plugins/login/fps_login/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 from typing import Optional, cast
 
-from fastapi import APIRouter
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from jupyverse_api.app import App
 from jupyverse_api.auth import AuthConfig
 from jupyverse_api.login import Login
 
 
@@ -17,25 +16,21 @@
     def __init__(
         self,
         app: App,
         auth_config: AuthConfig,
     ) -> None:
         super().__init__(app)
 
-        router = APIRouter()
-        prefix_static = Path(__file__).parent / "static"
+        self.prefix_static = Path(__file__).parent / "static"
 
         # fps_login needs an AuthConfig that has a login_url, such as fps_auth's config
         auth_config = cast(_AuthConfig, auth_config)
         auth_config.login_url = "/login"
 
         self.mount(
             "/static/login",
-            StaticFiles(directory=prefix_static),
+            StaticFiles(directory=self.prefix_static),
             name="static",
         )
 
-        @router.get("/login")
-        async def api_login():
-            return FileResponse(prefix_static / "index.html")
-
-        self.include_router(router)
+    async def get_login(self):
+        return FileResponse(self.prefix_static / "index.html")
```

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/index.html` & `jupyverse-0.1.4/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.1.4/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.1.4/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.1.4/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/nbconvert/COPYING.md` & `jupyverse-0.1.4/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/nbconvert/pyproject.toml` & `jupyverse-0.1.4/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 import tempfile
 from pathlib import Path
 
 import nbconvert
-from fastapi import APIRouter, Depends
 from fastapi.responses import FileResponse
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.nbconvert import Nbconvert
 
 
 class _Nbconvert(Nbconvert):
     def __init__(
         self,
         app: App,
         auth: Auth,
     ) -> None:
-        super().__init__(app)
+        super().__init__(app, auth)
 
-        router = APIRouter()
+    async def get_nbconvert_formats(self):
+        return {
+            name: {"output_mimetype": nbconvert.exporters.get_exporter(name).output_mimetype}
+            for name in nbconvert.exporters.get_export_names()
+        }
 
-        @router.get("/api/nbconvert")
-        async def get_nbconvert_formats():
-            return {
-                name: {"output_mimetype": nbconvert.exporters.get_exporter(name).output_mimetype}
-                for name in nbconvert.exporters.get_export_names()
-            }
-
-        @router.get("/nbconvert/{format}/{path}")
-        async def get_nbconvert_document(
-            format: str,
-            path: str,
-            download: bool,
-            user: User = Depends(auth.current_user(permissions={"nbconvert": ["read"]})),
-        ):
-            exporter = nbconvert.exporters.get_exporter(format)
-            if download:
-                media_type = "application/octet-stream"
-            else:
-                media_type = exporter.output_mimetype
-            tmp_dir = Path(tempfile.mkdtemp())
-            tmp_path = tmp_dir / (Path(path).stem + exporter().file_extension)
-            with open(tmp_path, "wt") as f:
-                f.write(exporter().from_filename(path)[0])
-            return FileResponse(tmp_path, media_type=media_type, filename=tmp_path.name)
-
-        self.include_router(router)
+    async def get_nbconvert_document(
+        self,
+        format: str,
+        path: str,
+        download: bool,
+        user: User,
+    ):
+        exporter = nbconvert.exporters.get_exporter(format)
+        if download:
+            media_type = "application/octet-stream"
+        else:
+            media_type = exporter.output_mimetype
+        tmp_dir = Path(tempfile.mkdtemp())
+        tmp_path = tmp_dir / (Path(path).stem + exporter().file_extension)
+        with open(tmp_path, "wt") as f:
+            f.write(exporter().from_filename(path)[0])
+        return FileResponse(tmp_path, media_type=media_type, filename=tmp_path.name)
```

### Comparing `jupyverse-0.1.3/plugins/noauth/COPYING.md` & `jupyverse-0.1.4/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/noauth/pyproject.toml` & `jupyverse-0.1.4/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.1.4/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/resource_usage/COPYING.md` & `jupyverse-0.1.4/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/resource_usage/pyproject.toml` & `jupyverse-0.1.4/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 import psutil
 from anyio import to_thread
-from fastapi import APIRouter, Depends
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.resource_usage import ResourceUsage, ResourceUsageConfig
 
 
 class _ResourceUsage(ResourceUsage):
     def __init__(
         self,
         app: App,
         auth: Auth,
         resource_usage_config: ResourceUsageConfig,
     ):
-        super().__init__(app)
+        super().__init__(app, auth)
+        self.resource_usage_config = resource_usage_config
 
-        router = APIRouter()
+    async def get_metrics(
+        self,
+        user: User,
+    ):
+        cur_process = psutil.Process()
+        all_processes = [cur_process] + cur_process.children(recursive=True)
 
-        @router.get("/api/metrics/v1")
-        async def get_metrics(
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
+        # Get memory information
+        rss = 0
+        for p in all_processes:
+            try:
+                rss += p.memory_info().rss
+            except (psutil.NoSuchProcess, psutil.AccessDenied):
+                pass
+
+        mem_limit = self.resource_usage_config.mem_limit
+
+        limits = {"memory": {"rss": mem_limit}}
+        if (
+            self.resource_usage_config.mem_limit
+            and self.resource_usage_config.mem_warning_threshold
         ):
-            cur_process = psutil.Process()
-            all_processes = [cur_process] + cur_process.children(recursive=True)
-
-            # Get memory information
-            rss = 0
-            for p in all_processes:
-                try:
-                    rss += p.memory_info().rss
-                except (psutil.NoSuchProcess, psutil.AccessDenied):
-                    pass
-
-            mem_limit = resource_usage_config.mem_limit
-
-            limits = {"memory": {"rss": mem_limit}}
-            if resource_usage_config.mem_limit and resource_usage_config.mem_warning_threshold:
-                limits["memory"]["warn"] = (mem_limit - rss) < (
-                    mem_limit * resource_usage_config.mem_warning_threshold
-                )
-
-            metrics = {"rss": rss, "limits": limits}
-
-            # Optionally get CPU information
-            if resource_usage_config.track_cpu_percent:
-                cpu_count = psutil.cpu_count()
-                cpu_percent = await to_thread.run_sync(_get_cpu_percent, all_processes)
-
-                if resource_usage_config.cpu_limit:
-                    limits["cpu"] = {"cpu": resource_usage_config.cpu_limit}
-                    if resource_usage_config.cpu_warning_threshold:
-                        limits["cpu"]["warn"] = (resource_usage_config.cpu_limit - cpu_percent) < (
-                            resource_usage_config.cpu_limit
-                            * resource_usage_config.cpu_warning_threshold
-                        )
-
-                metrics.update(cpu_percent=cpu_percent, cpu_count=cpu_count)
+            limits["memory"]["warn"] = (mem_limit - rss) < (
+                mem_limit * self.resource_usage_config.mem_warning_threshold
+            )
+
+        metrics = {"rss": rss, "limits": limits}
+
+        # Optionally get CPU information
+        if self.resource_usage_config.track_cpu_percent:
+            cpu_count = psutil.cpu_count()
+            cpu_percent = await to_thread.run_sync(_get_cpu_percent, all_processes)
+
+            if self.resource_usage_config.cpu_limit:
+                limits["cpu"] = {"cpu": self.resource_usage_config.cpu_limit}
+                if self.resource_usage_config.cpu_warning_threshold:
+                    limits["cpu"]["warn"] = (self.resource_usage_config.cpu_limit - cpu_percent) < (
+                        self.resource_usage_config.cpu_limit
+                        * self.resource_usage_config.cpu_warning_threshold
+                    )
 
-            return metrics
+            metrics.update(cpu_percent=cpu_percent, cpu_count=cpu_count)
 
-        self.include_router(router)
+        return metrics
 
 
 def _get_cpu_percent(all_processes):
     def get_cpu_percent(p):
         try:
             return p.cpu_percent(interval=0.05)
         # Avoid littering logs with stack traces complaining
```

### Comparing `jupyverse-0.1.3/plugins/retrolab/COPYING.md` & `jupyverse-0.1.4/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/retrolab/pyproject.toml` & `jupyverse-0.1.4/plugins/retrolab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.1.4/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.1.4/plugins/retrolab/fps_retrolab/routes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,120 @@
 import json
 from pathlib import Path
 
 import retrolab  # type: ignore
-from fastapi import APIRouter, Depends
-from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.frontend import FrontendConfig
 from jupyverse_api.lab import Lab
 from jupyverse_api.retrolab import RetroLab
 
 
 class _RetroLab(RetroLab):
     def __init__(self, app: App, auth: Auth, frontend_config: FrontendConfig, lab: Lab) -> None:
-        super().__init__(app)
+        super().__init__(app, auth, lab)
+        self.frontend_config = frontend_config
+        self.lab = lab
+        self.lab.redirect_after_root = "retro/tree"
 
-        router = APIRouter()
-        prefix_dir, federated_extensions = lab.init_router(router, "retro/tree")
-        retrolab_dir = Path(retrolab.__file__).parent
+        self.retrolab_dir = Path(retrolab.__file__).parent
 
         self.mount(
             "/static/retro",
-            StaticFiles(directory=retrolab_dir / "static"),
+            StaticFiles(directory=self.retrolab_dir / "static"),
             name="static",
         )
 
-        for path in (retrolab_dir / "labextension" / "static").glob("remoteEntry.*.js"):
+        for path in (self.retrolab_dir / "labextension" / "static").glob("remoteEntry.*.js"):
             load = f"static/{path.name}"
             break
-        retro_federated_extensions = [
+
+        self.retro_federated_extensions = [
             {
                 "extension": "./extension",
                 "load": load,
                 "name": "@retrolab/lab-extension",
                 "style": "./style",
             }
         ]
 
-        @router.get("/retro/tree", response_class=HTMLResponse)
-        async def get_tree(
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                "Tree", "tree", frontend_config.collaborative, frontend_config.base_url
-            )
+    async def get_tree(
+        self,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
+            "Tree",
+            "tree",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        @router.get("/retro/notebooks/{path:path}", response_class=HTMLResponse)
-        async def get_notebook(
+    async def get_notebook(
+        self,
+        path,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
             path,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                path, "notebooks", frontend_config.collaborative, frontend_config.base_url
-            )
+            "notebooks",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        @router.get("/retro/edit/{path:path}", response_class=HTMLResponse)
-        async def edit_file(
+    async def edit_file(
+        self,
+        path,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
             path,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(path, "edit", frontend_config.collaborative, frontend_config.base_url)
+            "edit",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        @router.get("/retro/consoles/{path:path}", response_class=HTMLResponse)
-        async def get_console(
+    async def get_console(
+        self,
+        path,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
             path,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                path, "consoles", frontend_config.collaborative, frontend_config.base_url
-            )
-
-        @router.get("/retro/terminals/{name}", response_class=HTMLResponse)
-        async def get_terminal(
-            name: str,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                name, "terminals", frontend_config.collaborative, frontend_config.base_url
-            )
-
-        def get_index(doc_name, retro_page, collaborative, base_url="/"):
-            extensions_dir = prefix_dir / "share" / "jupyter" / "labextensions"
-            federated_extensions, disabled_extension = lab.get_federated_extensions(extensions_dir)
-            page_config = {
-                "appName": "RetroLab",
-                "appNamespace": "retro",
-                "appSettingsDir": (
-                    prefix_dir / "share" / "jupyter" / "lab" / "settings"
-                ).as_posix(),
-                "appUrl": "/lab",
-                "appVersion": retrolab.__version__,
-                "baseUrl": base_url,
-                "cacheFiles": True,
-                "collaborative": collaborative,
-                "disabledExtensions": disabled_extension,
-                "extraLabextensionsPath": [],
-                "federated_extensions": retro_federated_extensions + federated_extensions,
-                "frontendUrl": "/retro/",
-                "fullAppUrl": f"{base_url}lab",
-                "fullLabextensionsUrl": f"{base_url}lab/extensions",
-                "fullLicensesUrl": f"{base_url}lab/api/licenses",
-                "fullListingsUrl": f"{base_url}lab/api/listings",
-                "fullMathjaxUrl": f"{base_url}static/notebook/components/MathJax/MathJax.js",
-                "fullSettingsUrl": f"{base_url}lab/api/settings",
-                "fullStaticUrl": f"{base_url}static/retro",
-                "fullThemesUrl": f"{base_url}lab/api/themes",
-                "fullTranslationsApiUrl": f"{base_url}lab/api/translations",
-                "fullTreeUrl": f"{base_url}lab/tree",
-                "fullWorkspacesApiUrl": f"{base_url}lab/api/workspaces",
-                "labextensionsPath": [
-                    (prefix_dir / "share" / "jupyter" / "labextensions").as_posix()
-                ],
-                "labextensionsUrl": "/lab/extensions",
-                "licensesUrl": "/lab/api/licenses",
-                "listingsUrl": "/lab/api/listings",
-                "mathjaxConfig": "TeX-AMS-MML_HTMLorMML-full,Safe",
-                "retroLogo": False,
-                "retroPage": retro_page,
-                "schemasDir": (prefix_dir / "share" / "jupyter" / "lab" / "schemas").as_posix(),
-                "settingsUrl": "/lab/api/settings",
-                "staticDir": (retrolab_dir / "static").as_posix(),
-                "templatesDir": (retrolab_dir / "templates").as_posix(),
-                "terminalsAvailable": True,
-                "themesDir": (prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
-                "themesUrl": "/lab/api/themes",
-                "translationsApiUrl": "/lab/api/translations",
-                "treeUrl": "/lab/tree",
-                "workspacesApiUrl": "/lab/api/workspaces",
-                "wsUrl": "",
-            }
-            index = (
-                INDEX_HTML.replace("PAGE_CONFIG", json.dumps(page_config))
-                .replace("DOC_NAME", doc_name)
-                .replace("BASE_URL", base_url)
-            )
-            return index
+            "consoles",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        self.include_router(router)
+    async def get_terminal(
+        self,
+        name: str,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
+            name,
+            "terminals",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
 
 INDEX_HTML = """\
 <!DOCTYPE html>
 <html>
 <head>
   <meta charset="utf-8">
@@ -164,7 +137,63 @@
         window.history.replaceState({ }, '', parsedUrl.href);
       }
     })();
   </script>
 </body>
 </html>
 """
+
+
+def get_index(
+    lab, retrolab_dir, retro_federated_extensions, doc_name, retro_page, collaborative, base_url="/"
+):
+    extensions_dir = lab.prefix_dir / "share" / "jupyter" / "labextensions"
+    federated_extensions, disabled_extension = lab.get_federated_extensions(extensions_dir)
+    page_config = {
+        "appName": "RetroLab",
+        "appNamespace": "retro",
+        "appSettingsDir": (lab.prefix_dir / "share" / "jupyter" / "lab" / "settings").as_posix(),
+        "appUrl": "/lab",
+        "appVersion": retrolab.__version__,
+        "baseUrl": base_url,
+        "cacheFiles": True,
+        "collaborative": collaborative,
+        "disabledExtensions": disabled_extension,
+        "extraLabextensionsPath": [],
+        "federated_extensions": retro_federated_extensions + federated_extensions,
+        "frontendUrl": "/retro/",
+        "fullAppUrl": f"{base_url}lab",
+        "fullLabextensionsUrl": f"{base_url}lab/extensions",
+        "fullLicensesUrl": f"{base_url}lab/api/licenses",
+        "fullListingsUrl": f"{base_url}lab/api/listings",
+        "fullMathjaxUrl": f"{base_url}static/notebook/components/MathJax/MathJax.js",
+        "fullSettingsUrl": f"{base_url}lab/api/settings",
+        "fullStaticUrl": f"{base_url}static/retro",
+        "fullThemesUrl": f"{base_url}lab/api/themes",
+        "fullTranslationsApiUrl": f"{base_url}lab/api/translations",
+        "fullTreeUrl": f"{base_url}lab/tree",
+        "fullWorkspacesApiUrl": f"{base_url}lab/api/workspaces",
+        "labextensionsPath": [(lab.prefix_dir / "share" / "jupyter" / "labextensions").as_posix()],
+        "labextensionsUrl": "/lab/extensions",
+        "licensesUrl": "/lab/api/licenses",
+        "listingsUrl": "/lab/api/listings",
+        "mathjaxConfig": "TeX-AMS-MML_HTMLorMML-full,Safe",
+        "retroLogo": False,
+        "retroPage": retro_page,
+        "schemasDir": (lab.prefix_dir / "share" / "jupyter" / "lab" / "schemas").as_posix(),
+        "settingsUrl": "/lab/api/settings",
+        "staticDir": (retrolab_dir / "static").as_posix(),
+        "templatesDir": (retrolab_dir / "templates").as_posix(),
+        "terminalsAvailable": True,
+        "themesDir": (lab.prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
+        "themesUrl": "/lab/api/themes",
+        "translationsApiUrl": "/lab/api/translations",
+        "treeUrl": "/lab/tree",
+        "workspacesApiUrl": "/lab/api/workspaces",
+        "wsUrl": "",
+    }
+    index = (
+        INDEX_HTML.replace("PAGE_CONFIG", json.dumps(page_config))
+        .replace("DOC_NAME", doc_name)
+        .replace("BASE_URL", base_url)
+    )
+    return index
```

### Comparing `jupyverse-0.1.3/plugins/terminals/COPYING.md` & `jupyverse-0.1.4/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/terminals/pyproject.toml` & `jupyverse-0.1.4/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.1.4/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.1.4/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.1.4/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/yjs/COPYING.md` & `jupyverse-0.1.4/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/yjs/pyproject.toml` & `jupyverse-0.1.4/plugins/yjs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.1.4/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.1.4/plugins/yjs/fps_yjs/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import asyncio
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import Optional, Tuple, cast
 from uuid import uuid4
 
 from fastapi import (
-    APIRouter,
-    Depends,
     HTTPException,
     Request,
     Response,
     WebSocketDisconnect,
     status,
 )
 from jupyter_ydoc import ydocs as YDOCS  # type: ignore
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.contents import Contents
 from jupyverse_api.yjs import Yjs
+from jupyverse_api.yjs.models import CreateDocumentSession
 from ypy_websocket.websocket_server import WebsocketServer, YRoom
 from ypy_websocket.ystore import BaseYStore, SQLiteYStore, YDocNotFound
 from ypy_websocket.yutils import YMessageType, YSyncMessageType
 
-from .models import CreateDocumentSession
-
 YFILE = YDOCS["file"]
 AWARENESS = 1
 RENAME_SESSION = 127
 SERVER_SESSION = uuid4().hex
 
 
 class JupyterSQLiteYStore(SQLiteYStore):
@@ -37,260 +34,72 @@
 class _Yjs(Yjs):
     def __init__(
         self,
         app: App,
         auth: Auth,
         contents: Contents,
     ) -> None:
-        super().__init__(app)
-
-        class YDocWebSocketHandler:
-            saving_document: Optional[asyncio.Task]
-            websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
-
-            def __init__(self, websocket, path, permissions):
-                self.websocket = websocket
-                self.can_write = permissions is None or "write" in permissions.get("yjs", [])
-                self.lock = asyncio.Lock()
-                self.room = self.websocket_server.get_room(self.websocket.path)
-                self.set_file_info(path)
-
-            async def get_file_info(self) -> Tuple[str, str, str]:
-                room_name = self.websocket_server.get_room_name(self.room)
-                file_format, file_type, file_id = room_name.split(":", 2)
-                file_path = await contents.file_id_manager.get_path(file_id)
-                if file_path is None:
-                    raise RuntimeError(f"File {self.room.document.path} cannot be found anymore")
-                if file_path != self.room.document.path:
-                    self.room.document.path = file_path
-                return file_format, file_type, file_path
-
-            def set_file_info(self, value: str) -> None:
-                self.websocket_server.rename_room(value, from_room=self.room)
-                self.websocket.path = value
-
-            async def serve(self):
-                self.set_file_info(self.websocket.path)
-                self.saving_document = None
-                self.room.on_message = self.on_message
-
-                # cancel the deletion of the room if it was scheduled
-                if not self.room.is_transient and self.room.cleaner is not None:
-                    self.room.cleaner.cancel()
-
-                if not self.room.is_transient and not self.room.ready:
-                    file_format, file_type, file_path = await self.get_file_info()
-                    is_notebook = file_type == "notebook"
-                    model = await contents.read_content(file_path, True, as_json=is_notebook)
-                    self.last_modified = to_datetime(model.last_modified)
-                    # check again if ready, because loading the file is async
-                    if not self.room.ready:
-                        # try to apply Y updates from the YStore for this document
-                        try:
-                            await self.room.ystore.apply_updates(self.room.ydoc)
-                            read_from_source = False
-                        except YDocNotFound:
-                            # YDoc not found in the YStore, create the document from
-                            # the source file (no change history)
-                            read_from_source = True
-                        if not read_from_source:
-                            # if YStore updates and source file are out-of-sync, resync updates
-                            # with source
-                            if self.room.document.source != model.content:
-                                read_from_source = True
-                        if read_from_source:
-                            self.room.document.source = model.content
-                            await self.room.ystore.encode_state_as_update(self.room.ydoc)
-
-                        self.room.document.dirty = False
-                        self.room.ready = True
-                        self.room.watcher = asyncio.create_task(self.watch_file())
-                        # save the document when changed
-                        self.room.document.observe(self.on_document_change)
-
-                await self.websocket_server.serve(self.websocket)
-                if not self.room.is_transient and not self.room.clients:
-                    # no client in this room after we disconnect
-                    # keep the document for a while in case someone reconnects
-                    self.room.cleaner = asyncio.create_task(self.clean_room())
-
-            async def on_message(self, message: bytes) -> bool:
-                """
-                Called whenever a message is received, before forwarding it to other clients.
-
-                :param message: received message
-                :returns: True if the message must be discarded, False otherwise (default: False).
-                """
-                skip = False
-                byte = message[0]
-                msg = message[1:]
-                if byte == RENAME_SESSION:
-                    # The client moved the document to a different location. After receiving this
-                    # message, we make the current document available under a different url.
-                    # The other clients are automatically notified of this change because
-                    # the path is shared through the Yjs document as well.
-                    new_room_name = msg.decode("utf-8")
-                    self.set_file_info(new_room_name)
-                    self.websocket_server.rename_room(new_room_name, from_room=self.room)
-                    # send rename acknowledge
-                    await self.websocket.send(bytes([RENAME_SESSION, 1]))
-                elif byte == AWARENESS:
-                    # changes = self.room.awareness.get_changes(msg)
-                    # # filter out message depending on changes
-                    # skip = True
-                    pass
-                elif byte == YMessageType.SYNC:
-                    if not self.can_write and msg[0] == YSyncMessageType.SYNC_UPDATE:
-                        skip = True
-                else:
-                    skip = True
-                return skip
-
-            async def watch_file(self):
-                file_format, file_type, file_path = await self.get_file_info()
-                while True:
-                    watcher = contents.file_id_manager.watch(file_path)
-                    async for changes in watcher:
-                        file_format, file_type, new_file_path = await self.get_file_info()
-                        if new_file_path != file_path:
-                            # file was renamed
-                            contents.file_id_manager.unwatch(file_path, watcher)
-                            file_path = new_file_path
-                            break
-                        await self.maybe_load_document()
-
-            async def maybe_load_document(self):
-                file_format, file_type, file_path = await self.get_file_info()
-                async with self.lock:
-                    model = await contents.read_content(file_path, False)
-                # do nothing if the file was saved by us
-                if self.last_modified < to_datetime(model.last_modified):
-                    is_notebook = file_type == "notebook"
-                    model = await contents.read_content(file_path, True, as_json=is_notebook)
-                    self.room.document.source = model.content
-                    self.last_modified = to_datetime(model.last_modified)
-
-            async def clean_room(self) -> None:
-                await asyncio.sleep(60)  # FIXME: pass in config
-                if self.room.watcher:
-                    self.room.watcher.cancel()
-                self.room.document.unobserve()
-                self.websocket_server.delete_room(room=self.room)
-
-            def on_document_change(self, target, event):
-                if target == "state" and "dirty" in event.keys:
-                    dirty = event.keys["dirty"]["newValue"]
-                    if not dirty:
-                        # we cleared the dirty flag, nothing to save
-                        return
-                # unobserve and observe again because the structure of the document may have changed
-                # e.g. a new cell added to a notebook
-                self.room.document.unobserve()
-                self.room.document.observe(self.on_document_change)
-                if self.saving_document is not None and not self.saving_document.done():
-                    # the document is being saved, cancel that
-                    self.saving_document.cancel()
-                    self.saving_document = None
-                self.saving_document = asyncio.create_task(self.maybe_save_document())
-
-            async def maybe_save_document(self):
-                # save after 1 second of inactivity to prevent too frequent saving
-                await asyncio.sleep(1)
-                # if the room cannot be found, don't save
-                try:
-                    file_format, file_type, file_path = await self.get_file_info()
-                except Exception:
-                    return
-                is_notebook = file_type == "notebook"
-                async with self.lock:
-                    model = await contents.read_content(file_path, True, as_json=is_notebook)
-                if self.last_modified < to_datetime(model.last_modified):
-                    # file changed on disk, let's revert
-                    self.room.document.source = model.content
-                    self.last_modified = to_datetime(model.last_modified)
-                    return
-                if model.content != self.room.document.source:
-                    # don't save if not needed
-                    # this also prevents the dirty flag from bouncing between windows of
-                    # the same document opened as different types (e.g. notebook/text editor)
-                    format = "json" if file_type == "notebook" else "text"
-                    content = {
-                        "content": self.room.document.source,
-                        "format": format,
-                        "path": file_path,
-                        "type": file_type,
-                    }
-                    async with self.lock:
-                        await contents.write_content(content)
-                        model = await contents.read_content(file_path, False)
-                        self.last_modified = to_datetime(model.last_modified)
-                self.room.document.dirty = False
+        super().__init__(app=app, auth=auth)
+        self.contents = contents
+        self.websocket_server = YDocWebSocketHandler.websocket_server
+
+    async def serve_room(self, websocket_permissions, path):
+        if websocket_permissions is None:
+            return
+        websocket, permissions = websocket_permissions
+        await websocket.accept()
+        socket = YDocWebSocketHandler(
+            WebsocketAdapter(websocket, path), path, permissions, self.contents
+        )
+        await socket.serve()
 
-        router = APIRouter()
+    async def yjs_websocket(
+        self,
+        path,
+        websocket_permissions,
+    ):
+        await self.serve_room(websocket_permissions, path)
 
-        async def serve_room(websocket_permissions, path):
-            if websocket_permissions is None:
-                return
-            websocket, permissions = websocket_permissions
-            await websocket.accept()
-            socket = YDocWebSocketHandler(WebsocketAdapter(websocket, path), path, permissions)
-            await socket.serve()
-
-        @router.websocket("/api/yjs/{path:path}")
-        async def yjs_websocket(
-            path,
-            websocket_permissions=Depends(
-                auth.websocket_auth(permissions={"yjs": ["read", "write"]})
-            ),
-        ):
-            await serve_room(websocket_permissions, path)
-
-        @router.websocket("/api/collaboration/room/{path:path}")
-        async def collaboration_room_websocket(
-            path,
-            websocket_permissions=Depends(
-                auth.websocket_auth(permissions={"yjs": ["read", "write"]})
-            ),
-        ):
-            await serve_room(websocket_permissions, path)
-
-        @router.put("/api/collaboration/session/{path:path}", status_code=200)
-        async def create_roomid(
-            path,
-            request: Request,
-            response: Response,
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
-        ):
-            # we need to process the request manually
-            # see https://github.com/tiangolo/fastapi/issues/3373#issuecomment-1306003451
-            create_document_session = CreateDocumentSession(**(await request.json()))
-            idx = await contents.file_id_manager.get_id(path)
-            if idx is not None:
-                return {
-                    "format": create_document_session.format,
-                    "type": create_document_session.type,
-                    "fileId": idx,
-                    "sessionId": SERVER_SESSION,
-                }
-
-            idx = await contents.file_id_manager.index(path)
-            if idx is None:
-                raise HTTPException(status_code=404, detail=f"File {path} does not exist")
+    async def collaboration_room_websocket(
+        self,
+        path,
+        websocket_permissions,
+    ):
+        await self.serve_room(websocket_permissions, path)
 
-            response.status_code = status.HTTP_201_CREATED
+    async def create_roomid(
+        self,
+        path,
+        request: Request,
+        response: Response,
+        user: User,
+    ):
+        # we need to process the request manually
+        # see https://github.com/tiangolo/fastapi/issues/3373#issuecomment-1306003451
+        create_document_session = CreateDocumentSession(**(await request.json()))
+        idx = await self.contents.file_id_manager.get_id(path)
+        if idx is not None:
             return {
                 "format": create_document_session.format,
                 "type": create_document_session.type,
                 "fileId": idx,
                 "sessionId": SERVER_SESSION,
             }
 
-        self.include_router(router)
-
-        self.YDocWebSocketHandler = YDocWebSocketHandler
+        idx = await self.contents.file_id_manager.index(path)
+        if idx is None:
+            raise HTTPException(status_code=404, detail=f"File {path} does not exist")
+
+        response.status_code = status.HTTP_201_CREATED
+        return {
+            "format": create_document_session.format,
+            "type": create_document_session.type,
+            "fileId": idx,
+            "sessionId": SERVER_SESSION,
+        }
 
 
 def to_datetime(iso_date: str) -> datetime:
     return datetime.fromisoformat(iso_date.rstrip("Z"))
 
 
 class WebsocketAdapter:
@@ -354,7 +163,193 @@
                 updates_file_path = (p.parent / f".{file_type}:{p.name}.y").as_posix()
                 ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
                 self.rooms[path] = DocumentRoom(file_type, ystore)
             else:
                 # it is a transient document (e.g. awareness)
                 self.rooms[path] = TransientRoom()
         return self.rooms[path]
+
+
+class YDocWebSocketHandler:
+    saving_document: Optional[asyncio.Task]
+    websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
+
+    def __init__(self, websocket, path, permissions, contents: Contents):
+        self.websocket = websocket
+        self.contents = contents
+        self.can_write = permissions is None or "write" in permissions.get("yjs", [])
+        self.lock = asyncio.Lock()
+        self.room = self.websocket_server.get_room(self.websocket.path)
+        self.set_file_info(path)
+
+    async def get_file_info(self) -> Tuple[str, str, str]:
+        room_name = self.websocket_server.get_room_name(self.room)
+        file_format, file_type, file_id = room_name.split(":", 2)
+        file_path = await self.contents.file_id_manager.get_path(file_id)
+        room = cast(DocumentRoom, self.room)
+        if file_path is None:
+            raise RuntimeError(f"File {room.document.path} cannot be found anymore")
+        if file_path != room.document.path:
+            room.document.path = file_path
+        return file_format, file_type, file_path
+
+    def set_file_info(self, value: str) -> None:
+        self.websocket_server.rename_room(value, from_room=self.room)
+        self.websocket.path = value
+
+    async def serve(self):
+        self.set_file_info(self.websocket.path)
+        self.saving_document = None
+        self.room.on_message = self.on_message
+
+        # cancel the deletion of the room if it was scheduled
+        if not self.room.is_transient and self.room.cleaner is not None:
+            self.room.cleaner.cancel()
+
+        if not self.room.is_transient and not self.room.ready:
+            file_format, file_type, file_path = await self.get_file_info()
+            is_notebook = file_type == "notebook"
+            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+            self.last_modified = to_datetime(model.last_modified)
+            # check again if ready, because loading the file is async
+            if not self.room.ready:
+                # try to apply Y updates from the YStore for this document
+                try:
+                    await self.room.ystore.apply_updates(self.room.ydoc)
+                    read_from_source = False
+                except YDocNotFound:
+                    # YDoc not found in the YStore, create the document from
+                    # the source file (no change history)
+                    read_from_source = True
+                if not read_from_source:
+                    # if YStore updates and source file are out-of-sync, resync updates
+                    # with source
+                    if self.room.document.source != model.content:
+                        read_from_source = True
+                if read_from_source:
+                    self.room.document.source = model.content
+                    await self.room.ystore.encode_state_as_update(self.room.ydoc)
+
+                self.room.document.dirty = False
+                self.room.ready = True
+                self.room.watcher = asyncio.create_task(self.watch_file())
+                # save the document when changed
+                self.room.document.observe(self.on_document_change)
+
+        await self.websocket_server.serve(self.websocket)
+        if not self.room.is_transient and not self.room.clients:
+            # no client in this room after we disconnect
+            # keep the document for a while in case someone reconnects
+            self.room.cleaner = asyncio.create_task(self.clean_room())
+
+    async def on_message(self, message: bytes) -> bool:
+        """
+        Called whenever a message is received, before forwarding it to other clients.
+
+        :param message: received message
+        :returns: True if the message must be discarded, False otherwise (default: False).
+        """
+        skip = False
+        byte = message[0]
+        msg = message[1:]
+        if byte == RENAME_SESSION:
+            # The client moved the document to a different location. After receiving this
+            # message, we make the current document available under a different url.
+            # The other clients are automatically notified of this change because
+            # the path is shared through the Yjs document as well.
+            new_room_name = msg.decode("utf-8")
+            self.set_file_info(new_room_name)
+            self.websocket_server.rename_room(new_room_name, from_room=self.room)
+            # send rename acknowledge
+            await self.websocket.send(bytes([RENAME_SESSION, 1]))
+        elif byte == AWARENESS:
+            # changes = self.room.awareness.get_changes(msg)
+            # # filter out message depending on changes
+            # skip = True
+            pass
+        elif byte == YMessageType.SYNC:
+            if not self.can_write and msg[0] == YSyncMessageType.SYNC_UPDATE:
+                skip = True
+        else:
+            skip = True
+        return skip
+
+    async def watch_file(self):
+        file_format, file_type, file_path = await self.get_file_info()
+        while True:
+            watcher = self.contents.file_id_manager.watch(file_path)
+            async for changes in watcher:
+                file_format, file_type, new_file_path = await self.get_file_info()
+                if new_file_path != file_path:
+                    # file was renamed
+                    self.contents.file_id_manager.unwatch(file_path, watcher)
+                    file_path = new_file_path
+                    break
+                await self.maybe_load_document()
+
+    async def maybe_load_document(self):
+        file_format, file_type, file_path = await self.get_file_info()
+        async with self.lock:
+            model = await self.contents.read_content(file_path, False)
+        # do nothing if the file was saved by us
+        if self.last_modified < to_datetime(model.last_modified):
+            is_notebook = file_type == "notebook"
+            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+            self.room.document.source = model.content
+            self.last_modified = to_datetime(model.last_modified)
+
+    async def clean_room(self) -> None:
+        await asyncio.sleep(60)  # FIXME: pass in config
+        room = cast(DocumentRoom, self.room)
+        if room.watcher:
+            room.watcher.cancel()
+        room.document.unobserve()
+        self.websocket_server.delete_room(room=room)
+
+    def on_document_change(self, target, event):
+        if target == "state" and "dirty" in event.keys:
+            dirty = event.keys["dirty"]["newValue"]
+            if not dirty:
+                # we cleared the dirty flag, nothing to save
+                return
+        # unobserve and observe again because the structure of the document may have changed
+        # e.g. a new cell added to a notebook
+        self.room.document.unobserve()
+        self.room.document.observe(self.on_document_change)
+        if self.saving_document is not None and not self.saving_document.done():
+            # the document is being saved, cancel that
+            self.saving_document.cancel()
+            self.saving_document = None
+        self.saving_document = asyncio.create_task(self.maybe_save_document())
+
+    async def maybe_save_document(self):
+        # save after 1 second of inactivity to prevent too frequent saving
+        await asyncio.sleep(1)
+        # if the room cannot be found, don't save
+        try:
+            file_format, file_type, file_path = await self.get_file_info()
+        except Exception:
+            return
+        is_notebook = file_type == "notebook"
+        async with self.lock:
+            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+        if self.last_modified < to_datetime(model.last_modified):
+            # file changed on disk, let's revert
+            self.room.document.source = model.content
+            self.last_modified = to_datetime(model.last_modified)
+            return
+        if model.content != self.room.document.source:
+            # don't save if not needed
+            # this also prevents the dirty flag from bouncing between windows of
+            # the same document opened as different types (e.g. notebook/text editor)
+            format = "json" if file_type == "notebook" else "text"
+            content = {
+                "content": self.room.document.source,
+                "format": format,
+                "path": file_path,
+                "type": file_type,
+            }
+            async with self.lock:
+                await self.contents.write_content(content)
+                model = await self.contents.read_content(file_path, False)
+                self.last_modified = to_datetime(model.last_modified)
+        self.room.document.dirty = False
```

### Comparing `jupyverse-0.1.3/tests/conftest.py` & `jupyverse-0.1.4/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         "run",
         "config.yaml",
         "--set",
         f"component.components.auth.mode={auth_mode}",
         "--set",
         f"component.components.auth.clear_users={str(clear_users).lower()}",
         "--set",
+        "component.components.kernels.require_yjs=true",
+        "--set",
         f"component.port={unused_tcp_port}",
     ]
     p = subprocess.Popen(command_list)
     url = f"http://127.0.0.1:{unused_tcp_port}"
     while True:
         try:
             requests.get(url)
```

### Comparing `jupyverse-0.1.3/tests/test_auth.py` & `jupyverse-0.1.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/tests/test_contents.py` & `jupyverse-0.1.4/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/tests/test_kernels.py` & `jupyverse-0.1.4/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/tests/test_server.py` & `jupyverse-0.1.4/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/tests/test_settings.py` & `jupyverse-0.1.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/tests/utils.py` & `jupyverse-0.1.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/tests/data/notebook0.ipynb` & `jupyverse-0.1.4/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/.gitignore` & `jupyverse-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/COPYING.md` & `jupyverse-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.3/README.md` & `jupyverse-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Build Status](https://github.com/jupyter-server/jupyverse/workflows/CI/badge.svg)](https://github.com/jupyter-server/jupyverse/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # jupyverse
 
-A set of [FPS](https://github.com/jupyter-server/fps) plugins implementing a Jupyter server.
+A set of [Asphalt](https://asphalt.readthedocs.io) components implementing a Jupyter server.
 
 Try it online:
 - JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jlab)
 - RetroLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-rlab)
 
 Documentation is available [here](https://davidbrochart.github.io/jupyverse).
```

### Comparing `jupyverse-0.1.3/pyproject.toml` & `jupyverse-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 [project]
 name = "jupyverse"
 description = "A set of FPS plugins implementing a Jupyter server"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
-    "rich-click >=1.6.1,<2",
-    "asphalt >=4.11.0,<5",
-    "asphalt-web[fastapi] >=1.1.0,<2",
-    "fastapi >=0.95.0,<1",
     "fps-contents >=0.1.2,<1",
     "fps-kernels >=0.1.2,<1",
     "fps-terminals >=0.1.2,<1",
     "fps-nbconvert >=0.1.2,<1",
     "fps-yjs >=0.1.2,<1",
     "fps-lab >=0.1.2,<1",
     "fps-frontend >=0.1.2,<1",
@@ -33,17 +29,14 @@
 
 [project.license]
 text = "BSD 3-Clause License"
 
 [project.urls]
 Homepage = "https://jupyter.org"
 
-[project.scripts]
-jupyverse = "jupyverse.cli:main"
-
 [project.optional-dependencies]
 jupyterlab = ["fps-jupyterlab >=0.1.2,<1"]
 retrolab = ["fps-retrolab >=0.1.2,<1"]
 auth = ["fps-auth >=0.1.2,<1"]
 auth-fief = ["fps-auth-fief >=0.1.2,<1"]
 noauth = ["fps-noauth >=0.1.2,<1"]
 test = [
@@ -74,52 +67,56 @@
   "pip install -e ./plugins/terminals",
   "pip install -e ./plugins/yjs",
   "pip install -e ./plugins/resource_usage",
 ]
 features = ["test"]
 
 [tool.hatch.envs.dev.overrides]
+matrix.frontend.post-install-commands = [
+  { value = "pip install -e ./plugins/jupyterlab", if = ["jupyterlab"]},
+  { value = "pip install -e ./plugins/retrolab", if = ["retrolab"]},
+]
 matrix.auth.post-install-commands = [
   { value = "pip install -e ./plugins/noauth", if = ["noauth"] },
   { value = "pip install -e ./plugins/auth -e ./plugins/login", if = ["auth"] },
   { value = "pip install -e ./plugins/auth_fief", if = ["auth_fief"] },
 ]
-matrix.frontend.post-install-commands = [
-  { value = "pip install -e ./plugins/jupyterlab", if = ["jupyterlab"]},
-  { value = "pip install -e ./plugins/retrolab", if = ["retrolab"]},
+
+matrix.frontend.scripts = [
+  { key = "typecheck1", value = "typecheck0 ./plugins/jupyterlab", if = ["jupyterlab"] },
+  { key = "typecheck1", value = "typecheck0 ./plugins/retrolab", if = ["retrolab"] },
+]
+
+matrix.auth.scripts = [
+  { key = "typecheck", value = "typecheck1 ./plugins/noauth", if = ["noauth"] },
+  { key = "typecheck", value = "typecheck1 ./plugins/auth ./plugins/login", if = ["auth"] },
+  { key = "typecheck", value = "typecheck1 ./plugins/auth_fief", if = ["auth_fief"] },
 ]
 
 [[tool.hatch.envs.dev.matrix]]
 frontend = ["jupyterlab", "retrolab"]
 auth = ["noauth", "auth", "auth_fief"]
 
 [tool.hatch.envs.dev.scripts]
 test = "pytest ./tests -v"
 lint = [
   "black --line-length 100 jupyverse ./plugins",
   "isort --profile=black jupyverse ./plugins",
 ]
-typecheck = [
-  "mypy --no-incremental jupyverse",
-  "mypy --no-incremental jupyverse_api",
-  "mypy --no-incremental plugins/frontend/fps_frontend",
-  "mypy --no-incremental plugins/contents/fps_contents",
-  "mypy --no-incremental plugins/kernels/fps_kernels",
-  "mypy --no-incremental plugins/retrolab/fps_retrolab",
-  "mypy --no-incremental plugins/jupyterlab/fps_jupyterlab",
-  "mypy --no-incremental plugins/lab/fps_lab",
-  "mypy --no-incremental plugins/auth/fps_auth",
-  "mypy --no-incremental plugins/noauth/fps_noauth",
-  "mypy --no-incremental plugins/auth_fief/fps_auth_fief",
-  "mypy --no-incremental plugins/nbconvert/fps_nbconvert",
-  "mypy --no-incremental plugins/yjs/fps_yjs",
-  "mypy --no-incremental plugins/resource_usage/fps_resource_usage",
-  "mypy --no-incremental plugins/terminals/fps_terminals",
-  "mypy --no-incremental plugins/login/fps_login",
-]
+typecheck0 = """mypy --no-incremental \
+./jupyverse_api \
+./plugins/contents \
+./plugins/frontend \
+./plugins/kernels \
+./plugins/lab \
+./plugins/nbconvert \
+./plugins/terminals \
+./plugins/yjs \
+./plugins/resource_usage \
+"""
 
 [tool.hatch.envs.docs]
 features = ["docs"]
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve --dev-addr localhost:8000"
```

### Comparing `jupyverse-0.1.3/PKG-INFO` & `jupyverse-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
-Requires-Dist: asphalt-web[fastapi]<2,>=1.1.0
-Requires-Dist: asphalt<5,>=4.11.0
-Requires-Dist: fastapi<1,>=0.95.0
 Requires-Dist: fps-contents<1,>=0.1.2
 Requires-Dist: fps-frontend<1,>=0.1.2
 Requires-Dist: fps-kernels<1,>=0.1.2
 Requires-Dist: fps-lab<1,>=0.1.2
 Requires-Dist: fps-nbconvert<1,>=0.1.2
 Requires-Dist: fps-terminals<1,>=0.1.2
 Requires-Dist: fps-yjs<1,>=0.1.2
 Requires-Dist: jupyverse-api<1,>=0.1.2
-Requires-Dist: rich-click<2,>=1.6.1
 Provides-Extra: auth
 Requires-Dist: fps-auth<1,>=0.1.2; extra == 'auth'
 Provides-Extra: auth-fief
 Requires-Dist: fps-auth-fief<1,>=0.1.2; extra == 'auth-fief'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
@@ -47,15 +43,15 @@
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/jupyter-server/jupyverse/workflows/CI/badge.svg)](https://github.com/jupyter-server/jupyverse/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # jupyverse
 
-A set of [FPS](https://github.com/jupyter-server/fps) plugins implementing a Jupyter server.
+A set of [Asphalt](https://asphalt.readthedocs.io) components implementing a Jupyter server.
 
 Try it online:
 - JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jlab)
 - RetroLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-rlab)
 
 Documentation is available [here](https://davidbrochart.github.io/jupyverse).
```

