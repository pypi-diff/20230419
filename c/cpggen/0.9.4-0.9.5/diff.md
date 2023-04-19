# Comparing `tmp/cpggen-0.9.4.tar.gz` & `tmp/cpggen-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.9.4.tar", max compression
+gzip compressed data, was "cpggen-0.9.5.tar", max compression
```

## Comparing `cpggen-0.9.4.tar` & `cpggen-0.9.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-17 10:17:36.727332 cpggen-0.9.4/LICENSE
--rw-r--r--   0        0        0     6972 2023-04-17 10:17:36.731332 cpggen-0.9.4/README.md
--rw-r--r--   0        0        0        0 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/__init__.py
--rw-r--r--   0        0        0    12908 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/cli.py
--rw-r--r--   0        0        0    30379 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/logger.py
--rw-r--r--   0        0        0    11089 2023-04-17 10:17:36.731332 cpggen-0.9.4/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-17 10:17:36.731332 cpggen-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     8300 1970-01-01 00:00:00.000000 cpggen-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 05:29:23.478079 cpggen-0.9.5/LICENSE
+-rw-r--r--   0        0        0     7201 2023-04-19 05:29:23.478079 cpggen-0.9.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/__init__.py
+-rw-r--r--   0        0        0    13069 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/cli.py
+-rw-r--r--   0        0        0    32803 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/logger.py
+-rw-r--r--   0        0        0    11089 2023-04-19 05:29:23.478079 cpggen-0.9.5/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-19 05:29:23.482079 cpggen-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     8529 1970-01-01 00:00:00.000000 cpggen-0.9.5/PKG-INFO
```

### Comparing `cpggen-0.9.4/LICENSE` & `cpggen-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.4/README.md` & `cpggen-0.9.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -52,26 +52,28 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.2/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.4/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.2/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.4/cpggen.exe
 .\cpggen.exe --help
 ```
 
+NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
+
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
 
 ```bash
 oras pull ghcr.io/appthreat/cpggen-bin:v1
 chmod +x cpggen-linux-amd64
```

### Comparing `cpggen-0.9.4/cpggen/cli.py` & `cpggen-0.9.5/cpggen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 
 import argparse
 import json
 import os
 import shutil
 import signal
 import tempfile
-from multiprocessing import Pool
+from multiprocessing import Pool, freeze_support
 from pathlib import Path, PurePath
 
 from quart import Quart, request
 
 from cpggen import executor, utils
 from cpggen.logger import LOG, console
 
 try:
     os.environ["PYTHONIOENCODING"] = "utf-8"
