# Comparing `tmp/markdown2anki-0.1.2.tar.gz` & `tmp/markdown2anki-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown2anki-0.1.2.tar", last modified: Thu Mar 16 08:54:11 2023, max compression
+gzip compressed data, was "markdown2anki-0.2.0.tar", last modified: Wed Apr 19 18:33:09 2023, max compression
```

## Comparing `markdown2anki-0.1.2.tar` & `markdown2anki-0.2.0.tar`

### file list

```diff
@@ -1,228 +1,226 @@
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.069894 markdown2anki-0.1.2/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       71 2023-01-03 23:07:56.000000 markdown2anki-0.1.2/.gitattributes
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1786 2023-02-28 16:09:04.000000 markdown2anki-0.1.2/.gitignore
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      599 2023-03-16 08:51:56.000000 markdown2anki-0.1.2/CHANGELOG.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9623 2023-03-15 21:20:26.000000 markdown2anki-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    35150 2023-02-19 20:57:41.000000 markdown2anki-0.1.2/GPL3
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3678 2023-02-19 20:56:52.000000 markdown2anki-0.1.2/LICENSES
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      191 2023-02-09 21:33:05.000000 markdown2anki-0.1.2/Note_when_updating.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    28736 2023-03-16 08:54:11.069894 markdown2anki-0.1.2/PKG-INFO
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9667 2022-12-16 09:52:49.000000 markdown2anki-0.1.2/PYGMENTS_AUTHORS
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    23505 2023-03-16 08:23:00.000000 markdown2anki-0.1.2/README.md
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.969894 markdown2anki-0.1.2/docs/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    24636 2023-03-13 18:30:41.000000 markdown2anki-0.1.2/docs/Anki_import_example.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    78708 2023-03-16 06:59:21.000000 markdown2anki-0.1.2/docs/CLI_demo.mp4
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    15432 2023-03-15 19:27:47.000000 markdown2anki-0.1.2/docs/Demo-cloze-addon.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    15326 2023-03-15 19:27:07.000000 markdown2anki-0.1.2/docs/Demo-cloze-answer.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    27318 2023-03-15 19:27:49.000000 markdown2anki-0.1.2/docs/Demo-cloze-split-screen-addon.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    13292 2023-03-15 19:27:03.000000 markdown2anki-0.1.2/docs/Demo-cloze-standard.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    49062 2023-03-15 19:30:21.000000 markdown2anki-0.1.2/docs/Demo-split-screen.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    21832 2023-03-15 19:26:55.000000 markdown2anki-0.1.2/docs/Demo-update.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)   101017 2023-03-16 08:12:48.000000 markdown2anki-0.1.2/docs/Demo_highlight.gif
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)   401588 2023-03-16 06:52:14.000000 markdown2anki-0.1.2/docs/How_to_find_styling.mp4
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)   406601 2023-03-16 06:56:58.000000 markdown2anki-0.1.2/docs/How_to_make_type_in_cloze.mp4
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    86422 2023-03-15 19:32:33.000000 markdown2anki-0.1.2/docs/Main-demo_1.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    17432 2023-03-15 19:26:51.000000 markdown2anki-0.1.2/docs/Terminal-demo.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    14588 2023-03-13 12:04:21.000000 markdown2anki-0.1.2/docs/Usage_demo1.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)   103382 2023-03-13 12:04:14.000000 markdown2anki-0.1.2/docs/Usage_demo2.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    88960 2023-03-13 12:05:41.000000 markdown2anki-0.1.2/docs/Usage_demo3.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     7464 2023-03-16 07:30:24.000000 markdown2anki-0.1.2/docs/cloze_example.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    11916 2023-03-16 07:04:32.000000 markdown2anki-0.1.2/docs/light_mode_cloze.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    13686 2023-03-16 07:03:49.000000 markdown2anki-0.1.2/docs/mobile_cloze_demo.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    24060 2023-03-16 07:04:19.000000 markdown2anki-0.1.2/docs/mobile_demo.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    69238 2023-03-11 22:17:43.000000 markdown2anki-0.1.2/docs/rose-pine.webp
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.976560 markdown2anki-0.1.2/frontend/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      518 2023-03-11 21:23:00.000000 markdown2anki-0.1.2/frontend/build_theme_builder.js
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      523 2023-03-11 21:57:19.000000 markdown2anki-0.1.2/frontend/esbuild.js
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      698 2023-03-11 20:59:58.000000 markdown2anki-0.1.2/frontend/esbuild_themes.js
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      841 2023-03-11 12:53:18.000000 markdown2anki-0.1.2/frontend/esbuild_watch.js
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9018 2023-03-15 16:46:21.000000 markdown2anki-0.1.2/frontend/main_test.html
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    60492 2023-03-11 12:26:35.000000 markdown2anki-0.1.2/frontend/package-lock.json
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      702 2023-03-15 19:14:11.000000 markdown2anki-0.1.2/frontend/package.json
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.976560 markdown2anki-0.1.2/frontend/src/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3632 2023-03-10 20:59:56.000000 markdown2anki-0.1.2/frontend/src/main.ts
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.979894 markdown2anki-0.1.2/frontend/src/style/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.926560 markdown2anki-0.1.2/frontend/src/style/CSS Themes/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.983227 markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5845 2023-03-11 12:24:54.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_latte.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     6665 2023-03-11 12:25:20.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_macchiato.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5636 2023-03-11 12:25:20.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/rose_pine.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5633 2023-03-11 12:25:20.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/rose_pine_dawn.css
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.986560 markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      824 2023-03-15 16:22:54.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/catpuccin_latte.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      815 2023-03-15 16:22:14.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/catpuccin_macchiato.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      801 2023-03-15 16:16:11.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/rose_pine.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      788 2023-03-15 16:18:07.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/rose_pine_dawn.css
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.986560 markdown2anki-0.1.2/frontend/src/style/CSS Themes/full_themes/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      109 2023-03-11 12:10:47.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/full_themes/catpuccin_latte.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      117 2023-03-11 12:27:08.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/full_themes/catpuccin_macchiato.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       97 2023-03-11 12:27:34.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/full_themes/rose_pine.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      107 2023-03-11 12:28:00.000000 markdown2anki-0.1.2/frontend/src/style/CSS Themes/full_themes/rose_pine_dawn.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      225 2023-03-15 16:16:43.000000 markdown2anki-0.1.2/frontend/src/style/anki_specific.sass
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)      710 2023-03-15 16:21:05.000000 markdown2anki-0.1.2/frontend/src/style/base.sass
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)      388 2023-03-09 22:51:25.000000 markdown2anki-0.1.2/frontend/src/style/layout.sass
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)      346 2023-03-15 17:50:31.000000 markdown2anki-0.1.2/frontend/src/style/main.sass
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.926560 markdown2anki-0.1.2/frontend/src/style/modules/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.989894 markdown2anki-0.1.2/frontend/src/style/modules/highlight/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1340 2022-11-15 11:51:38.000000 markdown2anki-0.1.2/frontend/src/style/modules/highlight/README.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1338 2023-03-09 19:19:25.000000 markdown2anki-0.1.2/frontend/src/style/modules/highlight/highlight.sass
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.989894 markdown2anki-0.1.2/frontend/src/style/modules/tab/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1503 2023-03-11 20:56:15.000000 markdown2anki-0.1.2/frontend/src/style/modules/tab/README.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3565 2023-03-15 16:38:16.000000 markdown2anki-0.1.2/frontend/src/style/modules/tab/tab.sass
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.993227 markdown2anki-0.1.2/frontend/src/style/modules/tab_group/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      724 2023-03-11 20:57:49.000000 markdown2anki-0.1.2/frontend/src/style/modules/tab_group/README.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      575 2023-03-13 20:42:12.000000 markdown2anki-0.1.2/frontend/src/style/modules/tab_group/tab_group.sass
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      907 2023-03-11 21:03:47.000000 markdown2anki-0.1.2/frontend/src/style/themeless_main.sass
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.993227 markdown2anki-0.1.2/frontend/src/style/utilities/
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)       27 2022-11-06 00:19:42.000000 markdown2anki-0.1.2/frontend/src/style/utilities/general.sass
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)     1396 2023-03-09 23:17:17.000000 markdown2anki-0.1.2/frontend/src/style/utilities/normalize.sass
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    11298 2022-12-16 09:56:35.000000 markdown2anki-0.1.2/frontend/tsconfig.json
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1926 2023-03-16 08:49:54.000000 markdown2anki-0.1.2/pyproject.toml
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       38 2023-03-16 08:54:11.069894 markdown2anki-0.1.2/setup.cfg
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.929894 markdown2anki-0.1.2/src/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.996560 markdown2anki-0.1.2/src/markdown2anki/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3965 2023-03-16 08:48:19.000000 markdown2anki-0.1.2/src/markdown2anki/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.003227 markdown2anki-0.1.2/src/markdown2anki/config/
--rw-------   0 mochitto  (1000) mochitto  (1000)   144547 2023-03-15 18:12:48.000000 markdown2anki-0.1.2/src/markdown2anki/config/Markdown2Anki.apkg
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.006560 markdown2anki-0.1.2/src/markdown2anki/config/config_setup/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5336 2023-02-20 18:04:01.000000 markdown2anki-0.1.2/src/markdown2anki/config/config_setup/__init__.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1026 2023-02-20 18:04:01.000000 markdown2anki-0.1.2/src/markdown2anki/config/config_setup/casters.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1058 2023-02-20 18:04:01.000000 markdown2anki-0.1.2/src/markdown2anki/config/config_setup/validators.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5493 2023-03-16 08:48:19.000000 markdown2anki-0.1.2/src/markdown2anki/config/configs_handle.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4292 2023-03-15 18:31:57.000000 markdown2anki-0.1.2/src/markdown2anki/config/first_config.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4553 2023-03-15 18:16:58.000000 markdown2anki-0.1.2/src/markdown2anki/config/parse_args.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1572 2023-03-15 18:18:21.000000 markdown2anki-0.1.2/src/markdown2anki/config/welcome_message.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2244 2023-03-15 18:56:15.000000 markdown2anki-0.1.2/src/markdown2anki/logger.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.006560 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4922 2023-03-08 11:22:39.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.006560 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1986 2023-03-15 19:56:05.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.006560 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4710 2023-03-08 11:22:39.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.006560 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2490 2023-03-05 19:41:30.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_image_plugin.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2127 2023-03-01 17:52:55.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_link_plugin.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.009894 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/extract/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5340 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/extract/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.009894 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/format/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2279 2023-03-09 17:00:58.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/format/formatters.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      753 2023-03-10 19:29:23.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/format/wrappers.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.009894 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/swap/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3719 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/swap/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.009894 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_clozes/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4113 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_clozes/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.013227 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_images/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2288 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_images/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.013227 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      180 2023-02-20 18:03:59.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/__init__.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      419 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/card_error.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1207 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/card_types.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       77 2023-02-19 20:39:18.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/common_types.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1462 2023-02-19 20:39:18.000000 markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/debug_tools.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4122 2023-03-15 15:38:54.000000 markdown2anki-0.1.2/src/markdown2anki/output_handler.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3146 2023-02-09 21:26:00.000000 markdown2anki-0.1.2/src/markdown2anki/template for coding cards.md
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.016560 markdown2anki-0.1.2/src/markdown2anki/utils/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       77 2023-02-19 20:39:18.000000 markdown2anki-0.1.2/src/markdown2anki/utils/common_types.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1462 2023-02-19 20:39:18.000000 markdown2anki-0.1.2/src/markdown2anki/utils/debug_tools.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      888 2023-03-15 17:46:31.000000 markdown2anki-0.1.2/src/markdown2anki/version_check.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.999894 markdown2anki-0.1.2/src/markdown2anki.egg-info/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    28736 2023-03-16 08:54:10.000000 markdown2anki-0.1.2/src/markdown2anki.egg-info/PKG-INFO
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     7027 2023-03-16 08:54:10.000000 markdown2anki-0.1.2/src/markdown2anki.egg-info/SOURCES.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)        1 2023-03-16 08:54:10.000000 markdown2anki-0.1.2/src/markdown2anki.egg-info/dependency_links.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       47 2023-03-16 08:54:10.000000 markdown2anki-0.1.2/src/markdown2anki.egg-info/entry_points.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       88 2023-03-16 08:54:10.000000 markdown2anki-0.1.2/src/markdown2anki.egg-info/requires.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       14 2023-03-16 08:54:10.000000 markdown2anki-0.1.2/src/markdown2anki.egg-info/top_level.txt
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.016560 markdown2anki-0.1.2/tests/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      257 2023-03-11 20:37:23.000000 markdown2anki-0.1.2/tests/__init__.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.019894 markdown2anki-0.1.2/tests/assets/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.019894 markdown2anki-0.1.2/tests/assets/images/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)   156474 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/2010.jpg
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.023227 markdown2anki-0.1.2/tests/assets/images/MORE/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    79730 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/MORE/Toing.jpg
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.026560 markdown2anki-0.1.2/tests/assets/images/MORE/YES_ME/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    25718 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/MORE/YES_ME/FroW.jpeg
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    95025 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/MORE/YES_ME/i_am_a_forest_fire.jpeg
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.026560 markdown2anki-0.1.2/tests/assets/images/MORE/exclude_me_too/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    66601 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/MORE/exclude_me_too/mmmm.jpg
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    35747 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/MORE/oiter.jpg
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    16241 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/MORE/vruM.jpg
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    25136 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/WAAAA.jpeg
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.029894 markdown2anki-0.1.2/tests/assets/images/exclude_me/
--rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    44099 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/assets/images/exclude_me/fkboi.jpeg
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)        0 2023-02-25 21:27:05.000000 markdown2anki-0.1.2/tests/assets/input.md
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.029894 markdown2anki-0.1.2/tests/assets/inputs/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)        4 2023-02-27 20:40:47.000000 markdown2anki-0.1.2/tests/assets/inputs/welcome_user_exit1.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       50 2023-02-27 20:40:47.000000 markdown2anki-0.1.2/tests/assets/inputs/welcome_user_exit2.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)       47 2023-02-27 20:40:47.000000 markdown2anki-0.1.2/tests/assets/inputs/welcome_user_good.txt
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      489 2023-02-28 18:37:09.000000 markdown2anki-0.1.2/tests/conftest.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.939894 markdown2anki-0.1.2/tests/integration/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.033227 markdown2anki-0.1.2/tests/integration/config/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     8828 2023-03-02 21:36:57.000000 markdown2anki-0.1.2/tests/integration/config/test_handle_configs.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3049 2023-02-28 10:04:25.000000 markdown2anki-0.1.2/tests/integration/config/test_welcome_user.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.939894 markdown2anki-0.1.2/tests/integration/md_2_anki/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.033227 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.033227 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/extract/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2154 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/extract/test_extract_tab.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.036560 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/format/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2300 2023-03-11 20:33:37.000000 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/format/test_formatting.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.036560 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/swap/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3224 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/swap/test_get_swapped_card.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2176 2023-03-11 20:31:29.000000 markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/test_process_card.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.036560 markdown2anki-0.1.2/tests/integration/md_2_anki/process_clozes/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2428 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/integration/md_2_anki/process_clozes/test_clozes_processing.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.036560 markdown2anki-0.1.2/tests/integration/md_2_anki/process_images/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2157 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/integration/md_2_anki/process_images/test_process_images.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.039894 markdown2anki-0.1.2/tests/setup/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2734 2023-03-06 21:43:40.000000 markdown2anki-0.1.2/tests/setup/__init__.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1243 2023-03-05 19:40:58.000000 markdown2anki-0.1.2/tests/setup/config_file_patch.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.943227 markdown2anki-0.1.2/tests/unit_tests/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.039894 markdown2anki-0.1.2/tests/unit_tests/config/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1369 2023-02-28 16:35:46.000000 markdown2anki-0.1.2/tests/unit_tests/config/test_configs_handle.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      995 2023-02-28 10:04:25.000000 markdown2anki-0.1.2/tests/unit_tests/config/test_first_config.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2003 2023-02-28 18:27:12.000000 markdown2anki-0.1.2/tests/unit_tests/config/test_setup_typeConfig.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.943227 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:10.943227 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.043227 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/compile/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2774 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_image_plugin.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1875 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_wikilink_plugin.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.046561 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      800 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_extract_cards.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2882 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_bodies.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      849 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_labels.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1052 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_parse_flags.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1706 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_parse_tab_label.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.046561 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/format/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1899 2023-03-11 20:35:35.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/format/test_format_tab.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4231 2023-03-05 19:40:58.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/format/test_format_tab_group.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.049894 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9562 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/test_create_back_tabs_list.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4248 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/test_create_front_tabs_list.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3817 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/test_get_swap_mappings.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.053227 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      685 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_are_clozes_in_card.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1083 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_clean_code_from_clozes.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      832 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_get_clozes.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1995 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_hash_clozes.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1819 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_replace_cloze_text_with_hashes.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.056561 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_images/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1988 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_images/test_find_image_path.py
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1124 2023-03-06 21:57:48.000000 markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_images/test_get_images_sources.py
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.056561 markdown2anki-0.1.2/theme_builder/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5671 2023-03-11 22:13:35.000000 markdown2anki-0.1.2/theme_builder/README.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1934 2023-03-15 17:50:49.000000 markdown2anki-0.1.2/theme_builder/main.js
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.059894 markdown2anki-0.1.2/theme_builder/style/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5051 2023-03-11 21:16:16.000000 markdown2anki-0.1.2/theme_builder/style/Hightlight_theme_template.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1248 2023-03-15 16:25:29.000000 markdown2anki-0.1.2/theme_builder/style/UI_theme_template.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     6032 2023-03-15 17:50:49.000000 markdown2anki-0.1.2/theme_builder/style/themeless_main.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9172 2023-03-15 16:46:36.000000 markdown2anki-0.1.2/theme_builder/test.html
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.063227 markdown2anki-0.1.2/themes/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)      798 2023-03-11 22:25:35.000000 markdown2anki-0.1.2/themes/README.md
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3509 2023-03-15 17:50:47.000000 markdown2anki-0.1.2/themes/catpuccin_latte.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4378 2023-03-15 17:50:46.000000 markdown2anki-0.1.2/themes/catpuccin_macchiato.css
-drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-03-16 08:54:11.066561 markdown2anki-0.1.2/themes/docs/
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    65108 2023-03-11 22:17:07.000000 markdown2anki-0.1.2/themes/docs/catpuccin-latte.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    72610 2023-03-11 22:17:05.000000 markdown2anki-0.1.2/themes/docs/catpuccin-macchiato.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    67610 2023-03-11 22:17:40.000000 markdown2anki-0.1.2/themes/docs/rose-pine-dawn.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)    69238 2023-03-11 22:17:43.000000 markdown2anki-0.1.2/themes/docs/rose-pine.webp
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3259 2023-03-15 17:50:46.000000 markdown2anki-0.1.2/themes/rose_pine.css
--rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3243 2023-03-15 17:50:46.000000 markdown2anki-0.1.2/themes/rose_pine_dawn.css
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.871019 markdown2anki-0.2.0/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       71 2023-01-03 23:07:56.000000 markdown2anki-0.2.0/.gitattributes
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1786 2023-02-28 16:09:04.000000 markdown2anki-0.2.0/.gitignore
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      997 2023-04-19 18:30:34.000000 markdown2anki-0.2.0/CHANGELOG.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9623 2023-03-15 21:20:26.000000 markdown2anki-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    35150 2023-02-19 20:57:41.000000 markdown2anki-0.2.0/GPL3
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3678 2023-02-19 20:56:52.000000 markdown2anki-0.2.0/LICENSES
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    28609 2023-04-19 18:33:09.867686 markdown2anki-0.2.0/PKG-INFO
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9667 2022-12-16 09:52:49.000000 markdown2anki-0.2.0/PYGMENTS_AUTHORS
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    23378 2023-04-19 18:08:46.000000 markdown2anki-0.2.0/README.md
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.794352 markdown2anki-0.2.0/docs/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    24636 2023-03-13 18:30:41.000000 markdown2anki-0.2.0/docs/Anki_import_example.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    78708 2023-03-16 06:59:21.000000 markdown2anki-0.2.0/docs/CLI_demo.mp4
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    15432 2023-03-15 19:27:47.000000 markdown2anki-0.2.0/docs/Demo-cloze-addon.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    15326 2023-03-15 19:27:07.000000 markdown2anki-0.2.0/docs/Demo-cloze-answer.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    27318 2023-03-15 19:27:49.000000 markdown2anki-0.2.0/docs/Demo-cloze-split-screen-addon.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    13292 2023-03-15 19:27:03.000000 markdown2anki-0.2.0/docs/Demo-cloze-standard.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    49062 2023-03-15 19:30:21.000000 markdown2anki-0.2.0/docs/Demo-split-screen.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    21832 2023-03-15 19:26:55.000000 markdown2anki-0.2.0/docs/Demo-update.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)   101017 2023-03-16 08:12:48.000000 markdown2anki-0.2.0/docs/Demo_highlight.gif
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)   401588 2023-03-16 06:52:14.000000 markdown2anki-0.2.0/docs/How_to_find_styling.mp4
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)   406601 2023-03-16 06:56:58.000000 markdown2anki-0.2.0/docs/How_to_make_type_in_cloze.mp4
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    86422 2023-03-15 19:32:33.000000 markdown2anki-0.2.0/docs/Main-demo_1.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    17432 2023-03-15 19:26:51.000000 markdown2anki-0.2.0/docs/Terminal-demo.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    14588 2023-03-13 12:04:21.000000 markdown2anki-0.2.0/docs/Usage_demo1.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)   103382 2023-03-13 12:04:14.000000 markdown2anki-0.2.0/docs/Usage_demo2.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    88960 2023-03-13 12:05:41.000000 markdown2anki-0.2.0/docs/Usage_demo3.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     7464 2023-03-16 07:30:24.000000 markdown2anki-0.2.0/docs/cloze_example.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    11916 2023-03-16 07:04:32.000000 markdown2anki-0.2.0/docs/light_mode_cloze.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    13686 2023-03-16 07:03:49.000000 markdown2anki-0.2.0/docs/mobile_cloze_demo.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    24060 2023-03-16 07:04:19.000000 markdown2anki-0.2.0/docs/mobile_demo.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    69238 2023-03-11 22:17:43.000000 markdown2anki-0.2.0/docs/rose-pine.webp
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.797686 markdown2anki-0.2.0/frontend/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      518 2023-03-11 21:23:00.000000 markdown2anki-0.2.0/frontend/build_theme_builder.js
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      523 2023-03-11 21:57:19.000000 markdown2anki-0.2.0/frontend/esbuild.js
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      698 2023-03-11 20:59:58.000000 markdown2anki-0.2.0/frontend/esbuild_themes.js
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      841 2023-03-11 12:53:18.000000 markdown2anki-0.2.0/frontend/esbuild_watch.js
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9018 2023-03-15 16:46:21.000000 markdown2anki-0.2.0/frontend/main_test.html
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    60492 2023-03-11 12:26:35.000000 markdown2anki-0.2.0/frontend/package-lock.json
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      702 2023-03-15 19:14:11.000000 markdown2anki-0.2.0/frontend/package.json
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.797686 markdown2anki-0.2.0/frontend/src/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3632 2023-03-10 20:59:56.000000 markdown2anki-0.2.0/frontend/src/main.ts
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.801019 markdown2anki-0.2.0/frontend/src/style/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.757686 markdown2anki-0.2.0/frontend/src/style/CSS Themes/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.804352 markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5845 2023-03-11 12:24:54.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_latte.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     6665 2023-03-11 12:25:20.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_macchiato.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5636 2023-03-11 12:25:20.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/rose_pine.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5633 2023-03-11 12:25:20.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/rose_pine_dawn.css
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.807686 markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      824 2023-03-15 16:22:54.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/catpuccin_latte.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      815 2023-03-15 16:22:14.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/catpuccin_macchiato.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      801 2023-03-15 16:16:11.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/rose_pine.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      788 2023-03-15 16:18:07.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/rose_pine_dawn.css
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.811019 markdown2anki-0.2.0/frontend/src/style/CSS Themes/full_themes/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      109 2023-03-11 12:10:47.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/full_themes/catpuccin_latte.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      117 2023-03-11 12:27:08.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/full_themes/catpuccin_macchiato.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       97 2023-03-11 12:27:34.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/full_themes/rose_pine.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      107 2023-03-11 12:28:00.000000 markdown2anki-0.2.0/frontend/src/style/CSS Themes/full_themes/rose_pine_dawn.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      225 2023-03-15 16:16:43.000000 markdown2anki-0.2.0/frontend/src/style/anki_specific.sass
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)      710 2023-03-15 16:21:05.000000 markdown2anki-0.2.0/frontend/src/style/base.sass
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)      388 2023-03-09 22:51:25.000000 markdown2anki-0.2.0/frontend/src/style/layout.sass
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)      346 2023-03-15 17:50:31.000000 markdown2anki-0.2.0/frontend/src/style/main.sass
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.757686 markdown2anki-0.2.0/frontend/src/style/modules/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.811019 markdown2anki-0.2.0/frontend/src/style/modules/highlight/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1340 2022-11-15 11:51:38.000000 markdown2anki-0.2.0/frontend/src/style/modules/highlight/README.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1338 2023-03-09 19:19:25.000000 markdown2anki-0.2.0/frontend/src/style/modules/highlight/highlight.sass
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.814352 markdown2anki-0.2.0/frontend/src/style/modules/tab/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1503 2023-03-11 20:56:15.000000 markdown2anki-0.2.0/frontend/src/style/modules/tab/README.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3565 2023-03-15 16:38:16.000000 markdown2anki-0.2.0/frontend/src/style/modules/tab/tab.sass
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.814352 markdown2anki-0.2.0/frontend/src/style/modules/tab_group/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      724 2023-03-11 20:57:49.000000 markdown2anki-0.2.0/frontend/src/style/modules/tab_group/README.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      575 2023-03-13 20:42:12.000000 markdown2anki-0.2.0/frontend/src/style/modules/tab_group/tab_group.sass
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      907 2023-03-11 21:03:47.000000 markdown2anki-0.2.0/frontend/src/style/themeless_main.sass
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.814352 markdown2anki-0.2.0/frontend/src/style/utilities/
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)       27 2022-11-06 00:19:42.000000 markdown2anki-0.2.0/frontend/src/style/utilities/general.sass
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)     1396 2023-03-09 23:17:17.000000 markdown2anki-0.2.0/frontend/src/style/utilities/normalize.sass
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    11298 2022-12-16 09:56:35.000000 markdown2anki-0.2.0/frontend/tsconfig.json
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1926 2023-04-19 18:23:22.000000 markdown2anki-0.2.0/pyproject.toml
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       38 2023-04-19 18:33:09.871019 markdown2anki-0.2.0/setup.cfg
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.761019 markdown2anki-0.2.0/src/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.817686 markdown2anki-0.2.0/src/markdown2anki/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4091 2023-04-19 18:16:08.000000 markdown2anki-0.2.0/src/markdown2anki/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.824352 markdown2anki-0.2.0/src/markdown2anki/config/
+-rw-------   0 mochitto  (1000) mochitto  (1000)   144547 2023-03-15 18:12:48.000000 markdown2anki-0.2.0/src/markdown2anki/config/Markdown2Anki.apkg
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.827686 markdown2anki-0.2.0/src/markdown2anki/config/config_setup/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5362 2023-04-19 18:20:24.000000 markdown2anki-0.2.0/src/markdown2anki/config/config_setup/__init__.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1026 2023-02-20 18:04:01.000000 markdown2anki-0.2.0/src/markdown2anki/config/config_setup/casters.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1058 2023-02-20 18:04:01.000000 markdown2anki-0.2.0/src/markdown2anki/config/config_setup/validators.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5493 2023-03-16 08:48:19.000000 markdown2anki-0.2.0/src/markdown2anki/config/configs_handle.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4292 2023-03-15 18:31:57.000000 markdown2anki-0.2.0/src/markdown2anki/config/first_config.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4553 2023-03-15 18:16:58.000000 markdown2anki-0.2.0/src/markdown2anki/config/parse_args.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1572 2023-03-15 18:18:21.000000 markdown2anki-0.2.0/src/markdown2anki/config/welcome_message.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2244 2023-03-15 18:56:15.000000 markdown2anki-0.2.0/src/markdown2anki/logger.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.827686 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4435 2023-04-19 17:25:04.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.827686 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1986 2023-03-15 19:56:05.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.827686 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4710 2023-03-08 11:22:39.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.827686 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2490 2023-03-05 19:41:30.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_image_plugin.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2127 2023-03-01 17:52:55.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_link_plugin.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.831019 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/extract/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5340 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/extract/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.831019 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/format/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2279 2023-03-09 17:00:58.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/format/formatters.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      753 2023-03-10 19:29:23.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/format/wrappers.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.831019 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/swap/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3719 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/swap/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.831019 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_clozes/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4153 2023-04-19 17:36:55.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_clozes/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.831019 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_images/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2288 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_images/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.834352 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      180 2023-02-20 18:03:59.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/__init__.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      419 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/card_error.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1207 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/card_types.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       77 2023-02-19 20:39:18.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/common_types.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1462 2023-02-19 20:39:18.000000 markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/debug_tools.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4158 2023-04-19 18:29:01.000000 markdown2anki-0.2.0/src/markdown2anki/output_handler.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3146 2023-02-09 21:26:00.000000 markdown2anki-0.2.0/src/markdown2anki/template for coding cards.md
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.834352 markdown2anki-0.2.0/src/markdown2anki/utils/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       77 2023-02-19 20:39:18.000000 markdown2anki-0.2.0/src/markdown2anki/utils/common_types.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1462 2023-02-19 20:39:18.000000 markdown2anki-0.2.0/src/markdown2anki/utils/debug_tools.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      888 2023-04-19 18:16:50.000000 markdown2anki-0.2.0/src/markdown2anki/version_check.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.821019 markdown2anki-0.2.0/src/markdown2anki.egg-info/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    28609 2023-04-19 18:33:09.000000 markdown2anki-0.2.0/src/markdown2anki.egg-info/PKG-INFO
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     6927 2023-04-19 18:33:09.000000 markdown2anki-0.2.0/src/markdown2anki.egg-info/SOURCES.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)        1 2023-04-19 18:33:09.000000 markdown2anki-0.2.0/src/markdown2anki.egg-info/dependency_links.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       47 2023-04-19 18:33:09.000000 markdown2anki-0.2.0/src/markdown2anki.egg-info/entry_points.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       88 2023-04-19 18:33:09.000000 markdown2anki-0.2.0/src/markdown2anki.egg-info/requires.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       14 2023-04-19 18:33:09.000000 markdown2anki-0.2.0/src/markdown2anki.egg-info/top_level.txt
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.834352 markdown2anki-0.2.0/tests/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      257 2023-03-11 20:37:23.000000 markdown2anki-0.2.0/tests/__init__.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.837686 markdown2anki-0.2.0/tests/assets/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.837686 markdown2anki-0.2.0/tests/assets/images/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)   156474 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/2010.jpg
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.841019 markdown2anki-0.2.0/tests/assets/images/MORE/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    79730 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/MORE/Toing.jpg
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.841019 markdown2anki-0.2.0/tests/assets/images/MORE/YES_ME/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    25718 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/MORE/YES_ME/FroW.jpeg
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    95025 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/MORE/YES_ME/i_am_a_forest_fire.jpeg
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.841019 markdown2anki-0.2.0/tests/assets/images/MORE/exclude_me_too/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    66601 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/MORE/exclude_me_too/mmmm.jpg
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    35747 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/MORE/oiter.jpg
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    16241 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/MORE/vruM.jpg
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    25136 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/WAAAA.jpeg
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.841019 markdown2anki-0.2.0/tests/assets/images/exclude_me/
+-rwxr-xr-x   0 mochitto  (1000) mochitto  (1000)    44099 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/assets/images/exclude_me/fkboi.jpeg
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)        0 2023-02-25 21:27:05.000000 markdown2anki-0.2.0/tests/assets/input.md
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.844352 markdown2anki-0.2.0/tests/assets/inputs/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)        4 2023-02-27 20:40:47.000000 markdown2anki-0.2.0/tests/assets/inputs/welcome_user_exit1.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       50 2023-02-27 20:40:47.000000 markdown2anki-0.2.0/tests/assets/inputs/welcome_user_exit2.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)       47 2023-02-27 20:40:47.000000 markdown2anki-0.2.0/tests/assets/inputs/welcome_user_good.txt
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      489 2023-02-28 18:37:09.000000 markdown2anki-0.2.0/tests/conftest.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.767686 markdown2anki-0.2.0/tests/integration/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.844352 markdown2anki-0.2.0/tests/integration/config/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     8828 2023-03-02 21:36:57.000000 markdown2anki-0.2.0/tests/integration/config/test_handle_configs.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3049 2023-02-28 10:04:25.000000 markdown2anki-0.2.0/tests/integration/config/test_welcome_user.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.771019 markdown2anki-0.2.0/tests/integration/md_2_anki/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.844352 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.844352 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/extract/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2154 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/extract/test_extract_tab.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.844352 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/format/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2300 2023-03-11 20:33:37.000000 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/format/test_formatting.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.847686 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/swap/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3224 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/swap/test_get_swapped_card.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2176 2023-03-11 20:31:29.000000 markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/test_process_card.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.847686 markdown2anki-0.2.0/tests/integration/md_2_anki/process_clozes/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2683 2023-04-19 17:54:45.000000 markdown2anki-0.2.0/tests/integration/md_2_anki/process_clozes/test_clozes_processing.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.847686 markdown2anki-0.2.0/tests/integration/md_2_anki/process_images/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2157 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/integration/md_2_anki/process_images/test_process_images.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.847686 markdown2anki-0.2.0/tests/setup/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2734 2023-03-06 21:43:40.000000 markdown2anki-0.2.0/tests/setup/__init__.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1243 2023-03-05 19:40:58.000000 markdown2anki-0.2.0/tests/setup/config_file_patch.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.771019 markdown2anki-0.2.0/tests/unit_tests/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.851019 markdown2anki-0.2.0/tests/unit_tests/config/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1369 2023-02-28 16:35:46.000000 markdown2anki-0.2.0/tests/unit_tests/config/test_configs_handle.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      995 2023-02-28 10:04:25.000000 markdown2anki-0.2.0/tests/unit_tests/config/test_first_config.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2003 2023-02-28 18:27:12.000000 markdown2anki-0.2.0/tests/unit_tests/config/test_setup_typeConfig.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.774352 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.771019 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.851019 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/compile/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2774 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_image_plugin.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1875 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_wikilink_plugin.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.854352 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      800 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_extract_cards.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2882 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_bodies.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      849 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_labels.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1052 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_parse_flags.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1706 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_parse_tab_label.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.854352 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/format/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1899 2023-03-11 20:35:35.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/format/test_format_tab.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4231 2023-03-05 19:40:58.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/format/test_format_tab_group.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.854352 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9562 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/test_create_back_tabs_list.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4248 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/test_create_front_tabs_list.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3817 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/test_get_swap_mappings.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.857686 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      685 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_are_clozes_in_card.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      960 2023-04-19 17:36:58.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_get_clozes.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     2008 2023-04-19 17:36:57.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_hash_clozes.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1852 2023-04-19 17:41:37.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_replace_clozes_with_hashes.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.857686 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_images/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1988 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_images/test_find_image_path.py
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1124 2023-03-06 21:57:48.000000 markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_images/test_get_images_sources.py
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.861019 markdown2anki-0.2.0/theme_builder/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5671 2023-03-11 22:13:35.000000 markdown2anki-0.2.0/theme_builder/README.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1934 2023-03-15 17:50:49.000000 markdown2anki-0.2.0/theme_builder/main.js
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.861019 markdown2anki-0.2.0/theme_builder/style/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     5051 2023-03-11 21:16:16.000000 markdown2anki-0.2.0/theme_builder/style/Hightlight_theme_template.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     1248 2023-03-15 16:25:29.000000 markdown2anki-0.2.0/theme_builder/style/UI_theme_template.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     6032 2023-03-15 17:50:49.000000 markdown2anki-0.2.0/theme_builder/style/themeless_main.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     9172 2023-03-15 16:46:36.000000 markdown2anki-0.2.0/theme_builder/test.html
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.864352 markdown2anki-0.2.0/themes/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)      798 2023-03-11 22:25:35.000000 markdown2anki-0.2.0/themes/README.md
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3509 2023-03-15 17:50:47.000000 markdown2anki-0.2.0/themes/catpuccin_latte.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     4378 2023-03-15 17:50:46.000000 markdown2anki-0.2.0/themes/catpuccin_macchiato.css
+drwxr-xr-x   0 mochitto  (1000) mochitto  (1000)        0 2023-04-19 18:33:09.867686 markdown2anki-0.2.0/themes/docs/
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    65108 2023-03-11 22:17:07.000000 markdown2anki-0.2.0/themes/docs/catpuccin-latte.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    72610 2023-03-11 22:17:05.000000 markdown2anki-0.2.0/themes/docs/catpuccin-macchiato.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    67610 2023-03-11 22:17:40.000000 markdown2anki-0.2.0/themes/docs/rose-pine-dawn.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)    69238 2023-03-11 22:17:43.000000 markdown2anki-0.2.0/themes/docs/rose-pine.webp
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3259 2023-03-15 17:50:46.000000 markdown2anki-0.2.0/themes/rose_pine.css
+-rw-r--r--   0 mochitto  (1000) mochitto  (1000)     3243 2023-03-15 17:50:46.000000 markdown2anki-0.2.0/themes/rose_pine_dawn.css
```

### Comparing `markdown2anki-0.1.2/.gitignore` & `markdown2anki-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/CHANGELOG.md` & `markdown2anki-0.2.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## [Unreleased]
 
