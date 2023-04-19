# Comparing `tmp/adsctl-0.1.0.tar.gz` & `tmp/adsctl-0.2.0.tar.gz`

## Comparing `adsctl-0.1.0.tar` & `adsctl-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,164 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/__about__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/prompt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/__init__.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/auth.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/cli.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/edit/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/edit/edit.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 adsctl-0.1.0/src/adsctl/cli/edit/campaign/budget.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 adsctl-0.1.0/tests/test_pkg.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 adsctl-0.1.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 adsctl-0.1.0/README.md
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 adsctl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 adsctl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.2.0/.DS_Store
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adsctl-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 adsctl-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.2.0/TESTING.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 adsctl-0.2.0/Taskfile.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/10a9dd0e5adddaf1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/11af71fc41104902
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/1300821ef2397b8d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/1be09cc27d42825f
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/1e390bbfc98b1261
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/22278fc9e9c974d5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/24388c23bc4581e1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/24acd61f3a44e711
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2ba7bbb13c6f1ff8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2e4287c1d42ae99c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2e4ce798cc3fd5c2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/2f05f6e2846725b8
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/32f05a3164dd0e5a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/338d67eba4c6bdff
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/37f0b12d8cc64a26
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/39f306ac02bb02fa
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/3bcf9dd6e88c27a8
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/41f825a5216815cb
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/420c14a4d8a7f822
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4691c6c53ef9d50d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4700a2e8f34df580
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/491adfbad040a642
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4c5b056d04e904b7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/4d6dfedc7028d85
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/506f573dae839856
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/50b72c98509d0f16
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5156a6d1dfdea5e8
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5174206c231b427
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/51d580e429e3c0f5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5485e4285df788f5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/54aac7aa945b4eea
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5d98ccd9a6b9e57a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5e6c26dd85411a59
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5eb2b7708bbab22a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/5ef45ad255bebe9e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/61324e2abd2c7394
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/6139ab745a83e112
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/634372ab84fcdbcb
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/644e31599b8e9334
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/6473c7264aba3c11
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/65f8915ba82563dd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/662c884e1aefe68d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/6e683bae26a97070
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/705ad6d5d08ac102
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/76e36826debb321d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7c353c43b7a6e871
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7c65e05ccd1c9bbb
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7c7f5cce4e0443cf
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7cfb88373125310
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7d23289c78f54ae7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7da3ad5bdc699672
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7e83f2c6e8c1dc3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/7efbe30ba86ed60b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/806660ee4170b006
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/8292eaab4ba08922
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/866b0f436c6ea144
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/86f500196eb4093e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/8b253cb47ea728f9
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/8e892b62735c3a22
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/909a15d3b4e8bcbe
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/90ca96135238d641
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/964e56fea98ed0c6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a020f1733d5f27cc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a05682a3f626f2e7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a0dc9ebbc118cbd2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a0f5216d10acefbc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a4f06cb80811dab6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a5299cf723a9da9e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/a7f2dbf98501bf26
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/aa77d19237682150
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/af875b2351696f9a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/afe656e26213792b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b23c85d45df72a6c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b5a6e95177cca536
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b6a151cd5537a666
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b7702dd98a1c8feb
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b8add4ae18edf8fe
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b8e51ba641007cd3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b8f20db2cdf13bf4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b9a17aed4565a2f5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b9a912145a8666c7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/b9bf929caeb8d5ff
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/bd8f2eb377cc390c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/bec3eace26d48273
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c2a7e3dbe51acec0
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c2ee9df2906b0aad
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c31a4240613aba4c
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c437a7deb9dca0d3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c4b9b21845be4e2a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c61e2bc2e3e68985
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/c7f894b3b4ff1101
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/cce24d291c5926a7
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/cffd6ef4b335e577
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/d57ff28381b694dc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/d6354cd37adec7f1
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/d8303c677b348538
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/db007523aa142218
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/dc9700eebaedaae0
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/df687802e9f41b67
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/e0049588e7dd3930
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/e48ea691d4c154c6
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/e96ac9b6b71a0fcc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ea412e3c1f88c72
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/eb207793d135be20
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ebf4a69dc4e4ce0b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ed35824412324ce
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ed553939ec479479
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/edc9e85377061c71
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/ee2280db6dd3b108
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/eebc50e7c61565df
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/eec97c7fbb7b4aac
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/f05e950057371d2
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/f71c91fb9f374a7f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/f83993ce009dfcc3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/fbb7edc21512479d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adsctl-0.2.0/.ruff_cache/content/fd7b9dc341c04ff5
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 adsctl-0.2.0/requirements/linting.in
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 adsctl-0.2.0/requirements/linting.txt
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 adsctl-0.2.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/__about__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/application.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/client.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/parse.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/queries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/budget.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/main.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/api/campaign/status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/__init__.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/auth.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/cli.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/config.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/edit/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/edit/campaign.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/cli/edit/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/config/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/config/config_file.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/config/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/prompt/__init__.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/prompt/cli.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/utils/__init__.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 adsctl-0.2.0/src/adsctl/utils/fs.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/test_parse.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.2.0/tests/test_pkg.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 adsctl-0.2.0/README.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 adsctl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 adsctl-0.2.0/PKG-INFO
```

### Comparing `adsctl-0.1.0/src/adsctl/cli/auth.py` & `adsctl-0.2.0/src/adsctl/cli/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-import argparse
 import hashlib
 import os
 import re
 import socket
 import sys
 from urllib.parse import unquote
 
 import click