+    os.environ["PYTHONUTF8"] = 1
 except Exception:
     pass
 
 product_logo = """
  ██████╗██████╗  ██████╗
 ██╔════╝██╔══██╗██╔════╝
 ██║     ██████╔╝██║  ███╗
@@ -59,15 +60,20 @@
         default=False,
     )
     parser.add_argument(
         "--build",
         dest="auto_build",
         help="Attempt to build the project automatically",
         action="store_true",
-        default=True if os.getenv("AUTO_BUILD") in ("true", "1") else False,
+        default=True
+        if (
+            os.getenv("AUTO_BUILD") in ("true", "1")
+            or os.getenv("SHIFTLEFT_ACCESS_TOKEN")
+        )
+        else False,
     )
     parser.add_argument(
         "--joern-home",
         dest="joern_home",
         help="Joern installation directory",
         default=os.getenv(
             "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
@@ -380,8 +386,9 @@
             shutil.rmtree(src)
         except Exception:
             # Ignore cleanup errors
             pass
 
 
 if __name__ == "__main__":
+    freeze_support()
     main()
```

### Comparing `cpggen-0.9.4/cpggen/executor.py` & `cpggen-0.9.5/cpggen/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 )
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
 cpu_count = str(psutil.cpu_count())
 
+bin_ext = ".bat" if sys.platform == "win32" else ".sh"
+use_shell = True if sys.platform == "win32" else False
+
 
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except Exception:
         base_path = os.path.dirname(__file__)
     return os.path.join(base_path, relative_path)
@@ -43,41 +46,56 @@
 cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
 local_bin_dir = resource_path("local_bin")
 if os.path.exists(local_bin_dir):
     csharp2cpg_bundled = resource_path(
         os.path.join("local_bin", "joern-cli", "csharp2cpg.zip")
     )
     joern_bundled = resource_path(os.path.join("local_bin", "joern-cli.zip"))
-    if os.path.exists(csharp2cpg_bundled):
-        with zipfile.ZipFile(csharp2cpg_bundled, "r") as zip_ref:
-            zip_ref.extractall(local_bin_dir)
-            os.symlink(
-                os.path.join(local_bin_dir, "bin", "csharp2cpg"),
-                os.path.join(local_bin_dir, "joern-cli", "csharp2cpg"),
+    if os.path.exists(csharp2cpg_bundled) and not os.path.exists(
+        os.path.join(local_bin_dir, "bin", "csharp2cpg")
+    ):
+        try:
+            with zipfile.ZipFile(csharp2cpg_bundled, "r") as zip_ref:
+                zip_ref.extractall(local_bin_dir)
+                if not os.path.exists(
+                    os.path.join(local_bin_dir, "joern-cli", "csharp2cpg")
+                ):
+                    os.symlink(
+                        os.path.join(local_bin_dir, "bin", "csharp2cpg"),
+                        os.path.join(local_bin_dir, "joern-cli", "csharp2cpg"),
+                    )
+        except Exception as e:
+            LOG.info(
+                "cpggen was prevented from extracting the csharp2cpg frontend.\nPlease check if your terminal has administrative privileges or if the antivirus is preventing this process.\nAlternatively, use container-based execution."
             )
-    if os.path.exists(joern_bundled):
-        with zipfile.ZipFile(joern_bundled, "r") as zip_ref:
-            zip_ref.extractall(local_bin_dir)
-            try:
+            LOG.error(e)
+    if os.path.exists(joern_bundled) and not os.path.exists(
+        os.path.join(local_bin_dir, "joern-cli")
+    ):
+        try:
+            with zipfile.ZipFile(joern_bundled, "r") as zip_ref:
+                zip_ref.extractall(local_bin_dir)
                 # Add execute permissions
                 for dirname, subdirs, files in os.walk(local_bin_dir):
                     for filename in files:
                         if not filename.endswith(".jar") and (
-                            filename.endswith(".sh")
+                            filename.endswith("%(bin_ext)s")
                             or "2cpg" in filename
                             or "joern-" in filename
                         ):
                             os.chmod(os.path.join(dirname, filename), 0o755)
                 LOG.debug(f"Extracted {joern_bundled}")
                 os.environ["JOERN_HOME"] = os.path.join(local_bin_dir, "joern-cli")
                 os.environ["CPGGEN_BIN_DIR"] = local_bin_dir
                 os.environ["PATH"] += os.sep + os.environ["JOERN_HOME"] + os.sep
-            except Exception:
-                # Ignore errors
-                pass
+        except Exception as e:
+            LOG.info(
+                "cpggen was prevented from extracting the joern library.\nPlease check if your terminal has administrative privileges or if the antivirus is preventing this process.\nAlternatively, use container-based execution."
+            )
+            LOG.error(e)
     if not shutil.which(cdxgen_cmd):
         local_cdxgen_cmd = resource_path(
             os.path.join(
                 "local_bin", "cdxgen.exe" if sys.platform == "win32" else "cdxgen"
             )
         )
         if os.path.exists(local_cdxgen_cmd):
@@ -100,27 +118,27 @@
             value = default_value
         return value
     except Exception:
         return default_value
 
 
 cpg_tools_map = {
-    "c": "%(joern_home)sc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
-    "cpp": "%(joern_home)sc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
+    "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
+    "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "java": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
     "binary": "%(joern_home)sghidra2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "js": "%(joern_home)sjssrc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "ts": "%(joern_home)sjssrc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "python": "%(joern_home)spysrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
-    "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --collect-js-files %(src)s --ignore-errors --no-log-file --ignore-tests -l error",
-    "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --collect-js-files %(src)s --ignore-errors --no-log-file --ignore-tests -l error",
+    "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
+    "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
     "go": "%(joern_home)sgo2cpg generate -o %(cpg_out)s ./...",
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
@@ -185,15 +203,17 @@
         LOG.info(f"Submitting {app_manifest['app']} for Qwiet.AI analysis")
         build_args = cpg_tools_map["qwiet"]
         policy = ""
         vcs_correction = ""
         if os.getenv("SHIFTLEFT_POLICY"):
             policy = f"""--policy {os.getenv("SHIFTLEFT_POLICY")} """
         elif os.getenv("ENABLE_BEST_PRACTICES") in ("true", "1"):
-            policy = """--policy io.shiftleft/defaultWithDictAndBestPractices """
+            policy = (
+                """--policy io%(bin_ext)siftleft/defaultWithDictAndBestPractices """
+            )
 
         if app_manifest.get("tool_lang"):
             if "jar" in app_manifest.get("tool_lang") or "jsp" in app_manifest.get(
                 "tool_lang"
             ):
                 vcs_correction = '--vcs-prefix-correction "*=src/main/java" '
             if "scala" in app_manifest.get("tool_lang"):
@@ -205,15 +225,15 @@
         cp = subprocess.run(
             build_args.split(" "),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
             env=env,
             check=False,
-            shell=False,
+            shell=use_shell,
             encoding="utf-8",
         )
         if cp:
             if LOG.isEnabledFor(DEBUG) and cp.stdout:
                 LOG.debug(cp.stdout)
             if cp.returncode and cp.stderr:
                 LOG.info(cp.stderr)
@@ -234,22 +254,22 @@
                 subprocess.run(
                     convert_cmd_with_args.split(" "),
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     cwd=export_out_dir,
                     env=env,
                     check=False,
-                    shell=False,
+                    shell=use_shell,
                     encoding="utf-8",
                 )
             except Exception as e:
                 LOG.debug(e)
     else:
         LOG.debug(
-            f"Install graphviz package and ensure the command `dot` is available in the PATH to convert to png automatically"
+            "Install graphviz package and ensure the command `dot` is available in the PATH to convert to png automatically"
         )
 
 
 def do_x_build(src, env, build_artefacts, tool_lang):
     tool_lang = tool_lang.split("-")[0]
     build_crashes = {}
     for k, v in build_artefacts.items():
@@ -284,30 +304,37 @@
                     except Exception:
                         # Ignore errors
                         pass
                 build_args_str = build_args_str % dict(
                     gradle_cmd=gradle_cmd, maven_cmd=maven_cmd
                 )
             try:
-                LOG.debug(f"Executing {build_args_str} in {base_dir}")
+                LOG.debug(f"Executing build command: {build_args_str} in {base_dir}")
                 cp = subprocess.run(
                     build_args_str.split(" "),
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     cwd=base_dir,
                     env=env,
                     check=False,
-                    shell=False,
+                    shell=use_shell,
                     encoding="utf-8",
                 )
-                if cp and LOG.isEnabledFor(DEBUG) and cp.returncode and cp.stderr:
-                    LOG.debug(cp.stderr)
+                if cp:
+                    # These languages always need troubleshooting
+                    if tool_lang in ("csharp", "dotnet", "go"):
+                        if cp.stderr:
+                            LOG.info(cp.stderr)
+                        if cp.stdout:
+                            LOG.info(cp.stdout)
+                    elif LOG.isEnabledFor(DEBUG) and cp.returncode and cp.stderr:
+                        LOG.debug(cp.stderr)
                     failed_modules = failed_modules + 1
             except Exception as e:
-                LOG.debug(e)
+                LOG.info(e)
                 crashed_modules = crashed_modules + 1
         build_crashes[k] = {
             "failed_modules": failed_modules,
             "crashed_modules": crashed_modules,
         }
     return build_crashes
 
@@ -337,14 +364,18 @@
         "make": find_makefiles(src),
     }
     return do_x_build(src, env, build_artefacts, "go")
 
 
 def do_build(tool_lang, src, cwd, env):
     if tool_lang in ("csharp",):
+        if os.path.exists(os.path.join(src, "global.json")):
+            LOG.debug(
+                "global.json is found in the root directory. Ensure the correct version of dotnet sdk is installed.\nAlternatively, set the rollForward property to latestMajor to use the bundled .Net 7 SDK from the cpggen container image."
+            )
         return do_x_build(src, env, {"csharp": find_csharp_artifacts(src)}, "csharp")
     elif (
         tool_lang in ("jar", "scala")
         or tool_lang.startswith("jar")
         or tool_lang.startswith("jsp")
     ):
         return do_jar_build(tool_lang, src, env)
@@ -397,18 +428,27 @@
                 total=100,
                 start=False,
             )
             cmd_with_args = cpg_tools_map.get(tool_lang)
             if not cmd_with_args:
                 return
             # Perform build first
-            if auto_build:
-                LOG.info(
-                    f"Automatically building {src}. To speed up this step, cache the build dependencies using the CI cache settings."
-                )
+            if auto_build or build_tools_map.get(tool_lang):
+                if os.getenv("CI"):
+                    LOG.info(
+                        f"Automatically building {src} for {tool_lang}. To speed up this step, cache the build dependencies using the CI cache settings."
+                    )
+                elif use_container:
+                    LOG.info(
+                        f"Attempting to build {src} for {tool_lang} using the bundled build tools from the container image."
+                    )
+                else:
+                    LOG.info(
+                        f"Attempting to build {src} for {tool_lang} using the locally available build tools.\nFor better results, please ensure the correct version of these tools are installed for your application.\nAlternatively, use container image based execution."
+                    )
                 lang_build_crashes[tool_lang] = do_build(tool_lang, src, cwd, env)
             uber_jar = ""
             csharp_artifacts = ""
             # For languages like scala, jsp or jar we need to create a uber jar containing all jar, war files from the source directory
             if "uber_jar" in cmd_with_args:
                 stdout = subprocess.PIPE
                 java_artifacts = find_java_artifacts(src)
@@ -472,14 +512,15 @@
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
+                    bin_ext=bin_ext,
                     **extra_args,
                 )
                 sbom_lang = tool_lang
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
@@ -516,15 +557,15 @@
                         cp = subprocess.run(
                             cmd_list_with_args,
                             stdout=stdout,
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
-                            shell=False,
+                            shell=use_shell,
                             encoding="utf-8",
                         )
                         if cp and cp.returncode and cp.stderr:
                             LOG.warn(f"Export CPG has failed for {src}")
                             if not os.getenv("AT_DEBUG_MODE"):
                                 LOG.info(
                                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
@@ -586,15 +627,15 @@
                         cp = subprocess.run(
                             sbom_cmd_list_with_args,
                             stdout=stdout,
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
-                            shell=False,
+                            shell=use_shell,
                             encoding="utf-8",
                         )
                         if cp and LOG.isEnabledFor(DEBUG):
                             if cp.stdout:
                                 LOG.debug(cp.stdout)
                             if cp.stderr:
                                 LOG.debug(cp.stderr)
@@ -607,25 +648,25 @@
                 cp = subprocess.run(
                     cmd_list_with_args,
                     stdout=stdout,
                     stderr=stderr,
                     cwd=cwd,
                     env=env,
                     check=False,
-                    shell=False,
+                    shell=use_shell,
                     encoding="utf-8",
                 )
                 if cp and stdout == subprocess.PIPE:
                     for line in cp.stdout:
                         progress.update(task, completed=5)
-                if cp and LOG.isEnabledFor(DEBUG) and cp.returncode:
+                if cp and cp.returncode:
                     if cp.stdout:
-                        LOG.debug(cp.stdout)
+                        LOG.info(cp.stdout)
                     if cp.stderr:
-                        LOG.debug(cp.stderr)
+                        LOG.info(cp.stderr)
                 if os.path.exists(cpg_out):
                     # go2cpg seems to produce a cpg without read permissions
                     try:
                         os.chmod(cpg_out, 0o644)
                     except Exception:
                         # Ignore errors
                         pass
```

### Comparing `cpggen-0.9.4/cpggen/logger.py` & `cpggen-0.9.5/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.4/cpggen/utils.py` & `cpggen-0.9.5/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.4/pyproject.toml` & `cpggen-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.9.4"
+version = "0.9.5"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.9.4/PKG-INFO` & `cpggen-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.9.4
+Version: 0.9.5
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -84,26 +84,28 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.2/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.4/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.2/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.4/cpggen.exe
 .\cpggen.exe --help
 ```
 
+NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
+
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
 
 ```bash
 oras pull ghcr.io/appthreat/cpggen-bin:v1
 chmod +x cpggen-linux-amd64
```

