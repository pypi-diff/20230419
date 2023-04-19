# Comparing `tmp/stdatamodels-1.3.1.tar.gz` & `tmp/stdatamodels-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdatamodels-1.3.1.tar", last modified: Fri Mar 31 11:48:36 2023, max compression
+gzip compressed data, was "stdatamodels-1.4.0.tar", last modified: Wed Apr 19 13:24:28 2023, max compression
```

## Comparing `stdatamodels-1.3.1.tar` & `stdatamodels-1.4.0.tar`

### file list

```diff
@@ -1,444 +1,440 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.062425 stdatamodels-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/workflows/cancel_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-31 11:48:36.062425 stdatamodels-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/asdf_in_fits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.958418 stdatamodels-1.3.1/docs/source/jwst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/docs/source/jwst/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/datamodels/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/datamodels/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/datamodels/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/datamodels/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/datamodels/new_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/datamodels/structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/docs/source/jwst/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/docs/source/jwst/transforms/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:48:36.062425 stdatamodels-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.962419 stdatamodels-1.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.966419 stdatamodels-1.3.1/src/stdatamodels/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/asdf_in_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/dynamicdq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    29344 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/fits_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.966419 stdatamodels-1.3.1/src/stdatamodels/jwst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.990420 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/abvega_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/amilg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/apcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/asn.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/barshadow.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/combinedspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/dark.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/darkMIRI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/drizpars.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/drizproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/extract1d_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/extract1dimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/fringe.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/fringefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/gls_rampfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/guider.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ifucube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ifucubepars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ifuimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/irs2.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/lastframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/level1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.990420 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/metaschema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/metaschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/mrsptcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/mrsxartcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multicombinedspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multiexposure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multiextract1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multiprod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multislit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multispec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/nirspec_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/outlierpars.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/pathloss.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/persat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/photom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/pixelarea.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/psfmask.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/rampfitoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/readnoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/rscd.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57881 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schema_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.014422 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/combinedspectable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/contrast.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    90654 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/dq_def.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/flatcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/gain.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ipc.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_channel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_gainfact.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_grating.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_groupgap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_lampmode.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_module.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_nframes.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_ngroups.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_nints.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_noutputs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pchannel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pgrating.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_photmjsr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_tsovisit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mask.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multiexposure.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multislit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/psfmask.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/readnoise.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/regions.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/resolution.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/segmap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/slit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/sosswavegrid.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/spec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specprofile.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/spectrace.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/spectracesingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/spectracetable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/straylight.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/throughput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/trapdensity.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/trapsfilled.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavemap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27691 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/segmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/slit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/sossextractmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/sosswavegrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/speckernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/specprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/spectrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/straylight.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/superbias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.018422 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.038423 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/association.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/headers.fits
--rw-r--r--   0 runner    (1001) docker     (123) 16801920 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/sip.fits
--rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/test.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_multislit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/throughput.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/trapdensity.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/trappars.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/trapsfilled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tsophot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15958 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/wavemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/wcs_ref_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/wfssbkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.042424 stdatamodels-1.3.1/src/stdatamodels/jwst/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/library/basic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.042424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.042424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/jwst_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.042424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.042424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    57153 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.046424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.046424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.958418 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.958418 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.050424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.050424 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    38869 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/src/stdatamodels/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:35.966419 stdatamodels-1.3.1/src/stdatamodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:48:35.000000 stdatamodels-1.3.1/src/stdatamodels.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.050424 stdatamodels-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.054424 stdatamodels-1.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/association.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/association_w_cat.json
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/headers.fits
--rw-r--r--   0 runner    (1001) docker     (123)   501120 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/jwst_image.fits
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/mask.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/nircam_abvega_offset.asdf
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/nonstandard_primary_array.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/nonstandard_primary_array.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/sip.fits
--rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/data/test.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:48:36.062425 stdatamodels-1.3.1/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/anyof_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/basic_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/core_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/deprecated_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/fits_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/required_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/table_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/transform_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/schemas/validation_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_asdf_in_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_embedded_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-31 11:48:25.000000 stdatamodels-1.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.312564 stdatamodels-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.200564 stdatamodels-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.200564 stdatamodels-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-19 13:24:28.312564 stdatamodels-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.200564 stdatamodels-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.204564 stdatamodels-1.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/asdf_in_fits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.196564 stdatamodels-1.4.0/docs/source/jwst/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.204564 stdatamodels-1.4.0/docs/source/jwst/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/datamodels/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/datamodels/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/datamodels/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/datamodels/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/datamodels/new_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/datamodels/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.204564 stdatamodels-1.4.0/docs/source/jwst/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/docs/source/jwst/transforms/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:24:28.312564 stdatamodels-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.204564 stdatamodels-1.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.208564 stdatamodels-1.4.0/src/stdatamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/asdf_in_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/dynamicdq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29597 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/fits_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.208564 stdatamodels-1.4.0/src/stdatamodels/jwst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.224564 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/abvega_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/amilg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/apcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/asn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/barshadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/combinedspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/dark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/darkMIRI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/drizpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/drizproduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/extract1dimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/fringe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/fringefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/guider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ifucube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ifucubepars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ifuimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/irs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/lastframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/level1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.224564 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/metaschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multiexposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multiextract1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multiprod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multislit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/outlierpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/pathloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/persat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/photom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/pixelarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/psfmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/readnoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/rscd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57881 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schema_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.256564 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/combinedspectable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/contrast.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    90805 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/dq_def.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/flatcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/gain.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ipc.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_channel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_gainfact.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_grating.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_groupgap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampmode.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_module.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nframes.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ngroups.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nints.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_noutputs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pchannel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pgrating.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_photmjsr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_tsovisit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mask.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multiexposure.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multislit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/psfmask.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/readnoise.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/regions.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/resolution.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/segmap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/slit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/sosswavegrid.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/spec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specprofile.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/spectrace.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/spectracesingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/spectracetable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/straylight.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/throughput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/trapdensity.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/trapsfilled.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavemap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27691 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/segmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/slit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/sosswavegrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/speckernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/specprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/spectrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/straylight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/superbias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.260564 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.280564 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/association.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 16801920 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14612 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/trapdensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/trappars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/trapsfilled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tsophot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/wavemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/wfssbkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.288564 stdatamodels-1.4.0/src/stdatamodels/jwst/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/library/basic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.288564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.292564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.292564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.292564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57153 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.292564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.292564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.196564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.196564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.300564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.300564 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38542 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/src/stdatamodels/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.208564 stdatamodels-1.4.0/src/stdatamodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-04-19 13:24:28.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:24:27.000000 stdatamodels-1.4.0/src/stdatamodels.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.300564 stdatamodels-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.304564 stdatamodels-1.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/association.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/association_w_cat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/headers.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   501120 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/jwst_image.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/mask.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/nircam_abvega_offset.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/nonstandard_primary_array.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/nonstandard_primary_array.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/sip.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/data/test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:24:28.312564 stdatamodels-1.4.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/anyof_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/basic_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/core_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/deprecated_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/fits_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/required_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/table_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/transform_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/schemas/validation_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_asdf_in_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_embedded_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-19 13:24:12.000000 stdatamodels-1.4.0/tox.ini
```

### Comparing `stdatamodels-1.3.1/.github/pull_request_template.md` & `stdatamodels-1.4.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/.github/workflows/ci.yml` & `stdatamodels-1.4.0/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,18 @@
       - '*'
   pull_request:
   schedule:
     # Weekly Monday 9AM build
     # * is a special character in YAML so you have to quote this string
     - cron: '0 9 * * 1'
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   crds:
     name: retrieve current CRDS context
     runs-on: ubuntu-latest
     env:
       OBSERVATORY: jwst
       CRDS_PATH: /tmp/crds_cache