-
-# If using Web flow, the redirect URL must match exactly what’s configured in GCP for
-# the OAuth client.  If using Desktop flow, the redirect must be a localhost URL and
-# is not explicitly set in GCP.
 from google_auth_oauthlib.flow import Flow
 
 _SCOPE = "https://www.googleapis.com/auth/adwords"
 _SERVER = "127.0.0.1"
 _PORT = 8080
 _REDIRECT_URI = f"http://{_SERVER}:{_PORT}"
 
 
 @click.command()
 @click.argument(
     "secrets_file",
     type=click.Path(exists=True),
 )
-def auth(secrets_file):
-    """Authenticate with Google Ads API.
+@click.pass_context
+def auth(ctx: click.Context, secrets_file):
+    """Authenticate with Google Ads API."""
+
+    # Do the OAuth flow to get a refresh token.
 
-    Args:
-        secrets_file: Path to the client secrets JSON file from the Google Developers Console that contains your client ID, client secret, and redirect URIs.
-    """
     configured_scopes = [_SCOPE]
 
     # if args.additional_scopes:
     #     configured_scopes.extend(args.additional_scopes)
 
     flow = Flow.from_client_secrets_file(secrets_file, scopes=configured_scopes)
     flow.redirect_uri = _REDIRECT_URI
@@ -61,20 +56,30 @@
     # redirect request and parsing the query parameters set in the URL.
     code = unquote(get_authorization_code(passthrough_val))
 
     # Pass the code back into the OAuth module to get a refresh token.
     flow.fetch_token(code=code)
     refresh_token = flow.credentials.refresh_token
 
-    print(f"\nYour refresh token is: {refresh_token}\n")
-    print(
-        "Add your refresh token to your client library configuration as "
-        "described here: "
-        "https://developers.google.com/google-ads/api/docs/client-libs/python/configuration"
-    )
+    click.echo(f"\nYour refresh token is: {refresh_token}\n")
+    click.echo("Updating config file to include refresh token")
+
+    with open(ctx.obj.config_file.path, "r") as f:
+        content = f.read()
+
+    with open(ctx.obj.config_file.path, "w") as f:
+        if "refresh_token" in content:
+            content = re.sub(
+                r"refresh_token = .*", f'refresh_token = "{refresh_token}"', content
+            )
+        else:
+            content = content + f'\nrefresh_token = "{refresh_token}"\n'
+        f.write(content)
+
+    click.echo("Done! You can now run adsctl commands.")
 
 
 def get_authorization_code(passthrough_val):
     """Opens a socket to handle a single HTTP request containing auth tokens.
     Args:
         passthrough_val: an anti-forgery token used to verify the request
           received by the socket.
@@ -129,13 +134,13 @@
         data: raw request data as bytes.
     Returns:
         a dict of query parameter key value pairs.
     """
     # Decode the request into a utf-8 encoded string
     decoded = data.decode("utf-8")
     # Use a regular expression to extract the URL query parameters string