+## [0.2.0] - 2023-04-19
+
+### Fixed
+- Fixed bugs regarding cloze deletion handling.
+- You can leave the "Obsidian vault name" empty now.
+
+### Added
+- Added a message letting you know the app is checking for when starting updates.
+
+### Changed
+- Bad cards are now appended to the "bad cards.md" file instead of overwriting the file. This way you don't have to fix them before running other imports.
+
 ## [0.1.2] - 2023-03-16
 
 ### Fixed
 - Updated dependency to Type-config, which was left to an earlier version in the `pyproject.toml`
 
 ## [0.1.1] - 2023-03-16
```

### Comparing `markdown2anki-0.1.2/CONTRIBUTING.md` & `markdown2anki-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/GPL3` & `markdown2anki-0.2.0/GPL3`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/LICENSES` & `markdown2anki-0.2.0/LICENSES`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/PKG-INFO` & `markdown2anki-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown2anki
-Version: 0.1.2
+Version: 0.2.0
 Summary: A CLI tool and an apkg template to allow you to create flashcards from markdown and have a better experience while using anki for your studies. 🌸
 Author-email: "Alex Biosa (mochitto)" <mochittodeveloper@gmail.com>
 License: Copyright (C) 2023, Alex Biosa (mochitto), mochittodeveloper@gmail.com 
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
@@ -148,15 +148,15 @@
 - **Mobile first responsive CSS**: to ensure it's fully responsive on all devices.
 - **High-level dev documentation** to make it easier for contributions and maintenance.
 
 ## Images
 
 ### CLI
 ![Demo image of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Terminal-demo.webp)  