```

### Comparing `stdatamodels-1.3.1/.github/workflows/ci_cron.yml` & `stdatamodels-1.4.0/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/.github/workflows/publish-to-pypi.yml` & `stdatamodels-1.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/.gitignore` & `stdatamodels-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/CHANGES.rst` & `stdatamodels-1.4.0/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+1.4.1 (unreleased)
+==================
+
+Other
+-----
+
+-
+
+1.4.0 (2023-04-19)
+==================
+
+Other
+-----
+
+- Add pixel replacement step keyword to jwst.datamodels core schema, and change
+  DQ bit 28 from ``UNRELIABLE_RESET`` to ``FLUX_ESTIMATED``. [#149]
+  
+- drop support for Python 3.8 [#143]
+
+- use Mamba to build docs [#155]
+
+- Remove the defunct ``s3_utils`` module, so that ``stpipe`` no longer needs to depend 
+  on this package. This also removes the ``aws`` install option as this is no longer need. [#154]
+  
+- Remove use of deprecated ``pytest-openfiles`` ``pytest`` plugin. This has been replaced by
+  catching ``ResourceWarning``s. [#152]
+
+- Fix open file handles, which were previously ignored by ``pytest-openfiles``, but which raise
+  blocked ``ResourceWarning`` errors. [#153]
+
 1.3.1 (2023-03-31)
 ==================
 
 Other
 -----
 
 - Add units to BARTDELT and HELIDELT jwst keywords in datamodels schema. [#147]
```

### Comparing `stdatamodels-1.3.1/CODE_OF_CONDUCT.md` & `stdatamodels-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/CONTRIBUTING.md` & `stdatamodels-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/LICENSE` & `stdatamodels-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/PKG-INFO` & `stdatamodels-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatamodels
-Version: 1.3.1
+Version: 1.4.0
 Summary: Core support for DataModel classes used in calibration pipelines
 Author: STScI
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -35,34 +35,39 @@
 Project-URL: Homepage, https://github.com/spacetelescope/stdatamodels
 Project-URL: Bug Tracker, https://github.com/spacetelescope/stdatamodels/issues
 Project-URL: Source Code, https://github.com/spacetelescope/stdatamodels
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
-Provides-Extra: aws
 License-File: LICENSE
 
 # stdatamodels
 
 [![CI](https://github.com/spacetelescope/stdatamodels/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/stdatamodels/actions/workflows/ci.yml)
 
 [![codecov](https://codecov.io/gh/spacetelescope/stdatamodels/branch/master/graph/badge.svg?token=TrmUKaTP2t)](https://codecov.io/gh/spacetelescope/stdatamodels)
 
 
-Provides `DataModel`, which is the base class for data models implemented in the JWST calibration software.
+Provides `DataModel`, which is the base class for data models implemented in the JWST and Roman calibration software.
 
 
 ## Unit Tests
 
 A few unit tests require downloading (~500MB) data from CRDS. CRDS must be configured for these tests to pass
 (see the [CRDS User Guide](https://jwst-crds.stsci.edu/static/users_guide/index.html)
 for more information). Minimally (if not on the stsci vpn where the default path of
 `/grp/crds/cache` is available) you will need to set `CRDS_PATH`.
 
 ```bash
 export CRDS_PATH=/tmp/crds_cache/jwst_ops
 ```
+
+These tests can also be skipped with the `no-crds` pytest option
+
+```bash
+pytest --no-crds
+```
```

### Comparing `stdatamodels-1.3.1/README.md` & `stdatamodels-1.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # stdatamodels
 
 [![CI](https://github.com/spacetelescope/stdatamodels/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/stdatamodels/actions/workflows/ci.yml)
 
 [![codecov](https://codecov.io/gh/spacetelescope/stdatamodels/branch/master/graph/badge.svg?token=TrmUKaTP2t)](https://codecov.io/gh/spacetelescope/stdatamodels)
 
 
-Provides `DataModel`, which is the base class for data models implemented in the JWST calibration software.
+Provides `DataModel`, which is the base class for data models implemented in the JWST and Roman calibration software.
 
 
 ## Unit Tests
 
 A few unit tests require downloading (~500MB) data from CRDS. CRDS must be configured for these tests to pass
 (see the [CRDS User Guide](https://jwst-crds.stsci.edu/static/users_guide/index.html)
 for more information). Minimally (if not on the stsci vpn where the default path of
 `/grp/crds/cache` is available) you will need to set `CRDS_PATH`.
 
 ```bash
 export CRDS_PATH=/tmp/crds_cache/jwst_ops
 ```
+
+These tests can also be skipped with the `no-crds` pytest option
+
+```bash
+pytest --no-crds
+```
```

### Comparing `stdatamodels-1.3.1/docs/Makefile` & `stdatamodels-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/asdf_in_fits.rst` & `stdatamodels-1.4.0/docs/source/asdf_in_fits.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/conf.py` & `stdatamodels-1.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/jwst/datamodels/attributes.rst` & `stdatamodels-1.4.0/docs/source/jwst/datamodels/attributes.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/jwst/datamodels/metadata.rst` & `stdatamodels-1.4.0/docs/source/jwst/datamodels/metadata.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/jwst/datamodels/models.rst` & `stdatamodels-1.4.0/docs/source/jwst/datamodels/models.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/jwst/datamodels/new_model.rst` & `stdatamodels-1.4.0/docs/source/jwst/datamodels/new_model.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/jwst/datamodels/structure.rst` & `stdatamodels-1.4.0/docs/source/jwst/datamodels/structure.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/docs/source/jwst/transforms/index.rst` & `stdatamodels-1.4.0/docs/source/jwst/transforms/index.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/pyproject.toml` & `stdatamodels-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "stdatamodels"
 description = "Core support for DataModel classes used in calibration pipelines"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [
     { name = "STScI" },
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Astronomy",
     "License :: OSI Approved :: BSD License",
@@ -45,30 +45,26 @@
 
 [project.optional-dependencies]
 test = [
     "asdf>=2.8.0",
     "psutil",
     "pytest>=4.6.0",
     "pytest-doctestplus",
-    "pytest-openfiles>=0.5.0",
     "crds>=11.16.14",
     "scipy>=1.5",
 ]
 docs = [
     "sphinx",
     "sphinx-automodapi",
     "numpydoc",
     "sphinx-rtd-theme",
     "stsci-rtd-theme",
     "sphinx-asdf>=0.1.1",
     'tomli; python_version <"3.11"',
 ]
-aws = [
-    "stsci-aws-utils>=0.1.2",
-]
 
 [build-system]
 requires = [
     "setuptools>=61.2",
     "setuptools_scm[toml]>=3.4",
     "wheel",
 ]
@@ -127,19 +123,27 @@
 ]
 
 [tool.pytest.ini_options]
 minversion = "4.6"
 doctest_plus = true
 doctest_rst = true
 text_file_format = "rst"
-addopts = "--open-files --color=yes"
+addopts = "--color=yes"
 testpaths = [
     "tests",
     "src/stdatamodels/jwst",
 ]
+filterwarnings = [
+    # This error replaces pytest-openfiles
+    "error::ResourceWarning",
+    # Sometimes turning ResourceWarnings into errors creates an unraisable exception
+    #   e.g. when pyest catches another exception, this will block the turning of
+    #        ResourceWarnings into errors
+    "error::pytest.PytestUnraisableExceptionWarning",
+]
 asdf_schema_tests_enabled = true
 asdf_schema_validate_default = false
 asdf_schema_root = "src/stdatamodels/jwst/datamodels/schemas\nsrc/stdatamodels/jwst/transforms/resources/schemas"
 norecursedirs = [
     "build",
     ".tox",
     ".eggs",
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/asdf_in_fits.py` & `stdatamodels-1.4.0/src/stdatamodels/asdf_in_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/basic_utils.py` & `stdatamodels-1.4.0/src/stdatamodels/basic_utils.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/dqflags.py` & `stdatamodels-1.4.0/src/stdatamodels/dqflags.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/dynamicdq.py` & `stdatamodels-1.4.0/src/stdatamodels/dynamicdq.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/filetype.py` & `stdatamodels-1.4.0/src/stdatamodels/filetype.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/fits_support.py` & `stdatamodels-1.4.0/src/stdatamodels/fits_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,14 +679,21 @@
         When `True` and the FITS file has an ASDF extension, the
         loading/validation of the FITS header will be skipped, loading
         the model only from the ASDF extension.
         When `None`, the value is taken from the environmental SKIP_FITS_UPDATE.
         Otherwise, the default is `False`
     """
     try:
+        return _from_fits(hdulist, schema, context, skip_fits_update=skip_fits_update, **kwargs)
+    except Exception as exc:
+        hdulist.close()
+        raise exc
+
+def _from_fits(hdulist, schema, context, skip_fits_update=None, **kwargs):
+    try:
         ff = from_fits_asdf(hdulist, **kwargs)
     except Exception as exc:
         raise exc.__class__("ERROR loading embedded ASDF: " + str(exc)) from exc
 
     # Determine whether skipping the FITS loading can be done.
     skip_fits_update = _verify_skip_fits_update(
         skip_fits_update, hdulist, ff, context
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/history.py` & `stdatamodels-1.4.0/src/stdatamodels/history.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/__init__.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/__init__.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/abvega_offset.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/abvega_offset.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/amilg.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/amilg.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/apcorr.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/apcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/asn.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/asn.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/barshadow.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/barshadow.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/cube.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/cube.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/dark.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/dark.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/darkMIRI.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/darkMIRI.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/dqflags.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/dqflags.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
          'NO_SAT_CHECK':     2**21,  # Saturation check not available
          'UNRELIABLE_BIAS':  2**22,  # Bias variance large
          'UNRELIABLE_DARK':  2**23,  # Dark variance large
          'UNRELIABLE_SLOPE': 2**24,  # Slope variance large (i.e., noisy pixel)
          'UNRELIABLE_FLAT':  2**25,  # Flat variance large
          'OPEN':             2**26,  # Open pixel (counts move to adjacent pixels)
          'ADJ_OPEN':         2**27,  # Adjacent to open pixel
-         'UNRELIABLE_RESET': 2**28,  # Sensitive to reset anomaly
+         'FLUX_ESTIMATED':   2**28,  # Pixel flux estimated due to missing/bad data
          'MSA_FAILED_OPEN':  2**29,  # Pixel sees light from failed-open shutter
          'OTHER_BAD_PIXEL':  2**30,  # A catch-all flag
          'REFERENCE_PIXEL':  2**31,  # Pixel is a reference pixel
          }
 
 
 # Group-specific flags. Once groups are combined, these flags
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/extract1d_spec.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/flat.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/flat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/fringe.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/fringe.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/gls_rampfit.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/guider.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/guider.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ifucube.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ifucube.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ifucubepars.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ifucubepars.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ifuimage.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ifuimage.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/image.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/image.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/integration.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/integration.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/irs2.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/irs2.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/lastframe.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/lastframe.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/level1b.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/level1b.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/linearity.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/linearity.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/mask.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/mask.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/model_base.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/model_base.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/mrsptcorr.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/mrsxartcorr.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multicombinedspec.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multiexposure.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multiexposure.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multiextract1d.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multiextract1d.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multislit.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multislit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/multispec.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/multispec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/nirspec_flat.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/pathloss.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/pathloss.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/persat.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/persat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/photom.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/photom.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/pixelarea.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/pixelarea.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/quad.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/quad.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/ramp.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/ramp.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/rampfitoutput.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/reference.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/reference.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/reset.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/reset.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/resolution.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/resolution.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/rscd.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/rscd.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/saturation.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/saturation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schema.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schema_editor.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schema_editor.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2398,14 +2398,19 @@
             fits_keyword: S_PERSIS
             blend_table: True
           photom:
             title: Photometric Calibration
             type: string
             fits_keyword: S_PHOTOM
             blend_table: True
+          pixel_replace:
+            title: Pixel Replacment
+            type: string
+            fits_keyword: S_PXREPL
+            blend_table: True
           ramp_fit:
             title: Ramp Fitting
             type: string
             fits_keyword: S_RAMP
             blend_table: True
           refpix:
             title: Reference Pixel Correction
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/slit.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/slit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/sossextractmodel.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/specprofile.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/specprofile.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/spectrace.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/spectrace.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/superbias.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/superbias.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/association.json` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/association.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/headers.fits` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/sip.fits` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/data/test.fits` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_fits.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_models.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,31 +73,31 @@
                           make_models,
                           which_file,
                           skip_fits_update,
                           expected_exp_type):
     """Test skip_fits_update setting"""
     # Setup the FITS file, modifying a header value
     path = make_models[which_file]
-    hduls = fits.open(path)
-    hduls[0].header['exp_type'] = 'FGS_DARK'
+    with fits.open(path) as hduls:
+        hduls[0].header['exp_type'] = 'FGS_DARK'
 
-    # Decide how to skip. If using the environmental,
-    # set that and pass None to the open function.
-    try:
-        del os.environ['SKIP_FITS_UPDATE']
-    except KeyError:
-        # No need to worry, environmental doesn't exist anyways
-        pass
-    if use_env:
-        if skip_fits_update is not None:
-            os.environ['SKIP_FITS_UPDATE'] = str(skip_fits_update)
-            skip_fits_update = None
+        # Decide how to skip. If using the environmental,
+        # set that and pass None to the open function.
+        try:
+            del os.environ['SKIP_FITS_UPDATE']
+        except KeyError:
+            # No need to worry, environmental doesn't exist anyways
+            pass
+        if use_env:
+            if skip_fits_update is not None:
+                os.environ['SKIP_FITS_UPDATE'] = str(skip_fits_update)
+                skip_fits_update = None
 
-    with datamodels.open(hduls, skip_fits_update=skip_fits_update) as model:
-        assert model.meta.exposure.type == expected_exp_type
+        with datamodels.open(hduls, skip_fits_update=skip_fits_update) as model:
+            assert model.meta.exposure.type == expected_exp_type
 
 
 def test_asnmodel_table_size_zero():
     with AsnModel() as dm:
         assert len(dm.asn_table) == 0
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_multislit.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_open.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_open.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,34 +128,14 @@
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", "model_type not found")
         fits_file = t_path('test.fits')
         with datamodels.open(fits_file) as model:
             assert isinstance(model, JwstDataModel)
 
 
-def test_open_fits_s3(s3_root_dir):
-    """Test opening a model from a FITS file on S3"""
-    path = str(s3_root_dir.join("test.fits"))
-    with JwstDataModel() as dm:
-        dm.save(path)
-
-    with datamodels.open("s3://test-s3-data/test.fits") as m:
-        assert isinstance(m, JwstDataModel)
-
-
-def test_open_asdf_s3(s3_root_dir):
-    """Test opening a model from an ASDF file on S3"""
-    path = str(s3_root_dir.join("test.asdf"))
-    with JwstDataModel() as dm:
-        dm.save(path)
-
-    with datamodels.open("s3://test-s3-data/test.asdf") as m:
-        assert isinstance(m, JwstDataModel)
-
-
 def test_open_none():
     with datamodels.open() as model:
         assert isinstance(model, JwstDataModel)
 
 
 def test_open_shape():
     shape = (50, 20)
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_schema.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,14 +167,18 @@
     'wavelengthrange': dm.WavelengthrangeModel,
     'wavemap': dm.WaveMapModel,
     'wcsregions': None,
     'wfssbkg': dm.WfssBkgModel,
 }
 
 
+@pytest.mark.skipif(
+    "config.getoption('--no-crds')",
+    reason="no_crds option was enabled",
+)
 @pytest.mark.parametrize('instrument', ['fgs', 'miri', 'nircam', 'niriss', 'nirspec'])
 def test_crds_selectors_vs_datamodel(jail_environ, instrument):
     log.info(f"crds_path: {crds.config.get_crds_path()}")
     log.info(f"crds_server: {crds.config.get_server_url('jwst')}")
 
     context = crds.get_context_name('jwst')
     dump_files(context)
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_validation.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tests/test_wcs.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/trapdensity.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/trapdensity.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/trappars.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/trappars.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/tsophot.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/tsophot.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/util.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import logging
 
 import asdf
 
 import numpy as np
 from astropy.io import fits
 from stdatamodels import filetype
-from stdatamodels import s3_utils
 from stdatamodels.model_base import _FileReference
 
 from stdatamodels.jwst.library.basic_utils import bytes2human
 
 
 __all__ = ['open', 'NoTypeWarning', 'can_broadcast', 'to_camelcase', 'is_association',
            'check_memory_allocation', "get_available_memory",
@@ -124,34 +123,28 @@
         if isinstance(init, bytes):
             init = init.decode(sys.getfilesystemencoding())
 
         file_name = basename(init)
         file_type = filetype.check(init)
 
         if file_type == "fits":
-            if s3_utils.is_s3_uri(init):
-                hdulist = fits.open(s3_utils.get_object(init))
-            else:
-                hdulist = fits.open(init, memmap=memmap)
+            hdulist = fits.open(init, memmap=memmap)
             file_to_close = hdulist
 
         elif file_type == "asn":
             # Read the file as an association / model container
             try:
                 from jwst.datamodels import ModelContainer
             except ImportError as err:
                 raise ValueError("Cannot open an association file without the jwst package installed") from err
 
             return ModelContainer(init, **kwargs)
 
         elif file_type == "asdf":
-            if s3_utils.is_s3_uri(init):
-                asdffile = asdf.open(s3_utils.get_object(init), copy_arrays=not memmap)
-            else:
-                asdffile = asdf.open(init, copy_arrays=not memmap)
+            asdffile = asdf.open(init, copy_arrays=not memmap)
 
             # Detect model type, then get defined model, and call it.
             new_class = _class_from_model_type(asdffile)
             if new_class is None:
                 # No model class found, so return generic DataModel.
                 model = model_base.JwstDataModel(asdffile, **kwargs)
                 _handle_missing_model_type(model, file_name)
@@ -198,14 +191,16 @@
             else:
                 shape = ()
 
     # First try to get the class name from the primary header
     new_class = _class_from_model_type(hdulist)
     has_model_type = new_class is not None
     if not guess and not has_model_type:
+        if file_to_close is not None:
+            file_to_close.close()
         raise TypeError('Model type is not specifically defined and guessing has been disabled.')
 
     # Special handling for ramp files for backwards compatibility
     if new_class is None:
         new_class = _class_from_ramp_type(hdulist, shape)
 
     # Or get the class from the reference file type and other header keywords
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/wavemap.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/wavemap.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/wcs_ref_models.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/datamodels/wfssbkg.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/datamodels/wfssbkg.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/library/basic_utils.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/library/basic_utils.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/__init__.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/jwst_models.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/converters/tests/test_models.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/extensions.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/extensions.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/integration.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/integration.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/models.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/jwst/transforms/tests/tests.py` & `stdatamodels-1.4.0/src/stdatamodels/jwst/transforms/tests/tests.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/model_base.py` & `stdatamodels-1.4.0/src/stdatamodels/model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from . import filetype
 from . import fits_support
 from . import properties
 from . import schema as mschema
 from . import validate
 from .util import get_envar_as_boolean, remove_none_from_tree
-from . import s3_utils
 
 from .history import HistoryList
 
 
 # This minimal schema creates metadata fields that
 # are accessed to be available by the core DataModel code.
 _DEFAULT_SCHEMA = {
@@ -228,21 +227,15 @@
             if isinstance(init, PurePath):
                 init = str(init)
             if isinstance(init, bytes):
                 init = init.decode(sys.getfilesystemencoding())
             file_type = filetype.check(init)
 
             if file_type == "fits":
-                if s3_utils.is_s3_uri(init):
-                    init_fitsopen = s3_utils.get_object(init)
-                    memmap = None
-                else:
-                    init_fitsopen = init
-
-                hdulist = fits.open(init_fitsopen, memmap=memmap)
+                hdulist = fits.open(init, memmap=memmap)
                 asdffile = fits_support.from_fits(
                     hdulist, self._schema, self._ctx, **kwargs
                 )
                 self._file_references.append(_FileReference(hdulist))
 
             elif file_type == "asdf":
                 asdffile = self.open_asdf(init=init, **kwargs)
@@ -540,16 +533,14 @@
                   ignore_version_mismatch=True,
                   ignore_unrecognized_tag=False,
                   **kwargs):
         """
         Open an asdf object from a filename or create a new asdf object
         """
         if isinstance(init, str):
-            if s3_utils.is_s3_uri(init):
-                init = s3_utils.get_object(init)
             asdffile = asdf.open(init,
                                  ignore_version_mismatch=ignore_version_mismatch,
                                  ignore_unrecognized_tag=ignore_unrecognized_tag)
 
         else:
             asdffile = AsdfFile(init,
                             ignore_version_mismatch=ignore_version_mismatch,
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels/properties.py` & `stdatamodels-1.4.0/src/stdatamodels/properties.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/schema.py` & `stdatamodels-1.4.0/src/stdatamodels/schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/util.py` & `stdatamodels-1.4.0/src/stdatamodels/util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels/validate.py` & `stdatamodels-1.4.0/src/stdatamodels/validate.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/src/stdatamodels.egg-info/PKG-INFO` & `stdatamodels-1.4.0/src/stdatamodels.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatamodels
-Version: 1.3.1
+Version: 1.4.0
 Summary: Core support for DataModel classes used in calibration pipelines
 Author: STScI
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -35,34 +35,39 @@
 Project-URL: Homepage, https://github.com/spacetelescope/stdatamodels
 Project-URL: Bug Tracker, https://github.com/spacetelescope/stdatamodels/issues
 Project-URL: Source Code, https://github.com/spacetelescope/stdatamodels
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
-Provides-Extra: aws
 License-File: LICENSE
 
 # stdatamodels
 
 [![CI](https://github.com/spacetelescope/stdatamodels/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/stdatamodels/actions/workflows/ci.yml)
 
 [![codecov](https://codecov.io/gh/spacetelescope/stdatamodels/branch/master/graph/badge.svg?token=TrmUKaTP2t)](https://codecov.io/gh/spacetelescope/stdatamodels)
 
 
-Provides `DataModel`, which is the base class for data models implemented in the JWST calibration software.
+Provides `DataModel`, which is the base class for data models implemented in the JWST and Roman calibration software.
 
 
 ## Unit Tests
 
 A few unit tests require downloading (~500MB) data from CRDS. CRDS must be configured for these tests to pass
 (see the [CRDS User Guide](https://jwst-crds.stsci.edu/static/users_guide/index.html)
 for more information). Minimally (if not on the stsci vpn where the default path of
 `/grp/crds/cache` is available) you will need to set `CRDS_PATH`.
 
 ```bash
 export CRDS_PATH=/tmp/crds_cache/jwst_ops
 ```
+
+These tests can also be skipped with the `no-crds` pytest option
+
+```bash
+pytest --no-crds
+```
```

### Comparing `stdatamodels-1.3.1/src/stdatamodels.egg-info/SOURCES.txt` & `stdatamodels-1.4.0/src/stdatamodels.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 tox.ini
 .github/CODEOWNERS
 .github/pull_request_template.md
-.github/workflows/cancel_workflows.yml
 .github/workflows/changelog.yml
 .github/workflows/ci.yml
 .github/workflows/ci_cron.yml
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
+docs/rtd_environment.yaml
 docs/source/api.rst
 docs/source/asdf_in_fits.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/jwst/datamodels/attributes.rst
 docs/source/jwst/datamodels/index.rst
 docs/source/jwst/datamodels/metadata.rst
@@ -36,27 +36,25 @@
 src/stdatamodels/dqflags.py
 src/stdatamodels/dynamicdq.py
 src/stdatamodels/filetype.py
 src/stdatamodels/fits_support.py
 src/stdatamodels/history.py
 src/stdatamodels/model_base.py
 src/stdatamodels/properties.py
-src/stdatamodels/s3_utils.py
 src/stdatamodels/schema.py
 src/stdatamodels/util.py
 src/stdatamodels/validate.py
 src/stdatamodels.egg-info/PKG-INFO
 src/stdatamodels.egg-info/SOURCES.txt
 src/stdatamodels.egg-info/dependency_links.txt
 src/stdatamodels.egg-info/entry_points.txt
 src/stdatamodels.egg-info/requires.txt
 src/stdatamodels.egg-info/top_level.txt
 src/stdatamodels.egg-info/zip-safe
 src/stdatamodels/jwst/__init__.py
-src/stdatamodels/jwst/helpers.py
 src/stdatamodels/jwst/datamodels/__init__.py
 src/stdatamodels/jwst/datamodels/abvega_offset.py
 src/stdatamodels/jwst/datamodels/amilg.py
 src/stdatamodels/jwst/datamodels/apcorr.py
 src/stdatamodels/jwst/datamodels/asn.py
 src/stdatamodels/jwst/datamodels/barshadow.py
 src/stdatamodels/jwst/datamodels/combinedspec.py
@@ -371,25 +369,23 @@
 src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
 src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
 src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
 src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
 src/stdatamodels/jwst/transforms/tests/__init__.py
 src/stdatamodels/jwst/transforms/tests/tests.py
 tests/conftest.py
-tests/helpers.py
 tests/models.py
 tests/test_asdf_in_fits.py
 tests/test_dq.py
 tests/test_embedded_asdf.py
 tests/test_filetype.py
 tests/test_fits.py
 tests/test_history.py
 tests/test_models.py
 tests/test_resources.py
-tests/test_s3_utils.py
 tests/test_schema.py
 tests/test_storage.py
 tests/test_util.py
 tests/test_validation.py
 tests/data/association.json
 tests/data/association_w_cat.json
 tests/data/headers.fits
```

### Comparing `stdatamodels-1.3.1/tests/conftest.py` & `stdatamodels-1.4.0/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 """Project default for pytest"""
 from pathlib import Path
 
 import pytest
 
 import asdf
 
-import helpers
-from stdatamodels import s3_utils
-
-
-@pytest.fixture(autouse=True)
-def monkey_patch_s3_client(monkeypatch, request):
-    # If tmpdir is used in the test, then it is providing the file.  Map to it.
-    if "s3_root_dir" in request.fixturenames:
-        path = request.getfixturevalue("s3_root_dir")
-    else:
-        path = None
-    monkeypatch.setattr(s3_utils, "_CLIENT", helpers.MockS3Client(path))
-
-
-@pytest.fixture
-def s3_root_dir(tmpdir):
-    return tmpdir
 
+def pytest_addoption(parser):
+    parser.addoption(
+        "--no-crds",
+        action="store_true",
+        default=False,
+        help="Skip tests against crds",
+    )
 
 @pytest.fixture(scope="session", autouse=True)
 def register_schemas():
     schemas_root = Path(__file__).parent/"schemas"
     with asdf.config_context() as config:
         config.add_resource_mapping(
             asdf.resource.DirectoryResourceMapping(schemas_root, "http://example.com/schemas")
```

### Comparing `stdatamodels-1.3.1/tests/data/association.json` & `stdatamodels-1.4.0/tests/data/association.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/association_w_cat.json` & `stdatamodels-1.4.0/tests/data/association_w_cat.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/headers.fits` & `stdatamodels-1.4.0/tests/data/headers.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/jwst_image.fits` & `stdatamodels-1.4.0/tests/data/jwst_image.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/mask.fits` & `stdatamodels-1.4.0/tests/data/mask.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/nircam_abvega_offset.asdf` & `stdatamodels-1.4.0/tests/data/nircam_abvega_offset.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/nonstandard_primary_array.schema.json` & `stdatamodels-1.4.0/tests/data/nonstandard_primary_array.schema.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/nonstandard_primary_array.schema.yaml` & `stdatamodels-1.4.0/tests/data/nonstandard_primary_array.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/sip.fits` & `stdatamodels-1.4.0/tests/data/sip.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/data/test.fits` & `stdatamodels-1.4.0/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/models.py` & `stdatamodels-1.4.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/schemas/basic_model.yaml` & `stdatamodels-1.4.0/tests/schemas/basic_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/schemas/deprecated_model.yaml` & `stdatamodels-1.4.0/tests/schemas/deprecated_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/schemas/fits_model.yaml` & `stdatamodels-1.4.0/tests/schemas/fits_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/schemas/table_model.yaml` & `stdatamodels-1.4.0/tests/schemas/table_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/schemas/validation_model.yaml` & `stdatamodels-1.4.0/tests/schemas/validation_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_asdf_in_fits.py` & `stdatamodels-1.4.0/tests/test_asdf_in_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_dq.py` & `stdatamodels-1.4.0/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_embedded_asdf.py` & `stdatamodels-1.4.0/tests/test_embedded_asdf.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_filetype.py` & `stdatamodels-1.4.0/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_fits.py` & `stdatamodels-1.4.0/tests/test_fits.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,23 +435,14 @@
 
     with fits.open(file_path, memmap=False) as hdulist:
         with FitsModel(hdulist) as dm:
             dm.data
         assert not hdulist.fileinfo(0)['file'].closed
 
 
-def test_open_fits_model_s3(s3_root_dir):
-    path = str(s3_root_dir.join("test.fits"))
-    with DataModel() as dm:
-        dm.save(path)
-
-    model = DataModel("s3://test-s3-data/test.fits")
-    assert isinstance(model, DataModel)
-
-
 def test_data_array(tmp_path):
     file_path = tmp_path/"test.fits"
     file_path2 = tmp_path/"test2.fits"
 
     data_array_schema = {
         "allOf": [
             asdf.schema.load_schema("http://example.com/schemas/core_metadata", resolve_references=True),
```

### Comparing `stdatamodels-1.3.1/tests/test_history.py` & `stdatamodels-1.4.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_models.py` & `stdatamodels-1.4.0/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,23 +168,14 @@
         af.write_to(file_path)
 
     with DataModel(file_path, ignore_version_mismatch=False, ignore_unrecognized_tag=True) as model:
         assert not model._asdf._ignore_version_mismatch
         assert model._asdf._ignore_unrecognized_tag
 
 
-def test_open_model_s3(s3_root_dir):
-    path = str(s3_root_dir.join("test.asdf"))
-    with DataModel() as dm:
-        dm.save(path)
-
-    model = DataModel("s3://test-s3-data/test.asdf")
-    assert isinstance(model, DataModel)
-
-
 def test_update_from_dict(tmp_path):
     """Test update method from a dictionary"""
     file_path = tmp_path/"update.asdf"
     with BasicModel((5, 5)) as m:
         m.update({"foo": "bar", "baz": 42})
         m.save(file_path)
```

### Comparing `stdatamodels-1.3.1/tests/test_resources.py` & `stdatamodels-1.4.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_schema.py` & `stdatamodels-1.4.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_util.py` & `stdatamodels-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tests/test_validation.py` & `stdatamodels-1.4.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.3.1/tox.ini` & `stdatamodels-1.4.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     CRDS_*
 extras =
     test
 deps =
     xdist: pytest-xdist
     cov: pytest-cov
     jwst: jwst[test] @ git+https://github.com/spacetelescope/jwst.git
+    jwst: stpipe @ git+https://github.com/spacetelescope/stpipe.git
 package=
     cov: editable
     !cov: wheel
 commands_pre =
     pip freeze
 commands =
     pytest \
```

