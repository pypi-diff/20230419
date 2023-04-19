# Comparing `tmp/foliantcontrib.escapecode-1.0.4.tar.gz` & `tmp/foliantcontrib.escapecode-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foliantcontrib.escapecode-1.0.4.tar", last modified: Thu Jul 30 21:09:54 2020, max compression
+gzip compressed data, was "foliantcontrib.escapecode-1.0.5.tar", last modified: Wed Apr 19 13:01:07 2023, max compression
```

## Comparing `foliantcontrib.escapecode-1.0.4.tar` & `foliantcontrib.escapecode-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliant/
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliant/preprocessors/
--rw-r--r--   0 lomov     (1000) lomov     (1000)     9607 2020-07-30 21:09:03.000000 foliantcontrib.escapecode-1.0.4/foliant/preprocessors/escapecode.py
--rw-r--r--   0 lomov     (1000) lomov     (1000)     3375 2020-07-22 15:25:01.000000 foliantcontrib.escapecode-1.0.4/foliant/preprocessors/unescapecode.py
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/
--rw-rw-r--   0 lomov     (1000) lomov     (1000)     8481 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/PKG-INFO
--rw-rw-r--   0 lomov     (1000) lomov     (1000)      336 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/SOURCES.txt
--rw-rw-r--   0 lomov     (1000) lomov     (1000)        1 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/dependency_links.txt
--rw-rw-r--   0 lomov     (1000) lomov     (1000)       15 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/requires.txt
--rw-rw-r--   0 lomov     (1000) lomov     (1000)        8 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/top_level.txt
--rw-r--r--   0 lomov     (1000) lomov     (1000)     6331 2020-07-19 00:32:20.000000 foliantcontrib.escapecode-1.0.4/README.md
--rw-r--r--   0 lomov     (1000) lomov     (1000)     1100 2020-07-30 21:09:03.000000 foliantcontrib.escapecode-1.0.4/setup.py
--rw-rw-r--   0 lomov     (1000) lomov     (1000)     8481 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/PKG-INFO
--rw-rw-r--   0 lomov     (1000) lomov     (1000)       38 2020-07-30 21:09:54.000000 foliantcontrib.escapecode-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:01:07.018711 foliantcontrib.escapecode-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-19 13:01:07.018711 foliantcontrib.escapecode-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:01:07.014711 foliantcontrib.escapecode-1.0.5/foliant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:01:07.018711 foliantcontrib.escapecode-1.0.5/foliant/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/foliant/preprocessors/escapecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/foliant/preprocessors/unescapecode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:01:07.018711 foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-19 13:01:07.000000 foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-19 13:01:07.000000 foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:01:07.000000 foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 13:01:07.000000 foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 13:01:07.000000 foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:01:07.018711 foliantcontrib.escapecode-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:01:07.018711 foliantcontrib.escapecode-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/tests/test_escapecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-19 13:00:55.000000 foliantcontrib.escapecode-1.0.5/tests/test_unescapecode.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `foliantcontrib.escapecode-1.0.4/foliant/preprocessors/unescapecode.py` & `foliantcontrib.escapecode-1.0.5/foliant/preprocessors/unescapecode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-'''
+"""
 Preprocessor for Foliant documentation authoring tool.
 Unescapes raw content that is escaped by the
 ``escapecode`` preprocessor.
-'''
+"""
 
-import re
 from pathlib import Path
 from typing import Dict
 OptionValue = int or float or bool or str
 
 from foliant.utils import output
 from foliant.preprocessors.base import BasePreprocessor
 
@@ -26,21 +25,21 @@
         self._cache_dir_path = (self.project_path / self.options['cache_dir']).resolve()
 
         self.logger = self.logger.getChild('unescapecode')
 
         self.logger.debug(f'Preprocessor inited: {self.__dict__}')
 
     def _unescape(self, options: Dict[str, OptionValue], full_tag: str) -> str:
-        '''Replace the ``<escaped>`` tag with the content of the corresponding file.
+        """Replace the ``<escaped>`` tag with the content of the corresponding file.
 
         :param options: Tag options (i.e. attributes)
 
         :returns: The content of the file that is defined
             by the ``hash`` attribute
-        '''
+        """
 
         self.logger.debug(f'Processing the tag, options: {options}')
 
         saved_content_hash = options.get('hash', '')
 
         saved_content_file_path = self._cache_dir_path / f'{saved_content_hash}.md'
 
@@ -63,22 +62,22 @@
             output(warning_message, self.quiet)
 
             self.logger.warning(warning_message)
 
             return full_tag
 
     def unescape(self, markdown_content: str) -> str:
-        '''Find the ``<escaped>...</escaped>`` tags that generated by the ``escapecode``
+        """Find the ``<escaped>...</escaped>`` tags that generated by the ``escapecode``
         preprocessor. Replace the tags with the content of corresponding files.
 
         :param markdown_content: Markdown content that may contain
             the ``<escaped>...</escaped>`` tags
 
         :returns: Markdown content with raw parts restored from files
-        '''
+        """
 
         def _sub(escaped_tag) -> str:
             return self._unescape(self.get_options(escaped_tag.group('options')), escaped_tag.group(0))
 
         markdown_content = self.pattern.sub(_sub, markdown_content)
 
         return markdown_content
```