-![Video demo of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/CLI_demo.mp4)
+[Video demo of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/CLI_demo.mp4)
 ### Split-screen
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-split-screen.webp) 
 ### Code highlighting
 ![Demo code highlighting](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo_highlight.gif)
 ### Clozes support
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-standard.webp) 
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-answer.webp) 
@@ -214,15 +214,15 @@
 You can learn more on `.apkg` files here: https://docs.ankiweb.net/exporting.html#deck-apkg
 
 ### Using fill the blanks
 
 If you would like to have "type-in" clozes, you can use this addon: [fill the blanks addon](https://ankiweb.net/shared/info/1933645497).  
 For it to work, you will need to duplicate the `Markdown2Anki - Cloze` Note type and modify it by changing the `Front side` field to: `{{type:cloze:Front}}`.  
 
-This is a video with how you can achieve this: ![Video Tutorial on how to modify a note type](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/How_to_make_type_in_cloze.mp4)
+This is a video with how you can achieve this: [Video Tutorial on how to modify a note type](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/How_to_make_type_in_cloze.mp4)
 
 ![Demo of fill the blanks](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-addon.webp)
 
 ## Usage
 
 ### Markdown input formatting
 To ensure that your notes are properly recognized by the program, there are a few formatting requirements:
@@ -367,22 +367,20 @@
 A `debug_log.txt` file is also present in your program folder, which is created every time you run the program. This file contains more information on what happens when the program is running, the result of various processes, your configuration and so on.  
 If you find a bug in the program, it would be of great help if you could add this file to your issues on GitHub.  
 
 **Privacy Notice:** the log file has your configuration in it, as it can contain crucial information for debugging.  
 If you don't want to share your paths or other information from it when making issues, you should search-and-replace that information with some fake one, while trying not to change their general structure.
 
 ### Using clozes
-You can specify clozes in your markdown and they will be carried over to your anki cards. Whenever there is a word or sentence you'd like to have as a cloze, you can use Anki's formatting `{{c<number>::<word>}}` (notice the two colons, not just one).
+You can specify clozes in your markdown and they will be carried over to your anki cards. Whenever there is a word or sentence you'd like to have as a cloze, you can use Anki's formatting `{{c<number>::<word>::<hint?>}}` (notice the two colons, not just one).
+Clozes will also work in code blocks.
 
 The number tells Anki what cloze to add to what card. This means that if you have C1, C2 and C3, there will be three cards created (this is a feature of Anki, not of Markdown2Anki), each missing the respective words.  
 More on this here: https://docs.ankiweb.net/editing.html#cloze-deletion
 
-If the clozed word/sentence is present multiple times, it will be automatically turned into a cloze, so you only need to specify it once.
-This works also in code blocks.
-
 For example:
 ```python
 my_list = [3,5,2]
 # New list
 sorted_list = {{C1::sorted}}(my_list, {{C1::True}}) 
 # In place
 my_list.{{C1::sort}}(True)
@@ -393,15 +391,15 @@
 
 ### Changing Themes
 The default theme is mochitto's Rosé Pine theme, but there is also a catpuccin theme.  
 You can find all the themes in the [themes folder](https://github.com/Mochitto/Markdown2Anki/tree/master/themes).  
 To use another theme, you can just copy the CSS from the file in the themes folder and paste it in your Note types' styling field.  
 
 This can be found by accessing `Tools>Manage Note Types>(select your note type)>Cards(on the right)>Styling(on the left)`. The `Tools` menu is found in the top-left part of Anki's main menu.   
-You can reference this: ![Video Tutorial showing how to access a card's style](https://github.com/Mochitto/Markdown2Anki/blob/master/docs/How_to_find_styling.mp4)
+You can reference this: [Video Tutorial showing how to access a card's style](https://github.com/Mochitto/Markdown2Anki/blob/master/docs/How_to_find_styling.mp4)
 
 You can read more on how styling happens here: https://docs.ankiweb.net/templates/styling.html
 
 ### Navigating the UI
 The custom User Interface of the note-type that comes with this project is focused on the concept of tabs.  
 You can have side-by-side tabs and multiple tabs to toggle through.
```

### Comparing `markdown2anki-0.1.2/PYGMENTS_AUTHORS` & `markdown2anki-0.2.0/PYGMENTS_AUTHORS`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/README.md` & `markdown2anki-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 - **Mobile first responsive CSS**: to ensure it's fully responsive on all devices.
 - **High-level dev documentation** to make it easier for contributions and maintenance.
 
 ## Images
 
 ### CLI
 ![Demo image of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Terminal-demo.webp)  
-![Video demo of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/CLI_demo.mp4)
+[Video demo of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/CLI_demo.mp4)
 ### Split-screen
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-split-screen.webp) 
 ### Code highlighting
 ![Demo code highlighting](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo_highlight.gif)
 ### Clozes support
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-standard.webp) 
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-answer.webp) 
@@ -131,15 +131,15 @@
 You can learn more on `.apkg` files here: https://docs.ankiweb.net/exporting.html#deck-apkg
 
 ### Using fill the blanks
 
 If you would like to have "type-in" clozes, you can use this addon: [fill the blanks addon](https://ankiweb.net/shared/info/1933645497).  
 For it to work, you will need to duplicate the `Markdown2Anki - Cloze` Note type and modify it by changing the `Front side` field to: `{{type:cloze:Front}}`.  
 
-This is a video with how you can achieve this: ![Video Tutorial on how to modify a note type](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/How_to_make_type_in_cloze.mp4)
+This is a video with how you can achieve this: [Video Tutorial on how to modify a note type](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/How_to_make_type_in_cloze.mp4)
 
 ![Demo of fill the blanks](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-addon.webp)
 
 ## Usage
 
 ### Markdown input formatting
 To ensure that your notes are properly recognized by the program, there are a few formatting requirements:
@@ -284,22 +284,20 @@
 A `debug_log.txt` file is also present in your program folder, which is created every time you run the program. This file contains more information on what happens when the program is running, the result of various processes, your configuration and so on.  
 If you find a bug in the program, it would be of great help if you could add this file to your issues on GitHub.  
 
 **Privacy Notice:** the log file has your configuration in it, as it can contain crucial information for debugging.  
 If you don't want to share your paths or other information from it when making issues, you should search-and-replace that information with some fake one, while trying not to change their general structure.
 
 ### Using clozes
-You can specify clozes in your markdown and they will be carried over to your anki cards. Whenever there is a word or sentence you'd like to have as a cloze, you can use Anki's formatting `{{c<number>::<word>}}` (notice the two colons, not just one).
+You can specify clozes in your markdown and they will be carried over to your anki cards. Whenever there is a word or sentence you'd like to have as a cloze, you can use Anki's formatting `{{c<number>::<word>::<hint?>}}` (notice the two colons, not just one).
+Clozes will also work in code blocks.
 
 The number tells Anki what cloze to add to what card. This means that if you have C1, C2 and C3, there will be three cards created (this is a feature of Anki, not of Markdown2Anki), each missing the respective words.  
 More on this here: https://docs.ankiweb.net/editing.html#cloze-deletion
 
-If the clozed word/sentence is present multiple times, it will be automatically turned into a cloze, so you only need to specify it once.
-This works also in code blocks.
-
 For example:
 ```python
 my_list = [3,5,2]
 # New list
 sorted_list = {{C1::sorted}}(my_list, {{C1::True}}) 
 # In place
 my_list.{{C1::sort}}(True)
@@ -310,15 +308,15 @@
 
 ### Changing Themes
 The default theme is mochitto's Rosé Pine theme, but there is also a catpuccin theme.  
 You can find all the themes in the [themes folder](https://github.com/Mochitto/Markdown2Anki/tree/master/themes).  
 To use another theme, you can just copy the CSS from the file in the themes folder and paste it in your Note types' styling field.  
 
 This can be found by accessing `Tools>Manage Note Types>(select your note type)>Cards(on the right)>Styling(on the left)`. The `Tools` menu is found in the top-left part of Anki's main menu.   
-You can reference this: ![Video Tutorial showing how to access a card's style](https://github.com/Mochitto/Markdown2Anki/blob/master/docs/How_to_find_styling.mp4)
+You can reference this: [Video Tutorial showing how to access a card's style](https://github.com/Mochitto/Markdown2Anki/blob/master/docs/How_to_find_styling.mp4)
 
 You can read more on how styling happens here: https://docs.ankiweb.net/templates/styling.html
 
 ### Navigating the UI
 The custom User Interface of the note-type that comes with this project is focused on the concept of tabs.  
 You can have side-by-side tabs and multiple tabs to toggle through.
```

### Comparing `markdown2anki-0.1.2/docs/Anki_import_example.webp` & `markdown2anki-0.2.0/docs/Anki_import_example.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/CLI_demo.mp4` & `markdown2anki-0.2.0/docs/CLI_demo.mp4`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo-cloze-addon.webp` & `markdown2anki-0.2.0/docs/Demo-cloze-addon.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo-cloze-answer.webp` & `markdown2anki-0.2.0/docs/Demo-cloze-answer.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo-cloze-split-screen-addon.webp` & `markdown2anki-0.2.0/docs/Demo-cloze-split-screen-addon.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo-cloze-standard.webp` & `markdown2anki-0.2.0/docs/Demo-cloze-standard.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo-split-screen.webp` & `markdown2anki-0.2.0/docs/Demo-split-screen.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo-update.webp` & `markdown2anki-0.2.0/docs/Demo-update.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Demo_highlight.gif` & `markdown2anki-0.2.0/docs/Demo_highlight.gif`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/How_to_find_styling.mp4` & `markdown2anki-0.2.0/docs/How_to_find_styling.mp4`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/How_to_make_type_in_cloze.mp4` & `markdown2anki-0.2.0/docs/How_to_make_type_in_cloze.mp4`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Main-demo_1.webp` & `markdown2anki-0.2.0/docs/Main-demo_1.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Terminal-demo.webp` & `markdown2anki-0.2.0/docs/Terminal-demo.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Usage_demo1.webp` & `markdown2anki-0.2.0/docs/Usage_demo1.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Usage_demo2.webp` & `markdown2anki-0.2.0/docs/Usage_demo2.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/Usage_demo3.webp` & `markdown2anki-0.2.0/docs/Usage_demo3.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/cloze_example.webp` & `markdown2anki-0.2.0/docs/cloze_example.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/light_mode_cloze.webp` & `markdown2anki-0.2.0/docs/light_mode_cloze.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/mobile_cloze_demo.webp` & `markdown2anki-0.2.0/docs/mobile_cloze_demo.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/mobile_demo.webp` & `markdown2anki-0.2.0/docs/mobile_demo.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/docs/rose-pine.webp` & `markdown2anki-0.2.0/docs/rose-pine.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/build_theme_builder.js` & `markdown2anki-0.2.0/frontend/build_theme_builder.js`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/esbuild.js` & `markdown2anki-0.2.0/frontend/esbuild.js`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/esbuild_themes.js` & `markdown2anki-0.2.0/frontend/esbuild_themes.js`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/esbuild_watch.js` & `markdown2anki-0.2.0/frontend/esbuild_watch.js`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/main_test.html` & `markdown2anki-0.2.0/frontend/main_test.html`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/package-lock.json` & `markdown2anki-0.2.0/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/package.json` & `markdown2anki-0.2.0/frontend/package.json`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/main.ts` & `markdown2anki-0.2.0/frontend/src/main.ts`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_latte.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_latte.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_macchiato.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/catpuccin_macchiato.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/rose_pine.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/rose_pine.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/Highlighting styles/rose_pine_dawn.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/Highlighting styles/rose_pine_dawn.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/catpuccin_latte.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/catpuccin_latte.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/catpuccin_macchiato.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/catpuccin_macchiato.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/rose_pine.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/rose_pine.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/CSS Themes/UI Themes/rose_pine_dawn.css` & `markdown2anki-0.2.0/frontend/src/style/CSS Themes/UI Themes/rose_pine_dawn.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/base.sass` & `markdown2anki-0.2.0/frontend/src/style/base.sass`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/modules/highlight/README.md` & `markdown2anki-0.2.0/frontend/src/style/modules/highlight/README.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/modules/highlight/highlight.sass` & `markdown2anki-0.2.0/frontend/src/style/modules/highlight/highlight.sass`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/modules/tab/README.md` & `markdown2anki-0.2.0/frontend/src/style/modules/tab/README.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/modules/tab/tab.sass` & `markdown2anki-0.2.0/frontend/src/style/modules/tab/tab.sass`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/modules/tab_group/README.md` & `markdown2anki-0.2.0/frontend/src/style/modules/tab_group/README.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/modules/tab_group/tab_group.sass` & `markdown2anki-0.2.0/frontend/src/style/modules/tab_group/tab_group.sass`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/themeless_main.sass` & `markdown2anki-0.2.0/frontend/src/style/themeless_main.sass`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/src/style/utilities/normalize.sass` & `markdown2anki-0.2.0/frontend/src/style/utilities/normalize.sass`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/frontend/tsconfig.json` & `markdown2anki-0.2.0/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/pyproject.toml` & `markdown2anki-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 [project]
 name = "markdown2anki"
-version = "0.1.2"
+version = "0.2.0"
 description = "A CLI tool and an apkg template to allow you to create flashcards from markdown and have a better experience while using anki for your studies. 🌸"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSES"}
 keywords = ["anki", "flashcard", "markdown", "apkg", "cli"]
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#authors-maintainers
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,26 @@
 
     config = config_handle.handle_configs(
         CONFIG_LINK_PATH, CONFIGFILE_NAME, ADD_TYPES_TO_CONFIG
     )
     log.setup_file_logging(
         logger, os.path.join(config["config directory"], "debug_log.txt")
     )
-
     current_version = ver.get_current_version(markdown2anki.__name__)
-    logger.info(f"Running Markdown2Anki v{current_version} 🌸")
+    logger.info(f"Running Markdown2Anki v{current_version} 🌸\n")
 
+    logger.info(f"Checking for updates...")
     latest_version = ver.get_latest_version(markdown2anki.__name__)
     if not (ver.check_for_version(current_version, latest_version)):
-        logger.info(f"⏫ There is a new version available: v{latest_version}!\n"
-                    "You can read what's new here: https://github.com/Mochitto/Markdown2Anki/blob/master/CHANGELOG.md\n\n")
+        logger.info(
+            f"⏫ There is a new version available: v{latest_version}!\n"
+            "You can read what's new here: https://github.com/Mochitto/Markdown2Anki/blob/master/CHANGELOG.md\n\n"
+        )
+    else:
+        logger.info("✨ Running the latest version!\n")
 
 
     expressive_debug(logger, "Processed config from main", config, "pprint")
     logger.info("Starting cards extraction")
 
     with open(config["input md file path"], "r", encoding="utf-8") as markdown_file:
         markdown_input = markdown_file.read()
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/Markdown2Anki.apkg` & `markdown2anki-0.2.0/src/markdown2anki/config/Markdown2Anki.apkg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/config_setup/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/config/config_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     fileConfig.add_option(
         type="str",
         option="Obsidian valut name",
         help="The name of the obsidian vault where the input file is from.",
         important_help="If left empty, Obsidian links will not work in your cards.",
         default="",
+        can_be_empty=True
     )
     fileConfig.add_option(
         type="ExistingPath",
         option="search images folder",
         help="This is where the program will look for images when they appear in your cards.\nIt also searches inside of subfolders.",
         important_help="Necessary. Must be an absolute path to an existing folder.",
     )
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/config_setup/casters.py` & `markdown2anki-0.2.0/src/markdown2anki/config/config_setup/casters.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/config_setup/validators.py` & `markdown2anki-0.2.0/src/markdown2anki/config/config_setup/validators.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/configs_handle.py` & `markdown2anki-0.2.0/src/markdown2anki/config/configs_handle.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/first_config.py` & `markdown2anki-0.2.0/src/markdown2anki/config/first_config.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/parse_args.py` & `markdown2anki-0.2.0/src/markdown2anki/config/parse_args.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/config/welcome_message.txt` & `markdown2anki-0.2.0/src/markdown2anki/config/welcome_message.txt`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/logger.py` & `markdown2anki-0.2.0/src/markdown2anki/logger.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 import logging
 
 import markdown2anki.md_2_anki.utils.common_types as Types
 from markdown2anki.md_2_anki.utils.card_error import CardError
 from markdown2anki.md_2_anki.process_card import process_card
-from markdown2anki.md_2_anki.process_clozes import (
-    get_clozes,
-    hash_clozes,
-    clean_code_from_clozes,
-    replace_cloze_text_with_hashes,
-    inject_clozes,
-    are_clozes_in_card,
-)
+from markdown2anki.md_2_anki.process_clozes import HandleClozes, are_clozes_in_card
 from markdown2anki.md_2_anki.process_images import get_images_to_copy
 from markdown2anki.md_2_anki.process_card.extract import extract_cards
 
 from markdown2anki.utils.debug_tools import expressive_debug
 
 # NOTE: if changes are made to the cards' HTML/CSS/JS, you also want to look into cards_specific_wrappers' functions
 
@@ -53,49 +46,36 @@
     failed_cards = []
     images_to_copy = {}
     aborted_cards = 0
     successful_cards = 0
     for index, card in enumerate(cards):
         # card is not immutable: it can change when clozes are found
         try:  # Handle CardErrors
-            cloze_card_flag = False
-
             if are_clozes_in_card(card):
-                cloze_card_flag = True
-
-                clozes = get_clozes(card)
-                hash_dictionary = hash_clozes(clozes)
+                clozes_handler = HandleClozes(card)
 
-                card_without_clozes = clean_code_from_clozes(card)
-                card_with_hashes = replace_cloze_text_with_hashes(
-                    card_without_clozes, hash_dictionary
+                formatted_card_with_hashes = process_card(
+                    clozes_handler.hashed_markdown, vault, linenos=linenos
                 )
 
-                formatted_card_without_clozes = process_card(
-                    card_with_hashes, vault, linenos=linenos
-                )
-
-                formatted_card = inject_clozes(
-                    formatted_card_without_clozes, hash_dictionary
+                formatted_card = clozes_handler.inject_clozes(
+                    formatted_card_with_hashes
                 )
+                processed_cards_with_cloze.append(formatted_card)
             else:
                 formatted_card = process_card(card, vault, linenos=linenos)
+                processed_cards.append(formatted_card)
 
             if images_dir:
                 images = get_images_to_copy(
                     formatted_card, images_dir, folders_to_exclude
                 )
                 images_to_copy.update(images)
                 # TODO: Add check for images not found to send to debug/Find a better way to handle errors
 
-            if cloze_card_flag:
-                processed_cards_with_cloze.append(formatted_card)
-            else:
-                processed_cards.append(formatted_card)
-
             successful_cards += 1
 
         except CardError as error:
             if fast_forward:
                 logger.info(f"|--- ❌ Failed to process the card number {index + 1}...")
                 logger.error(f"|------- ERROR: {error}")
                 aborted_cards += 1
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_image_plugin.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_image_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_link_plugin.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/compile/custom_plugins/obsidian_link_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/extract/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/format/formatters.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/format/formatters.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/format/wrappers.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/format/wrappers.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_card/swap/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_card/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_clozes/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_clozes/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,139 +5,132 @@
 import markdown2anki.md_2_anki.utils.common_types as Types
 from markdown2anki.md_2_anki.utils.card_error import CardError
 from markdown2anki.utils.debug_tools import expressive_debug
 
 logger = logging.getLogger(__name__)
 
 
-# TODO: might be worth turning these into a class
-# To have a global "clozes regex", as it was a problem
-# When writing tests (they were all different)
-
-
-def get_clozes(text: Types.MDString) -> List[Tuple[str, str]]:
-    """
-    Extract clozes from text.
-
-    Pattern:
-    {{c1::something}}
-    {{C9::something}}
-    """
-    clozes_regex = re.compile(r"(?i){{c(\d+)::(.+?)}}")
-
-    clozes_matches = clozes_regex.findall(text)
-
-    return clozes_matches
-
-
-def hash_clozes(clozes: List[Tuple[str, str]]) -> Dict[str, Tuple[str, str]]:
-    """
-    Transform matches from re.findall into a dictionary that has:
-    keys: hashed match
-    values: (cloze's number, cloze's text)
+class HandleClozes:
     """
-
-    # A dictionary built to use with translate()
-    # {key: ord(number), value: letter} + "-" : Z
-    number_to_letter_translation = {
-        48: "A",
-        49: "B",
-        50: "C",
-        51: "D",
-        52: "E",
-        53: "F",
-        54: "G",
-        55: "H",
-        56: "I",
-        57: "J",
-        45: "Z",
-    }
-
-    result = dict()
-    for cloze_number, cloze_text in clozes:
-        hash_number = str(hash(cloze_text))
-
-        hash_in_letters = hash_number.translate(number_to_letter_translation)
-        result[hash_in_letters] = (cloze_number, cloze_text)
-
-    return result
-
-
-def replace_cloze_text_with_hashes(
-    markdown_code: Types.MDString, hashed_clozes: Dict[str, Tuple[str, str]]
-) -> Types.MDString:
-    """
-    Replace the text of clozes ({{c1::This part}}) with the corresponding hash.
-
-    Raise an error if there are no matches, the reasons could be:
-    - The cloze is not a full word/number
-    - There are other clozes that are sub-strings of the one that you are matching
-    - Your cloze is a sub-string of another cloze, so it was already taken
+    This class takes care of hashing and unhashing clozes.
+    This is necessary to make sure code-highlighting won't break clozes.
     """
-    if not hashed_clozes:
-        return markdown_code
 
-    code_with_hashes = markdown_code
-    for hash_key, cloze_match in hashed_clozes.items():
-        cloze_regex = re.compile(rf"\b{cloze_match[1]}\b")
-        code_with_hashes, number_of_substitutions = re.subn(
-            cloze_regex, hash_key, code_with_hashes
-        )
-        if not number_of_substitutions:
-            raise CardError(
-                "Bad formatting in code's cloze; clozes should:\n"
-                + "- Be full words/numbers\n"
-                + "- Not be a sub-string of another cloze\n"
-                + "- Not have sub-strings of another cloze\n"
+    def __init__(self, card: Types.MDString) -> None:
+        self.card = card
+        self._clozes = self._get_clozes(card)
+        self._hash_dictionary = self._create_hash_dictionary(self._clozes)
+        self.hashed_markdown = self._hash_clozes()
+
+    def _get_clozes(self, text: Types.MDString) -> List[str]:
+        """
+        Extract clozes from text.
+
+        Pattern:
+        {{c1::something}}
+        {{C9::something}}
+        """
+        clozes_regex = re.compile(r"(?i)({{c\d+::.+?}})")
+
+        clozes_matches = clozes_regex.findall(text)
+
+        return clozes_matches
+
+    def _create_hash_dictionary(self, clozes: List[str]) -> Dict[str, str]:
+        """
+        Transform matched clozes into a dictionary that has:
+        keys: hashed match
+        values: cloze
+        """
+
+        # A dictionary built to use with translate()
+        # {key: ord(number), value: letter} + "-" : Z
+        number_to_letter_translation = {
+            48: "A",
+            49: "B",
+            50: "C",
+            51: "D",
+            52: "E",
+            53: "F",
+            54: "G",
+            55: "H",
+            56: "I",
+            57: "J",
+            45: "Z",
+        }
+
+        result = dict()
+        for cloze in clozes:
+            hash_number = str(hash(cloze))
+
+            hash_in_letters = hash_number.translate(number_to_letter_translation)
+            result[hash_in_letters] = cloze
+
+        return result
+
+    def _replace_clozes_with_hashes(
+        self, markdown_text: Types.MDString, hashed_clozes: Dict[str, str]
+    ) -> Types.MDString:
+        """
+        Replace the text of clozes ({{c1::This part}}) with the corresponding hash.
+        """
+        if not hashed_clozes:
+            return markdown_text
+
+        markdown_with_hashes = markdown_text
+
+        for hash_key, cloze in hashed_clozes.items():
+            cloze_regex = re.compile(re.escape(cloze))
+            markdown_with_hashes, number_of_substitutions = re.subn(
+                cloze_regex,
+                hash_key,
+                markdown_with_hashes,
             )
+            if number_of_substitutions < 1:
+                raise CardError(
+                    "Bad formatting in code's cloze; make sure you are not using nested clozes."
+                )
+        expressive_debug(logger, "Markdown with hash", markdown_with_hashes, "json")
+
+        return markdown_with_hashes
+
+    def _hash_clozes(self) -> Types.MDString:
+        """
+        Replace clozes that are part of the card with string hashes.
+        """
+        hashed_markdown = self._replace_clozes_with_hashes(
+            self.card, self._hash_dictionary
+        )
+        return hashed_markdown
 
-    return code_with_hashes
-
-
-def clean_code_from_clozes(text: Types.MDString) -> Types.MDString:
-    """
-    Replace clozes with their just their text, in the given text.
-    """
-    clozes_regex = re.compile(r"{{c(\d+)::(.+?)}}", re.IGNORECASE)
-
-    text_without_clozes = re.sub(clozes_regex, r"\2", text)
-
-    return text_without_clozes
-
-
-def inject_clozes(
-    card: Dict[str, Types.MDString], hashed_clozes: Dict[str, Tuple[str, str]]
-) -> Dict[str, Types.MDString]:
-    """
-    Replace the hashes in the text with the corresponding cloze:
-    HSJDKASKHDAKS -> {{c1::my cloze}}
-    """
-    front = card["front"]
-    back = card["back"]
-
-    for hashed_cloze, cloze_match in hashed_clozes.items():
-        number = cloze_match[0]
-        clozed_text = cloze_match[1]
-
-        word_regex = re.compile(rf"\b{hashed_cloze}\b")
+    def inject_clozes(
+        self, card: Dict[str, Types.MDString]
+    ) -> Dict[str, Types.MDString]:
+        """
+        Replace the hashes in the text with the corresponding cloze:
+        HSJDKASKHDAKS -> {{c1::my cloze}}
+        And normalize clozes (make sure the "c" is lowercase).
+        """
+        front = card["front"]
+        back = card["back"]
+
+        for hashed_cloze, cloze in self._hash_dictionary.items():
+            normalized_cloze = "{{c" + cloze[3:]
+            hash_regex = re.compile(re.escape(hashed_cloze))
 
-        front = re.sub(word_regex, f"{{{{c{number}::{clozed_text}}}}}", front)
-        back = re.sub(word_regex, f"{{{{c{number}::{clozed_text}}}}}", back)
+            front = re.sub(hash_regex, normalized_cloze, front)
+            back = re.sub(hash_regex, normalized_cloze, back)
 
-    return {"front": front, "back": back}
+        return {"front": front, "back": back}
 
 
 def are_clozes_in_card(card: Types.MDString) -> bool:
     """
     Check if in the front of the card there is at least one cloze
 
-    Dict:
-    "front": HTMLString
-    "back": HTMLString
-
     Pattern:
     {{c1::something}}
     {{C5::something else}}
     """
     clozes_regex = re.compile(r"{{c(\d+)::(.+?)}}", re.IGNORECASE)
 
     return bool(clozes_regex.search(card))
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/process_images/__init__.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/process_images/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/card_types.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/card_types.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/md_2_anki/utils/debug_tools.py` & `markdown2anki-0.2.0/src/markdown2anki/md_2_anki/utils/debug_tools.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/output_handler.py` & `markdown2anki-0.2.0/src/markdown2anki/output_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,16 +69,17 @@
             for card in cloze_cards:
                 writer.writerow(card)
 
 
 def write_failed_cards(
     failed_cards: List[Types.MDString], file_path: Types.PathString
 ) -> None:
-    with open(file_path, "w", encoding="utf-8") as output:
+    with open(file_path, "a", encoding="utf-8") as output:
         output.write("\n\n---\n\n".join(failed_cards))
+        output.write("\n\n---\n\n")
 
 
 def backup_file(file_path: Types.PathString, output_folder: Types.PathString) -> None:
     """
     Create a copy of the file at file_path iin the output_folder
     with a new file name that "{now.isoformat}.md".
     """
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki/template for coding cards.md` & `markdown2anki-0.2.0/src/markdown2anki/template for coding cards.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/utils/debug_tools.py` & `markdown2anki-0.2.0/src/markdown2anki/utils/debug_tools.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki/version_check.py` & `markdown2anki-0.2.0/src/markdown2anki/version_check.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/src/markdown2anki.egg-info/PKG-INFO` & `markdown2anki-0.2.0/src/markdown2anki.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown2anki
-Version: 0.1.2
+Version: 0.2.0
 Summary: A CLI tool and an apkg template to allow you to create flashcards from markdown and have a better experience while using anki for your studies. 🌸
 Author-email: "Alex Biosa (mochitto)" <mochittodeveloper@gmail.com>
 License: Copyright (C) 2023, Alex Biosa (mochitto), mochittodeveloper@gmail.com 
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
@@ -148,15 +148,15 @@
 - **Mobile first responsive CSS**: to ensure it's fully responsive on all devices.
 - **High-level dev documentation** to make it easier for contributions and maintenance.
 
 ## Images
 
 ### CLI
 ![Demo image of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Terminal-demo.webp)  
-![Video demo of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/CLI_demo.mp4)
+[Video demo of the CLI](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/CLI_demo.mp4)
 ### Split-screen
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-split-screen.webp) 
 ### Code highlighting
 ![Demo code highlighting](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo_highlight.gif)
 ### Clozes support
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-standard.webp) 
 ![Demo image](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-answer.webp) 
@@ -214,15 +214,15 @@
 You can learn more on `.apkg` files here: https://docs.ankiweb.net/exporting.html#deck-apkg
 
 ### Using fill the blanks
 
 If you would like to have "type-in" clozes, you can use this addon: [fill the blanks addon](https://ankiweb.net/shared/info/1933645497).  
 For it to work, you will need to duplicate the `Markdown2Anki - Cloze` Note type and modify it by changing the `Front side` field to: `{{type:cloze:Front}}`.  
 
-This is a video with how you can achieve this: ![Video Tutorial on how to modify a note type](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/How_to_make_type_in_cloze.mp4)
+This is a video with how you can achieve this: [Video Tutorial on how to modify a note type](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/How_to_make_type_in_cloze.mp4)
 
 ![Demo of fill the blanks](https://raw.githubusercontent.com/Mochitto/Markdown2Anki/master/docs/Demo-cloze-addon.webp)
 
 ## Usage
 
 ### Markdown input formatting
 To ensure that your notes are properly recognized by the program, there are a few formatting requirements:
@@ -367,22 +367,20 @@
 A `debug_log.txt` file is also present in your program folder, which is created every time you run the program. This file contains more information on what happens when the program is running, the result of various processes, your configuration and so on.  
 If you find a bug in the program, it would be of great help if you could add this file to your issues on GitHub.  
 
 **Privacy Notice:** the log file has your configuration in it, as it can contain crucial information for debugging.  
 If you don't want to share your paths or other information from it when making issues, you should search-and-replace that information with some fake one, while trying not to change their general structure.
 
 ### Using clozes
-You can specify clozes in your markdown and they will be carried over to your anki cards. Whenever there is a word or sentence you'd like to have as a cloze, you can use Anki's formatting `{{c<number>::<word>}}` (notice the two colons, not just one).
+You can specify clozes in your markdown and they will be carried over to your anki cards. Whenever there is a word or sentence you'd like to have as a cloze, you can use Anki's formatting `{{c<number>::<word>::<hint?>}}` (notice the two colons, not just one).
+Clozes will also work in code blocks.
 
 The number tells Anki what cloze to add to what card. This means that if you have C1, C2 and C3, there will be three cards created (this is a feature of Anki, not of Markdown2Anki), each missing the respective words.  
 More on this here: https://docs.ankiweb.net/editing.html#cloze-deletion
 
-If the clozed word/sentence is present multiple times, it will be automatically turned into a cloze, so you only need to specify it once.
-This works also in code blocks.
-
 For example:
 ```python
 my_list = [3,5,2]
 # New list
 sorted_list = {{C1::sorted}}(my_list, {{C1::True}}) 
 # In place
 my_list.{{C1::sort}}(True)
@@ -393,15 +391,15 @@
 
 ### Changing Themes
 The default theme is mochitto's Rosé Pine theme, but there is also a catpuccin theme.  
 You can find all the themes in the [themes folder](https://github.com/Mochitto/Markdown2Anki/tree/master/themes).  
 To use another theme, you can just copy the CSS from the file in the themes folder and paste it in your Note types' styling field.  
 
 This can be found by accessing `Tools>Manage Note Types>(select your note type)>Cards(on the right)>Styling(on the left)`. The `Tools` menu is found in the top-left part of Anki's main menu.   
-You can reference this: ![Video Tutorial showing how to access a card's style](https://github.com/Mochitto/Markdown2Anki/blob/master/docs/How_to_find_styling.mp4)
+You can reference this: [Video Tutorial showing how to access a card's style](https://github.com/Mochitto/Markdown2Anki/blob/master/docs/How_to_find_styling.mp4)
 
 You can read more on how styling happens here: https://docs.ankiweb.net/templates/styling.html
 
 ### Navigating the UI
 The custom User Interface of the note-type that comes with this project is focused on the concept of tabs.  
 You can have side-by-side tabs and multiple tabs to toggle through.
```

### Comparing `markdown2anki-0.1.2/src/markdown2anki.egg-info/SOURCES.txt` & `markdown2anki-0.2.0/src/markdown2anki.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitattributes
 .gitignore
 CHANGELOG.md
 CONTRIBUTING.md
 GPL3
 LICENSES
-Note_when_updating.txt
 PYGMENTS_AUTHORS
 README.md
 pyproject.toml
 docs/Anki_import_example.webp
 docs/CLI_demo.mp4
 docs/Demo-cloze-addon.webp
 docs/Demo-cloze-answer.webp
@@ -137,18 +136,17 @@
 tests/unit_tests/md_2_anki/process_card/extract/test_parse_tab_label.py
 tests/unit_tests/md_2_anki/process_card/format/test_format_tab.py
 tests/unit_tests/md_2_anki/process_card/format/test_format_tab_group.py
 tests/unit_tests/md_2_anki/process_card/swap/test_create_back_tabs_list.py
 tests/unit_tests/md_2_anki/process_card/swap/test_create_front_tabs_list.py
 tests/unit_tests/md_2_anki/process_card/swap/test_get_swap_mappings.py
 tests/unit_tests/md_2_anki/process_clozes/test_are_clozes_in_card.py
-tests/unit_tests/md_2_anki/process_clozes/test_clean_code_from_clozes.py
 tests/unit_tests/md_2_anki/process_clozes/test_get_clozes.py
 tests/unit_tests/md_2_anki/process_clozes/test_hash_clozes.py
-tests/unit_tests/md_2_anki/process_clozes/test_replace_cloze_text_with_hashes.py
+tests/unit_tests/md_2_anki/process_clozes/test_replace_clozes_with_hashes.py
 tests/unit_tests/md_2_anki/process_images/test_find_image_path.py
 tests/unit_tests/md_2_anki/process_images/test_get_images_sources.py
 theme_builder/README.md
 theme_builder/main.js
 theme_builder/test.html
 theme_builder/style/Hightlight_theme_template.css
 theme_builder/style/UI_theme_template.css
```

### Comparing `markdown2anki-0.1.2/tests/assets/images/2010.jpg` & `markdown2anki-0.2.0/tests/assets/images/2010.jpg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/MORE/Toing.jpg` & `markdown2anki-0.2.0/tests/assets/images/MORE/Toing.jpg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/MORE/YES_ME/FroW.jpeg` & `markdown2anki-0.2.0/tests/assets/images/MORE/YES_ME/FroW.jpeg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/MORE/YES_ME/i_am_a_forest_fire.jpeg` & `markdown2anki-0.2.0/tests/assets/images/MORE/YES_ME/i_am_a_forest_fire.jpeg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/MORE/exclude_me_too/mmmm.jpg` & `markdown2anki-0.2.0/tests/assets/images/MORE/exclude_me_too/mmmm.jpg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/MORE/oiter.jpg` & `markdown2anki-0.2.0/tests/assets/images/MORE/oiter.jpg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/MORE/vruM.jpg` & `markdown2anki-0.2.0/tests/assets/images/MORE/vruM.jpg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/WAAAA.jpeg` & `markdown2anki-0.2.0/tests/assets/images/WAAAA.jpeg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/assets/images/exclude_me/fkboi.jpeg` & `markdown2anki-0.2.0/tests/assets/images/exclude_me/fkboi.jpeg`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/config/test_handle_configs.py` & `markdown2anki-0.2.0/tests/integration/config/test_handle_configs.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/config/test_welcome_user.py` & `markdown2anki-0.2.0/tests/integration/config/test_welcome_user.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/extract/test_extract_tab.py` & `markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/extract/test_extract_tab.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/format/test_formatting.py` & `markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/format/test_formatting.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/swap/test_get_swapped_card.py` & `markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/swap/test_get_swapped_card.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/md_2_anki/process_card/test_process_card.py` & `markdown2anki-0.2.0/tests/integration/md_2_anki/process_card/test_process_card.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/integration/md_2_anki/process_clozes/test_clozes_processing.py` & `markdown2anki-0.2.0/tests/integration/md_2_anki/process_clozes/test_clozes_processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 import markdown2anki.md_2_anki.process_clozes as clozes
 
 
 class TestClozesProcessing:
     def test_basic_case(self):
         content = (
-            "This is a string with 2 {{c1::clozes}}.\n"
+            "This is a string with 2 {{c1::clozes::with hints!}}.\n"
             + "Another line with another {{c2::cloze}}."
         )
 
         assert clozes.are_clozes_in_card(content)
-        match_clozes = clozes.get_clozes(content)
-        hashed_clozes = clozes.hash_clozes(match_clozes)
-        cleaned_content = clozes.clean_code_from_clozes(content)
-        hashed_content = clozes.replace_cloze_text_with_hashes(
-            cleaned_content, hashed_clozes
+        cloze_handler = clozes.HandleClozes(content)
+
+        card = {"front": cloze_handler.hashed_markdown, "back": ""}
+        processed_card = cloze_handler.inject_clozes(card)
+
+        assert processed_card["front"] == content
+
+    def test_single_letter_case(self):
+        content = (
+                "This is a cloze with a single letter {c1::a}"
+        )
+
+        assert clozes.are_clozes_in_card(content)
+        cloze_handler = clozes.HandleClozes(content)
+
+        card = {"front": cloze_handler.hashed_markdown, "back": ""}
+        processed_card = cloze_handler.inject_clozes(card)
+
+        assert processed_card["front"] == content
+
+    def test_same_cloze_case(self):
+        content = (
+            "This is a string with 2 {{c1::clozes}}.\n"
+            + "Another line, same {{c1::clozes}}."
         )
 
-        card = {"front": hashed_content, "back": ""}
-        processed_card = clozes.inject_clozes(card, hashed_clozes)
+        assert clozes.are_clozes_in_card(content)
+        cloze_handler = clozes.HandleClozes(content)
+
+        card = {"front": cloze_handler.hashed_markdown, "back": ""}
+        processed_card = cloze_handler.inject_clozes(card)
 
         assert processed_card["front"] == content
 
     def test_variation_case(self):
         """
-        Check for high numbers and uppercase/lowercase "c".
-
+        Check for high numbers, uppercase/lowercase "c" and
+        uppercase/lowercase similar strings.
         """
         content = (
             "This is a string with 2 {{C394::cloZe}}.\n"
-            + "Another line, same {{C394::cloZe}}."
+            + "Another line, same {{C394::cloze}}."
         )
 
-        # When clozes are injected back, the c normalized,
+        # When clozes are injected back, the "c" should be normalized,
         # so it is always undercase.
         normalized_content = (
             "This is a string with 2 {{c394::cloZe}}.\n"
-            + "Another line, same {{c394::cloZe}}."
+            + "Another line, same {{c394::cloze}}."
         )
 
         assert clozes.are_clozes_in_card(content)
-        match_clozes = clozes.get_clozes(content)
-        hashed_clozes = clozes.hash_clozes(match_clozes)
-        cleaned_content = clozes.clean_code_from_clozes(content)
-        hashed_content = clozes.replace_cloze_text_with_hashes(
-            cleaned_content, hashed_clozes
-        )
+        cloze_handler = clozes.HandleClozes(content)
 
-        card = {"front": hashed_content, "back": ""}
-        processed_card = clozes.inject_clozes(card, hashed_clozes)
+        card = {"front": cloze_handler.hashed_markdown, "back": ""}
+        processed_card = cloze_handler.inject_clozes(card)
 
         assert processed_card["front"] == normalized_content
 
     def test_false_case(self):
         content = "This is a string with 2 {{c1:clozeS}}.\n" + "Another line."
         assert not clozes.are_clozes_in_card(content)
-        match_clozes = clozes.get_clozes(content)
-        hashed_clozes = clozes.hash_clozes(match_clozes)
-        cleaned_content = clozes.clean_code_from_clozes(content)
-        hashed_content = clozes.replace_cloze_text_with_hashes(
-            cleaned_content, hashed_clozes
-        )
+        cloze_handler = clozes.HandleClozes(content)
 
-        card = {"front": hashed_content, "back": ""}
-        processed_card = clozes.inject_clozes(card, hashed_clozes)
+        card = {"front": cloze_handler.hashed_markdown, "back": ""}
+        processed_card = cloze_handler.inject_clozes(card)
 
         assert processed_card["front"] == content
```

### Comparing `markdown2anki-0.1.2/tests/integration/md_2_anki/process_images/test_process_images.py` & `markdown2anki-0.2.0/tests/integration/md_2_anki/process_images/test_process_images.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/setup/__init__.py` & `markdown2anki-0.2.0/tests/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/setup/config_file_patch.py` & `markdown2anki-0.2.0/tests/setup/config_file_patch.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/config/test_configs_handle.py` & `markdown2anki-0.2.0/tests/unit_tests/config/test_configs_handle.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/config/test_first_config.py` & `markdown2anki-0.2.0/tests/unit_tests/config/test_first_config.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/config/test_setup_typeConfig.py` & `markdown2anki-0.2.0/tests/unit_tests/config/test_setup_typeConfig.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_image_plugin.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_image_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_wikilink_plugin.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/compile/test_obsidian_wikilink_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_extract_cards.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_extract_cards.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_bodies.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_bodies.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_labels.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_extract_tabs_labels.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_parse_flags.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_parse_flags.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/extract/test_parse_tab_label.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/extract/test_parse_tab_label.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/format/test_format_tab.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/format/test_format_tab.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/format/test_format_tab_group.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/format/test_format_tab_group.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/test_create_back_tabs_list.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/test_create_back_tabs_list.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/test_create_front_tabs_list.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/test_create_front_tabs_list.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_card/swap/test_get_swap_mappings.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_card/swap/test_get_swap_mappings.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_are_clozes_in_card.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_are_clozes_in_card.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_hash_clozes.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_hash_clozes.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,54 +5,55 @@
     def test_basic_case(self):
         content = (
             "This is a string with 2 {{c1::clozes}}.\n"
             + "Another line with another {{c2::cloze}}."
         )
 
         expected_hashed_clozes = {
-            "something": ("1", "clozes"),
-            "something else": ("2", "cloze"),
+            "something": "{{c1::clozes}}",
+            "something else": "{{c2::cloze}}",
         }
         expected_length = len(expected_hashed_clozes.values())
 
-        match_clozes = clozes.get_clozes(content)
-        hashed_clozes = clozes.hash_clozes(match_clozes)
-        length = len(hashed_clozes.values())
+        clozes_handler = clozes.HandleClozes(content)
+
+        hashed_clozes = clozes_handler._hash_dictionary
 
+        length = len(hashed_clozes.values())
         difference = set(expected_hashed_clozes.values()) - set(hashed_clozes.values())
 
         assert not difference and expected_length == length
 
     def test_variation_case(self):
         """
         Check for high numbers and uppercase/lowercase "c".
         """
         content = (
             "This is a string with 2 {{C394::cloZe}}.\n"
             + "Another line, same {{C394::cloZe}}."
         )
 
-        expected_hashed_clozes = {"something": ("394", "cloZe")}
+        expected_hashed_clozes = {"something": "{{C394::cloZe}}"}
         expected_length = len(expected_hashed_clozes.values())
 
-        match_clozes = clozes.get_clozes(content)
-        hashed_clozes = clozes.hash_clozes(match_clozes)
+        clozes_handler = clozes.HandleClozes(content)
+        hashed_clozes = clozes_handler._hash_dictionary
 
         length = len(hashed_clozes.values())
         difference = set(expected_hashed_clozes.values()) - set(
             hashed_clozes.values()
         )  # type:ignore
 
         assert not difference and expected_length == length
 
     def test_false_case(self):
         content = "This is a string with 2 {{c1:clozeS}}.\n" + "Another line."
         expected_hashed_clozes = {}
         expected_length = len(expected_hashed_clozes.values())
 
-        match_clozes = clozes.get_clozes(content)
-        hashed_clozes = clozes.hash_clozes(match_clozes)
+        clozes_handler = clozes.HandleClozes(content)
+        hashed_clozes = clozes_handler._hash_dictionary
 
         length = len(hashed_clozes.values())
         difference = set(expected_hashed_clozes.values()) - set(hashed_clozes.values())
 
         assert not difference and expected_length == length
```

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_clozes/test_replace_cloze_text_with_hashes.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_clozes/test_replace_clozes_with_hashes.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,19 @@
         )
         expected_hashed_content = (
             "This is a string with 2 HIIDAJIGJADFBDBJJDF.\n"
             + "Another line with another ZEJDDDHDEBDEICGIHBGF."
         )
 
         hashed_clozes = {
-            "HIIDAJIGJADFBDBJJDF": ("1", "clozes"),
-            "ZEJDDDHDEBDEICGIHBGF": ("2", "cloze"),
+                "HIIDAJIGJADFBDBJJDF": "{{c1::clozes}}",
+                "ZEJDDDHDEBDEICGIHBGF": "{{c2::cloze}}",
         }
-
-        cleaned_content = clozes.clean_code_from_clozes(content)
-        hashed_content = clozes.replace_cloze_text_with_hashes(
-            cleaned_content, hashed_clozes
-        )
+        clozes_handler = clozes.HandleClozes(content)
+        hashed_content = clozes_handler._replace_clozes_with_hashes(clozes_handler.card, hashed_clozes)
 
         assert hashed_content == expected_hashed_content
 
     def test_variation_case(self):
         """
         Check for high numbers and uppercase/lowercase "c".
         """
@@ -33,21 +30,20 @@
             + "Another line, same {{C394::cloZe}}."
         )
         expected_hashed_content = (
             "This is a string with 2 ZIAGEIHFICDIEFCECJF.\n"
             + "Another line, same ZIAGEIHFICDIEFCECJF."
         )
 
-        hashed_clozes = {"ZIAGEIHFICDIEFCECJF": ("394", "cloZe")}
-        cleaned_content = clozes.clean_code_from_clozes(content)
-        hashed_content = clozes.replace_cloze_text_with_hashes(
-            cleaned_content, hashed_clozes
-        )
+        hashed_clozes = {"ZIAGEIHFICDIEFCECJF": "{{C394::cloZe}}"}
+        clozes_handler = clozes.HandleClozes(content)
+        hashed_content = clozes_handler._replace_clozes_with_hashes(clozes_handler.card, hashed_clozes)
 
         assert hashed_content == expected_hashed_content
 
     def test_false_case(self):
         content = "This is a string with 2 {{c1:clozeS}}.\n" + "Another line."
         hashed_clozes = {}
-        hashed_content = clozes.replace_cloze_text_with_hashes(content, hashed_clozes)
+        clozes_handler = clozes.HandleClozes(content)
+        hashed_content = clozes_handler._replace_clozes_with_hashes(clozes_handler.card, hashed_clozes)
 
         assert hashed_content == content
```

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_images/test_find_image_path.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_images/test_find_image_path.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/tests/unit_tests/md_2_anki/process_images/test_get_images_sources.py` & `markdown2anki-0.2.0/tests/unit_tests/md_2_anki/process_images/test_get_images_sources.py`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/theme_builder/README.md` & `markdown2anki-0.2.0/theme_builder/README.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/theme_builder/main.js` & `markdown2anki-0.2.0/theme_builder/main.js`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/theme_builder/style/Hightlight_theme_template.css` & `markdown2anki-0.2.0/theme_builder/style/Hightlight_theme_template.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/theme_builder/style/UI_theme_template.css` & `markdown2anki-0.2.0/theme_builder/style/UI_theme_template.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/theme_builder/style/themeless_main.css` & `markdown2anki-0.2.0/theme_builder/style/themeless_main.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/theme_builder/test.html` & `markdown2anki-0.2.0/theme_builder/test.html`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/README.md` & `markdown2anki-0.2.0/themes/README.md`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/catpuccin_latte.css` & `markdown2anki-0.2.0/themes/catpuccin_latte.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/catpuccin_macchiato.css` & `markdown2anki-0.2.0/themes/catpuccin_macchiato.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/docs/catpuccin-latte.webp` & `markdown2anki-0.2.0/themes/docs/catpuccin-latte.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/docs/catpuccin-macchiato.webp` & `markdown2anki-0.2.0/themes/docs/catpuccin-macchiato.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/docs/rose-pine-dawn.webp` & `markdown2anki-0.2.0/themes/docs/rose-pine-dawn.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/docs/rose-pine.webp` & `markdown2anki-0.2.0/themes/docs/rose-pine.webp`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/rose_pine.css` & `markdown2anki-0.2.0/themes/rose_pine.css`

 * *Files identical despite different names*

### Comparing `markdown2anki-0.1.2/themes/rose_pine_dawn.css` & `markdown2anki-0.2.0/themes/rose_pine_dawn.css`

 * *Files identical despite different names*