-    match = re.search("GET\s\/\?(.*) ", decoded)
+    match = re.search("GET\\s\\/\\?(.*) ", decoded)
     params = match.group(1)
     # Split the parameters to isolate the key/value pairs
     pairs = [pair.split("=") for pair in params.split("&")]
     # Convert pairs to a dict to make it easy to access the values
-    return {key: val for key, val in pairs}
+    return dict(pairs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `adsctl-0.1.0/src/adsctl/cli/edit/campaign/budget.py` & `adsctl-0.2.0/src/adsctl/api/campaign/budget.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,40 @@
-import proto
-from google.api_core import protobuf_helpers
+from adsctl.api.utils import mask_operation
+from adsctl.application import Application
 
-from adsctl.cli import utils
 
+def get_rn(campaign_id, app: Application):
+    """Get the budget Resource Name for a campaign."""
 
-def mutate(client, customer_id, resource_name, budget):
-    """Set campaign budget."""
-
-    # Retrieve Object
     query = f"""
-    SELECT campaign_budget.amount_micros, campaign_budget.resource_name
-    FROM campaign_budget
-    WHERE campaign_budget.resource_name = "{resource_name}"
+        SELECT campaign.id, campaign.campaign_budget
+        FROM campaign
+        WHERE campaign.id = {campaign_id}
     """
 
-    response = utils.gaql_query(client, customer_id, query)
-    first = utils.get_first_row(response)
+    response = app.search(query)
+    for row in response:
+        return row.campaign.campaign_budget
+    return None
 
-    print(first)
 
-    if first is None:
-        print(f"Budget not found for campaign {resource_name}")
-        return None
-    initial = first.campaign_budget
+def mutate(budget, resource_name: str, app: Application):
+    """Set campaign budget."""
+    client = app.client
 
-    # Update Object
     campaign_budget_service = client.get_service("CampaignBudgetService")
     campaign_budget_operation = client.get_type("CampaignBudgetOperation")
 
     updated = campaign_budget_operation.update
     updated.resource_name = resource_name
 
     # Changes
     updated.amount_micros = int(budget * 1000000)
 
-    # Create a field mask using the updated campaign.
-    field_mask = protobuf_helpers.field_mask(None, updated._pb)
-    print(field_mask)
-    # Copy the field mask onto the operation's update_mask field.
-    client.copy_from(campaign_budget_operation.update_mask, field_mask)
+    # Boilerplate:
+    mask_operation(campaign_budget_operation, updated, client)
 
     response = campaign_budget_service.mutate_campaign_budgets(
-        customer_id=customer_id, operations=[campaign_budget_operation]
+        customer_id=app.customer_id, operations=[campaign_budget_operation]
     )
 
     return response
-
-
-def get_rn(client, customer_id, campaign_id):
-    """Get the budget ID for a campaign."""
-
-    query = f"""
-        SELECT campaign.id, campaign.campaign_budget
-        FROM campaign
-        WHERE campaign.id = {campaign_id}
-    """
-
-    response = utils.gaql_query(client, customer_id, query)
-    for row in response:
-        return row.campaign.campaign_budget
-    return None
```

### Comparing `adsctl-0.1.0/.gitignore` & `adsctl-0.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -154,7 +154,12 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# Project specific
+*.csv
+*.json
+*.sql
```

### Comparing `adsctl-0.1.0/LICENSE.txt` & `adsctl-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