### Comparing `foliantcontrib.escapecode-1.0.4/foliantcontrib.escapecode.egg-info/PKG-INFO` & `foliantcontrib.escapecode-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,230 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.escapecode
-Version: 1.0.4
+Version: 1.0.5
 Summary: Preprocessor for Foliant to escape/unescape raw content.
 Home-page: https://github.com/foliant-docs/foliantcontrib.escapecode
 Author: Artemy Lomov
 Author-email: artemy@lomov.ru
 License: MIT
-Description: [![](https://img.shields.io/pypi/v/foliantcontrib.escapecode.svg)](https://pypi.org/project/foliantcontrib.escapecode/) [![](https://img.shields.io/github/v/tag/foliant-docs/foliantcontrib.escapecode.svg?label=GitHub)](https://github.com/foliant-docs/foliantcontrib.escapecode)
-        
-        # EscapeCode and UnescapeCode
-        
-        EscapeCode and UnescapeCode preprocessors work in pair.
-        
-        EscapeCode finds in the source Markdown content the parts that should not be modified by any next preprocessors. Examples of content that should be left raw: fence code blocks, pre code blocks, inline code.
-        
-        EscapeCode replaces these raw content parts with pseudo-XML tags recognized by UnescapeCode preprocessor.
-        
-        EscapeCode saves raw content parts into files. Later, UnescapeCode restores this content from files.
-        
-        Also, before the replacement, EscapeCode normalizes the source Markdown content to unify and simplify further operations. The preprocessor replaces `CRLF` with `LF`, removes excessive whitespace characters, provides trailing newline, etc.
-        
-        ## Installation
-        
-        To install EscapeCode and UnescapeCode preprocessors, run:
-        
-        ```bash
-        $ pip install foliantcontrib.escapecode
-        ```
-        
-        See more details below.
-        
-        ## Integration with Foliant and Includes
-        
-        You may call EscapeCode and UnescapeCode explicitly, but these preprocessors are integrated with Foliant core (since version 1.0.10) and with Includes preprocessor (since version 1.1.1).
-        
-        The `escape_code` project’s config option, if set to `true`, provides applying EscapeCode before all other preprocessors, and applying UnescapeCode after all other preprocessors. Also this option tells Includes preprocessor to apply EscapeCode to each included file.
-        
-        In this mode EscapeCode and UnescapeCode preprocessors deprecate _unescape preprocessor.
-        
-            >    **Note**
-            >
-            >    The preprocessor _unescape is a part of Foliant core. It allows to use pseudo-XML tags in code examples. If you want an opening tag not to be interpreted by any preprocessor, precede this tag with the `<` character. The preprocessor _unescape applies after all other preprocessors and removes such characters.
-        
-        Config example:
-        
-        ```yaml
-        title: My Awesome Project
-        
-        chapters:
-            - index.md
-            ...
-        
-        escape_code: true
-        
-        preprocessors:
-            ...
-            - includes
-            ...
-        ...
-        ```
-        
-        If the `escape_code` option isn’t used or set to `false`, backward compatibility mode is involved. In this mode EscapeCode and UnescapeCode aren’t applied automatically, but _unescape preprocessor is applied.
-        
-        In more complicated case, you may pass some custom options to EscapeCode preprocessor:
-        
-        ```
-        escape_code:
-            options:
-                ...
-        ```
-        
-        Custom options available in EscapeCode since version 1.0.2. Foliant core supports passing custom options to EscapeCode preprocessor as the value of `escape_code.options` parameter since version 1.0.11. Options are described below.
-        
-        The Python package that includes EscapeCode and UnescapeCode preprocessors is the dependence of Includes preprocessor since version 1.1.1. At the same time this package isn’t a dependence of Foliant core. To use `escape_code` config option in Foliant core, you have to install the package with EscapeCode and UnescapeCode preprocessors separately.
-        
-        ## Explicit Enabling
-        
-        You may not want to use the `escape_code` option and call the preprocessors explicitly:
-        
-        ```yaml
-        preprocessors:
-            - escapecode      # usually the first list item
-            ...
-            - unescapecode    # usually the last list item
-        ```
-        
-        Both preprocessors allow to override the path to the directory that is used to store temporary files:
-        
-        ```yaml
-        preprocessors:
-            - escapecode:
-                cache_dir: !path .escapecodecache
-            ...
-            - unescapecode:
-                cache_dir: !path .escapecodecache
-        ```
-        
-        The default values are shown in this example. EscapeCode and related UnescapeCode must work with the same cache directory.
-        
-        Note that if you use Includes preprocessor, and the included content doesn’t belong to the current Foliant project, there’s no way to escape raw parts of this content before Includes preprocessor is applied.
-        
-        ## Config
-        
-        Since version 1.0.2, EscapeCode preprocessor supports the option `actions` in additional to `cache_dir`.
-        
-        The value of `actions` options should be a list of acceptable actions. By default, the following list is used:
-        
-        ```yaml
-        actions:
-            - normalize
-            - escape:
-                - fence_blocks
-                - pre_blocks
-                - inline_code
-        ```
-        
-        This default list may be overridden. For example:
-        
-        ```yaml
-        actions:
-            - normalize
-            - escape:
-                - fence_blocks
-                - inline_code
-                - tags:
-                    - plantuml
-                    - seqdiag
-                - comments
-        ```
-        
-        Meanings of parameters:
-        
-        * `normalize`—perform normalization;
-        * `escape`—perform escaping of certain types of raw content:
-            * `fence_blocks`—fence code blocks;
-            * `pre_blocks`—pre code blocks;
-            * `inline_code`—inline code;
-            * `comments`—HTML-style comments, also usual for Markdown;
-            * `tags`—content of certain tags with the tags themselves, for example `plantuml` for `<<plantuml>...</plantuml>`.
-        
-        ## Usage
-        
-        Below you can see an example of Markdown content with code blocks and inline code.
-        
-            # Heading
-        
-            Text that contains some `inline code`.
-        
-            Below is a fence code block, language is optional:
-        
-            ```python
-            import this
-            ```
-        
-            One more fence code block:
-        
-            ~~~
-            # This is a comment that should not be interpreted as a heading
-        
-            print('Hello World')
-            ~~~
-        
-            And this is a pre code block:
-        
-                mov dx, hello;
-                mov ah, 9;
-                int 21h;
-        
-        The preprocessor EscapeCode with default behavior will do the following replacements:
-        
-            # Heading
-        
-            Text that contains some <<escaped hash="2bb20aeb00314e915ecfefd86d26f46a"></escaped>.
-        
-            Below is a fence code block, language is optional:
-        
-            <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
-        
-            One more fence code block:
-        
-            <<escaped hash="91c3d3da865e24c33c4b366760c99579"></escaped>
-        
-            And this is a pre code block:
-        
-            <<escaped hash="a1e51c9ad3da841d393533f1522ab17e"></escaped>
-        
-        Escaped content parts will be saved into files located in the cache directory. The names of the files correspond the values of the `hash` attributes. For example, that’s the content of the file `15e1e46a75ef29eb760f392bb2df4ebb.md`:
-        
-            ```python
-            import this
-            ```
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![](https://img.shields.io/pypi/v/foliantcontrib.escapecode.svg)](https://pypi.org/project/foliantcontrib.escapecode/) [![](https://img.shields.io/github/v/tag/foliant-docs/foliantcontrib.escapecode.svg?label=GitHub)](https://github.com/foliant-docs/foliantcontrib.escapecode)
+
+# EscapeCode and UnescapeCode
+
+EscapeCode and UnescapeCode preprocessors work in pair.
+
+EscapeCode finds in the source Markdown content the parts that should not be modified by any next preprocessors. Examples of content that should be left raw: fence code blocks, pre code blocks, inline code.
+
+EscapeCode replaces these raw content parts with pseudo-XML tags recognized by UnescapeCode preprocessor.
+
+EscapeCode saves raw content parts into files. Later, UnescapeCode restores this content from files.
+
+Also, before the replacement, EscapeCode normalizes the source Markdown content to unify and simplify further operations. The preprocessor replaces `CRLF` with `LF`, removes excessive whitespace characters, provides trailing newline, etc.
+
+## Installation
+
+To install EscapeCode and UnescapeCode preprocessors, run:
+
+```bash
+$ pip install foliantcontrib.escapecode
+```
+
+See more details below.
+
+## Integration with Foliant and Includes
+
+You may call EscapeCode and UnescapeCode explicitly, but these preprocessors are integrated with Foliant core (since version 1.0.10) and with Includes preprocessor (since version 1.1.1).
+
+The `escape_code` project’s config option, if set to `true`, provides applying EscapeCode before all other preprocessors, and applying UnescapeCode after all other preprocessors. Also this option tells Includes preprocessor to apply EscapeCode to each included file.
+
+In this mode EscapeCode and UnescapeCode preprocessors deprecate _unescape preprocessor.
+
+    >    **Note**
+    >
+    >    The preprocessor _unescape is a part of Foliant core. It allows to use pseudo-XML tags in code examples. If you want an opening tag not to be interpreted by any preprocessor, precede this tag with the `<` character. The preprocessor _unescape applies after all other preprocessors and removes such characters.
+
+Config example:
+
+```yaml
+title: My Awesome Project
+
+chapters:
+    - index.md
+    ...
+
+escape_code: true
+
+preprocessors:
+    ...
+    - includes
+    ...
+...
+```
+
+If the `escape_code` option isn’t used or set to `false`, backward compatibility mode is involved. In this mode EscapeCode and UnescapeCode aren’t applied automatically, but _unescape preprocessor is applied.
+
+In more complicated case, you may pass some custom options to EscapeCode preprocessor:
+
+```
+escape_code:
+    options:
+        ...
+```
+
+Custom options available in EscapeCode since version 1.0.2. Foliant core supports passing custom options to EscapeCode preprocessor as the value of `escape_code.options` parameter since version 1.0.11. Options are described below.
+
+The Python package that includes EscapeCode and UnescapeCode preprocessors is the dependence of Includes preprocessor since version 1.1.1. At the same time this package isn’t a dependence of Foliant core. To use `escape_code` config option in Foliant core, you have to install the package with EscapeCode and UnescapeCode preprocessors separately.
+
+## Explicit Enabling
+
+You may not want to use the `escape_code` option and call the preprocessors explicitly:
+
+```yaml
+preprocessors:
+    - escapecode      # usually the first list item
+    ...
+    - unescapecode    # usually the last list item
+```
+
+Both preprocessors allow to override the path to the directory that is used to store temporary files:
+
+```yaml
+preprocessors:
+    - escapecode:
+        cache_dir: !path .escapecodecache
+    ...
+    - unescapecode:
+        cache_dir: !path .escapecodecache
+```
+
+The default values are shown in this example. EscapeCode and related UnescapeCode must work with the same cache directory.
+
+Note that if you use Includes preprocessor, and the included content doesn’t belong to the current Foliant project, there’s no way to escape raw parts of this content before Includes preprocessor is applied.
+
+## Config
+
+Since version 1.0.2, EscapeCode preprocessor supports the option `actions` in additional to `cache_dir`.
+
+The value of `actions` options should be a list of acceptable actions. By default, the following list is used:
+
+```yaml
+actions:
+    - normalize
+    - escape:
+        - fence_blocks
+        - pre_blocks
+        - inline_code
+```
+
+This default list may be overridden. For example:
+
+```yaml
+actions:
+    - normalize
+    - escape:
+        - fence_blocks
+        - inline_code
+        - tags:
+            - plantuml
+            - seqdiag
+        - comments
+    - pattern_override:
+        inline_code: '\<pattern_override_inline_code_\d+\>'
+```
+
+Meanings of parameters:
+
+* `normalize`—perform normalization;
+* `escape`—perform escaping of certain types of raw content:
+    * `fence_blocks`—fence code blocks;
+    * `pre_blocks`—pre code blocks;
+    * `inline_code`—inline code;
+    * `comments`—HTML-style comments, also usual for Markdown;
+    * `tags`—content of certain tags with the tags themselves, for example `plantuml` for `<plantuml>...</plantuml>`.
+* `pattern_override`—a regular expression that will not be escaped:
+    * `pre_blocks`—the lines of the pre code block containing this template will not be escaped;
+    * `inline_code`—pattern for inline code;
+    * `comments`—pattern for HTML-style comments, also usual for Markdown.
+
+## Usage
+
+Below you can see an example of Markdown content with code blocks and inline code.
+
+    # Heading
+
+    Text that contains some `inline code`. Text containing `<pattern_override_inline_code_01>`.
+
+    Below is a fence code block, language is optional:
+
+    ```python
+    import this
+    ```
+
+    One more fence code block:
+
+    ~~~
+    # This is a comment that should not be interpreted as a heading
+
+    print('Hello World')
+    ~~~
+
+    One more fence code block in list:
+
+    - first list item
+
+      ```python
+      import this
+      ```
+
+    - second list item
+
+    And this is a pre code block:
+
+        mov dx, hello;
+        mov ah, 9;
+        int 21h;
+
+The preprocessor EscapeCode with default behavior will do the following replacements:
+
+    # Heading
+
+    Text that contains some <<escaped hash="2bb20aeb00314e915ecfefd86d26f46a"></escaped>. Text containing `<pattern_override_inline_code_01>`.
+
+    Below is a fence code block, language is optional:
+
+    <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
+
+    One more fence code block:
+
+    <<escaped hash="91c3d3da865e24c33c4b366760c99579"></escaped>
+
+    One more fence code block in list:
+
+    - first list item
+
+      <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
+
+    - second list item
+
+    And this is a pre code block:
+
+        <<escaped hash="644952599350cd6676697cc95f52b999"></escaped>
+        <<escaped hash="e24afa46b55281fcf0b4b0e38d10419c"></escaped>
+        <<escaped hash="6bf655ac3a98b481ef3d33ac8dfcd93f"></escaped>
+
+Escaped content parts will be saved into files located in the cache directory. The names of the files correspond the values of the `hash` attributes. For example, that’s the content of the file `15e1e46a75ef29eb760f392bb2df4ebb.md`:
+
+    ```python
+    import this
+    ```
```

### Comparing `foliantcontrib.escapecode-1.0.4/README.md` & `foliantcontrib.escapecode-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -115,33 +115,39 @@
     - escape:
         - fence_blocks
         - inline_code
         - tags:
             - plantuml
             - seqdiag
         - comments
+    - pattern_override:
+        inline_code: '\<pattern_override_inline_code_\d+\>'
 ```
 
 Meanings of parameters:
 
 * `normalize`—perform normalization;
 * `escape`—perform escaping of certain types of raw content:
     * `fence_blocks`—fence code blocks;
     * `pre_blocks`—pre code blocks;
     * `inline_code`—inline code;
     * `comments`—HTML-style comments, also usual for Markdown;
-    * `tags`—content of certain tags with the tags themselves, for example `plantuml` for `<<plantuml>...</plantuml>`.
+    * `tags`—content of certain tags with the tags themselves, for example `plantuml` for `<plantuml>...</plantuml>`.
+* `pattern_override`—a regular expression that will not be escaped:
+    * `pre_blocks`—the lines of the pre code block containing this template will not be escaped;
+    * `inline_code`—pattern for inline code;
+    * `comments`—pattern for HTML-style comments, also usual for Markdown.
 
 ## Usage
 
 Below you can see an example of Markdown content with code blocks and inline code.
 
     # Heading
 
-    Text that contains some `inline code`.
+    Text that contains some `inline code`. Text containing `<pattern_override_inline_code_01>`.
 
     Below is a fence code block, language is optional:
 
     ```python
     import this
     ```
 
@@ -149,36 +155,56 @@
 
     ~~~
     # This is a comment that should not be interpreted as a heading
 
     print('Hello World')
     ~~~
 
+    One more fence code block in list:
+
+    - first list item
+
+      ```python
+      import this
+      ```
+
+    - second list item
+
     And this is a pre code block:
 
         mov dx, hello;
         mov ah, 9;
         int 21h;
 
 The preprocessor EscapeCode with default behavior will do the following replacements:
 
     # Heading
 
-    Text that contains some <<escaped hash="2bb20aeb00314e915ecfefd86d26f46a"></escaped>.
+    Text that contains some <<escaped hash="2bb20aeb00314e915ecfefd86d26f46a"></escaped>. Text containing `<pattern_override_inline_code_01>`.
 
     Below is a fence code block, language is optional:
 
     <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
 
     One more fence code block:
 
     <<escaped hash="91c3d3da865e24c33c4b366760c99579"></escaped>
 
+    One more fence code block in list:
+
+    - first list item
+
+      <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
+
+    - second list item
+
     And this is a pre code block:
 
-    <<escaped hash="a1e51c9ad3da841d393533f1522ab17e"></escaped>
+        <<escaped hash="644952599350cd6676697cc95f52b999"></escaped>
+        <<escaped hash="e24afa46b55281fcf0b4b0e38d10419c"></escaped>
+        <<escaped hash="6bf655ac3a98b481ef3d33ac8dfcd93f"></escaped>
 
 Escaped content parts will be saved into files located in the cache directory. The names of the files correspond the values of the `hash` attributes. For example, that’s the content of the file `15e1e46a75ef29eb760f392bb2df4ebb.md`:
 
     ```python
     import this
     ```
```

### Comparing `foliantcontrib.escapecode-1.0.4/setup.py` & `foliantcontrib.escapecode-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 
 
 setup(
     name='foliantcontrib.escapecode',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='1.0.4',
+    version='1.0.5',
     author='Artemy Lomov',
     author_email='artemy@lomov.ru',
     url='https://github.com/foliant-docs/foliantcontrib.escapecode',
     packages=['foliant.preprocessors'],
     license='MIT',
     platforms='any',
     install_requires=[
-        'foliant>=1.0.4'
+        'foliant>=1.0.4',
+        'marko==1.3.0'
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `foliantcontrib.escapecode-1.0.4/PKG-INFO` & `foliantcontrib.escapecode-1.0.5/foliantcontrib.escapecode.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,230 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.escapecode
-Version: 1.0.4
+Version: 1.0.5
 Summary: Preprocessor for Foliant to escape/unescape raw content.
 Home-page: https://github.com/foliant-docs/foliantcontrib.escapecode
 Author: Artemy Lomov
 Author-email: artemy@lomov.ru
 License: MIT
-Description: [![](https://img.shields.io/pypi/v/foliantcontrib.escapecode.svg)](https://pypi.org/project/foliantcontrib.escapecode/) [![](https://img.shields.io/github/v/tag/foliant-docs/foliantcontrib.escapecode.svg?label=GitHub)](https://github.com/foliant-docs/foliantcontrib.escapecode)
-        
-        # EscapeCode and UnescapeCode
-        
-        EscapeCode and UnescapeCode preprocessors work in pair.
-        
-        EscapeCode finds in the source Markdown content the parts that should not be modified by any next preprocessors. Examples of content that should be left raw: fence code blocks, pre code blocks, inline code.
-        
-        EscapeCode replaces these raw content parts with pseudo-XML tags recognized by UnescapeCode preprocessor.
-        
-        EscapeCode saves raw content parts into files. Later, UnescapeCode restores this content from files.
-        
-        Also, before the replacement, EscapeCode normalizes the source Markdown content to unify and simplify further operations. The preprocessor replaces `CRLF` with `LF`, removes excessive whitespace characters, provides trailing newline, etc.
-        
-        ## Installation
-        
-        To install EscapeCode and UnescapeCode preprocessors, run:
-        
-        ```bash
-        $ pip install foliantcontrib.escapecode
-        ```
-        
-        See more details below.
-        
-        ## Integration with Foliant and Includes
-        
-        You may call EscapeCode and UnescapeCode explicitly, but these preprocessors are integrated with Foliant core (since version 1.0.10) and with Includes preprocessor (since version 1.1.1).
-        
-        The `escape_code` project’s config option, if set to `true`, provides applying EscapeCode before all other preprocessors, and applying UnescapeCode after all other preprocessors. Also this option tells Includes preprocessor to apply EscapeCode to each included file.
-        
-        In this mode EscapeCode and UnescapeCode preprocessors deprecate _unescape preprocessor.
-        
-            >    **Note**
-            >
-            >    The preprocessor _unescape is a part of Foliant core. It allows to use pseudo-XML tags in code examples. If you want an opening tag not to be interpreted by any preprocessor, precede this tag with the `<` character. The preprocessor _unescape applies after all other preprocessors and removes such characters.
-        
-        Config example:
-        
-        ```yaml
-        title: My Awesome Project
-        
-        chapters:
-            - index.md
-            ...
-        
-        escape_code: true
-        
-        preprocessors:
-            ...
-            - includes
-            ...
-        ...
-        ```
-        
-        If the `escape_code` option isn’t used or set to `false`, backward compatibility mode is involved. In this mode EscapeCode and UnescapeCode aren’t applied automatically, but _unescape preprocessor is applied.
-        
-        In more complicated case, you may pass some custom options to EscapeCode preprocessor:
-        
-        ```
-        escape_code:
-            options:
-                ...
-        ```
-        
-        Custom options available in EscapeCode since version 1.0.2. Foliant core supports passing custom options to EscapeCode preprocessor as the value of `escape_code.options` parameter since version 1.0.11. Options are described below.
-        
-        The Python package that includes EscapeCode and UnescapeCode preprocessors is the dependence of Includes preprocessor since version 1.1.1. At the same time this package isn’t a dependence of Foliant core. To use `escape_code` config option in Foliant core, you have to install the package with EscapeCode and UnescapeCode preprocessors separately.
-        
-        ## Explicit Enabling
-        
-        You may not want to use the `escape_code` option and call the preprocessors explicitly:
-        
-        ```yaml
-        preprocessors:
-            - escapecode      # usually the first list item
-            ...
-            - unescapecode    # usually the last list item
-        ```
-        
-        Both preprocessors allow to override the path to the directory that is used to store temporary files:
-        
-        ```yaml
-        preprocessors:
-            - escapecode:
-                cache_dir: !path .escapecodecache
-            ...
-            - unescapecode:
-                cache_dir: !path .escapecodecache
-        ```
-        
-        The default values are shown in this example. EscapeCode and related UnescapeCode must work with the same cache directory.
-        
-        Note that if you use Includes preprocessor, and the included content doesn’t belong to the current Foliant project, there’s no way to escape raw parts of this content before Includes preprocessor is applied.
-        
-        ## Config
-        
-        Since version 1.0.2, EscapeCode preprocessor supports the option `actions` in additional to `cache_dir`.
-        
-        The value of `actions` options should be a list of acceptable actions. By default, the following list is used:
-        
-        ```yaml
-        actions:
-            - normalize
-            - escape:
-                - fence_blocks
-                - pre_blocks
-                - inline_code
-        ```
-        
-        This default list may be overridden. For example:
-        
-        ```yaml
-        actions:
-            - normalize
-            - escape:
-                - fence_blocks
-                - inline_code
-                - tags:
-                    - plantuml
-                    - seqdiag
-                - comments
-        ```
-        
-        Meanings of parameters:
-        
-        * `normalize`—perform normalization;
-        * `escape`—perform escaping of certain types of raw content:
-            * `fence_blocks`—fence code blocks;
-            * `pre_blocks`—pre code blocks;
-            * `inline_code`—inline code;
-            * `comments`—HTML-style comments, also usual for Markdown;
-            * `tags`—content of certain tags with the tags themselves, for example `plantuml` for `<<plantuml>...</plantuml>`.
-        
-        ## Usage
-        
-        Below you can see an example of Markdown content with code blocks and inline code.
-        
-            # Heading
-        
-            Text that contains some `inline code`.
-        
-            Below is a fence code block, language is optional:
-        
-            ```python
-            import this
-            ```
-        
-            One more fence code block:
-        
-            ~~~
-            # This is a comment that should not be interpreted as a heading
-        
-            print('Hello World')
-            ~~~
-        
-            And this is a pre code block:
-        
-                mov dx, hello;
-                mov ah, 9;
-                int 21h;
-        
-        The preprocessor EscapeCode with default behavior will do the following replacements:
-        
-            # Heading
-        
-            Text that contains some <<escaped hash="2bb20aeb00314e915ecfefd86d26f46a"></escaped>.
-        
-            Below is a fence code block, language is optional:
-        
-            <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
-        
-            One more fence code block:
-        
-            <<escaped hash="91c3d3da865e24c33c4b366760c99579"></escaped>
-        
-            And this is a pre code block:
-        
-            <<escaped hash="a1e51c9ad3da841d393533f1522ab17e"></escaped>
-        
-        Escaped content parts will be saved into files located in the cache directory. The names of the files correspond the values of the `hash` attributes. For example, that’s the content of the file `15e1e46a75ef29eb760f392bb2df4ebb.md`:
-        
-            ```python
-            import this
-            ```
-        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![](https://img.shields.io/pypi/v/foliantcontrib.escapecode.svg)](https://pypi.org/project/foliantcontrib.escapecode/) [![](https://img.shields.io/github/v/tag/foliant-docs/foliantcontrib.escapecode.svg?label=GitHub)](https://github.com/foliant-docs/foliantcontrib.escapecode)
+
+# EscapeCode and UnescapeCode
+
+EscapeCode and UnescapeCode preprocessors work in pair.
+
+EscapeCode finds in the source Markdown content the parts that should not be modified by any next preprocessors. Examples of content that should be left raw: fence code blocks, pre code blocks, inline code.
+
+EscapeCode replaces these raw content parts with pseudo-XML tags recognized by UnescapeCode preprocessor.
+
+EscapeCode saves raw content parts into files. Later, UnescapeCode restores this content from files.
+
+Also, before the replacement, EscapeCode normalizes the source Markdown content to unify and simplify further operations. The preprocessor replaces `CRLF` with `LF`, removes excessive whitespace characters, provides trailing newline, etc.
+
+## Installation
+
+To install EscapeCode and UnescapeCode preprocessors, run:
+
+```bash
+$ pip install foliantcontrib.escapecode
+```
+
+See more details below.
+
+## Integration with Foliant and Includes
+
+You may call EscapeCode and UnescapeCode explicitly, but these preprocessors are integrated with Foliant core (since version 1.0.10) and with Includes preprocessor (since version 1.1.1).
+
+The `escape_code` project’s config option, if set to `true`, provides applying EscapeCode before all other preprocessors, and applying UnescapeCode after all other preprocessors. Also this option tells Includes preprocessor to apply EscapeCode to each included file.
+
+In this mode EscapeCode and UnescapeCode preprocessors deprecate _unescape preprocessor.
+
+    >    **Note**
+    >
+    >    The preprocessor _unescape is a part of Foliant core. It allows to use pseudo-XML tags in code examples. If you want an opening tag not to be interpreted by any preprocessor, precede this tag with the `<` character. The preprocessor _unescape applies after all other preprocessors and removes such characters.
+
+Config example:
+
+```yaml
+title: My Awesome Project
+
+chapters:
+    - index.md
+    ...
+
+escape_code: true
+
+preprocessors:
+    ...
+    - includes
+    ...
+...
+```
+
+If the `escape_code` option isn’t used or set to `false`, backward compatibility mode is involved. In this mode EscapeCode and UnescapeCode aren’t applied automatically, but _unescape preprocessor is applied.
+
+In more complicated case, you may pass some custom options to EscapeCode preprocessor:
+
+```
+escape_code:
+    options:
+        ...
+```
+
+Custom options available in EscapeCode since version 1.0.2. Foliant core supports passing custom options to EscapeCode preprocessor as the value of `escape_code.options` parameter since version 1.0.11. Options are described below.
+
+The Python package that includes EscapeCode and UnescapeCode preprocessors is the dependence of Includes preprocessor since version 1.1.1. At the same time this package isn’t a dependence of Foliant core. To use `escape_code` config option in Foliant core, you have to install the package with EscapeCode and UnescapeCode preprocessors separately.
+
+## Explicit Enabling
+
+You may not want to use the `escape_code` option and call the preprocessors explicitly:
+
+```yaml
+preprocessors:
+    - escapecode      # usually the first list item
+    ...
+    - unescapecode    # usually the last list item
+```
+
+Both preprocessors allow to override the path to the directory that is used to store temporary files:
+
+```yaml
+preprocessors:
+    - escapecode:
+        cache_dir: !path .escapecodecache
+    ...
+    - unescapecode:
+        cache_dir: !path .escapecodecache
+```
+
+The default values are shown in this example. EscapeCode and related UnescapeCode must work with the same cache directory.
+
+Note that if you use Includes preprocessor, and the included content doesn’t belong to the current Foliant project, there’s no way to escape raw parts of this content before Includes preprocessor is applied.
+
+## Config
+
+Since version 1.0.2, EscapeCode preprocessor supports the option `actions` in additional to `cache_dir`.
+
+The value of `actions` options should be a list of acceptable actions. By default, the following list is used:
+
+```yaml
+actions:
+    - normalize
+    - escape:
+        - fence_blocks
+        - pre_blocks
+        - inline_code
+```
+
+This default list may be overridden. For example:
+
+```yaml
+actions:
+    - normalize
+    - escape:
+        - fence_blocks
+        - inline_code
+        - tags:
+            - plantuml
+            - seqdiag
+        - comments
+    - pattern_override:
+        inline_code: '\<pattern_override_inline_code_\d+\>'
+```
+
+Meanings of parameters:
+
+* `normalize`—perform normalization;
+* `escape`—perform escaping of certain types of raw content:
+    * `fence_blocks`—fence code blocks;
+    * `pre_blocks`—pre code blocks;
+    * `inline_code`—inline code;
+    * `comments`—HTML-style comments, also usual for Markdown;
+    * `tags`—content of certain tags with the tags themselves, for example `plantuml` for `<plantuml>...</plantuml>`.
+* `pattern_override`—a regular expression that will not be escaped:
+    * `pre_blocks`—the lines of the pre code block containing this template will not be escaped;
+    * `inline_code`—pattern for inline code;
+    * `comments`—pattern for HTML-style comments, also usual for Markdown.
+
+## Usage
+
+Below you can see an example of Markdown content with code blocks and inline code.
+
+    # Heading
+
+    Text that contains some `inline code`. Text containing `<pattern_override_inline_code_01>`.
+
+    Below is a fence code block, language is optional:
+
+    ```python
+    import this
+    ```
+
+    One more fence code block:
+
+    ~~~
+    # This is a comment that should not be interpreted as a heading
+
+    print('Hello World')
+    ~~~
+
+    One more fence code block in list:
+
+    - first list item
+
+      ```python
+      import this
+      ```
+
+    - second list item
+
+    And this is a pre code block:
+
+        mov dx, hello;
+        mov ah, 9;
+        int 21h;
+
+The preprocessor EscapeCode with default behavior will do the following replacements:
+
+    # Heading
+
+    Text that contains some <<escaped hash="2bb20aeb00314e915ecfefd86d26f46a"></escaped>. Text containing `<pattern_override_inline_code_01>`.
+
+    Below is a fence code block, language is optional:
+
+    <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
+
+    One more fence code block:
+
+    <<escaped hash="91c3d3da865e24c33c4b366760c99579"></escaped>
+
+    One more fence code block in list:
+
+    - first list item
+
+      <<escaped hash="15e1e46a75ef29eb760f392bb2df4ebb"></escaped>
+
+    - second list item
+
+    And this is a pre code block:
+
+        <<escaped hash="644952599350cd6676697cc95f52b999"></escaped>
+        <<escaped hash="e24afa46b55281fcf0b4b0e38d10419c"></escaped>
+        <<escaped hash="6bf655ac3a98b481ef3d33ac8dfcd93f"></escaped>
+
+Escaped content parts will be saved into files located in the cache directory. The names of the files correspond the values of the `hash` attributes. For example, that’s the content of the file `15e1e46a75ef29eb760f392bb2df4ebb.md`:
+
+    ```python
+    import this
+    ```
```

