# Comparing `tmp/rubbrband-0.1.8.tar.gz` & `tmp/rubbrband-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.1.8.tar", last modified: Wed Feb 22 01:47:22 2023, max compression
+gzip compressed data, was "rubbrband-0.1.9.tar", last modified: Thu Feb 23 01:33:12 2023, max compression
```

## Comparing `rubbrband-0.1.8.tar` & `rubbrband-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.166745 rubbrband-0.1.8/
--rw-r--r--   0 llewyn     (501) staff       (20)       36 2023-02-21 21:59:17.000000 rubbrband-0.1.8/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)       53 2023-02-22 01:47:22.166833 rubbrband-0.1.8/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)        6 2023-02-17 20:36:16.000000 rubbrband-0.1.8/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)      126 2023-02-20 21:41:06.000000 rubbrband-0.1.8/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.163355 rubbrband-0.1.8/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)     6413 2023-02-22 01:02:49.000000 rubbrband-0.1.8/rubbrband/cli.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.162310 rubbrband-0.1.8/rubbrband/models/
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.164703 rubbrband-0.1.8/rubbrband/models/ControlNet/
--rw-r--r--   0 llewyn     (501) staff       (20)     2071 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/ControlNet/Dockerfile
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.164966 rubbrband-0.1.8/rubbrband/models/ControlNet/library-scripts/
--rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/ControlNet/library-scripts/common-debian.sh
--rw-r--r--   0 llewyn     (501) staff       (20)      403 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/ControlNet/train.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.165281 rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/
--rw-r--r--   0 llewyn     (501) staff       (20)     4751 2023-02-22 01:46:32.000000 rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/Dockerfile
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.165431 rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/
--rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/common-debian.sh
--rw-r--r--   0 llewyn     (501) staff       (20)     1648 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/train.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.166236 rubbrband-0.1.8/rubbrband/models/LoRA/
--rw-r--r--   0 llewyn     (501) staff       (20)     1886 2023-02-22 01:13:57.000000 rubbrband-0.1.8/rubbrband/models/LoRA/Dockerfile
--rw-r--r--   0 llewyn     (501) staff       (20)       75 2023-02-22 00:58:07.000000 rubbrband-0.1.8/rubbrband/models/LoRA/infer.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.166516 rubbrband-0.1.8/rubbrband/models/LoRA/library-scripts/
--rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/LoRA/library-scripts/common-debian.sh
--rw-r--r--   0 llewyn     (501) staff       (20)      961 2023-02-22 00:59:05.000000 rubbrband-0.1.8/rubbrband/models/LoRA/library-scripts/infer.py
--rwxr-xr-x   0 llewyn     (501) staff       (20)      824 2023-02-20 19:35:42.000000 rubbrband-0.1.8/rubbrband/models/LoRA/train.sh
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-22 01:47:22.164328 rubbrband-0.1.8/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)       53 2023-02-22 01:47:22.000000 rubbrband-0.1.8/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      794 2023-02-22 01:47:22.000000 rubbrband-0.1.8/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-02-22 01:47:22.000000 rubbrband-0.1.8/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       49 2023-02-22 01:47:22.000000 rubbrband-0.1.8/rubbrband.egg-info/entry_points.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       27 2023-02-22 01:47:22.000000 rubbrband-0.1.8/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-02-22 01:47:22.000000 rubbrband-0.1.8/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      240 2023-02-22 01:47:22.167113 rubbrband-0.1.8/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-02-21 22:05:53.000000 rubbrband-0.1.8/setup.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.395436 rubbrband-0.1.9/
+-rw-r--r--   0 llewyn     (501) staff       (20)       36 2023-02-21 21:59:17.000000 rubbrband-0.1.9/MANIFEST.in
+-rw-r--r--   0 llewyn     (501) staff       (20)       53 2023-02-23 01:33:12.395485 rubbrband-0.1.9/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)        6 2023-02-17 20:36:16.000000 rubbrband-0.1.9/README.md
+-rw-r--r--   0 llewyn     (501) staff       (20)      126 2023-02-20 21:41:06.000000 rubbrband-0.1.9/pyproject.toml
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.393328 rubbrband-0.1.9/rubbrband/
+-rw-r--r--   0 llewyn     (501) staff       (20)     6658 2023-02-23 01:20:10.000000 rubbrband-0.1.9/rubbrband/cli.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.392605 rubbrband-0.1.9/rubbrband/models/
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394217 rubbrband-0.1.9/rubbrband/models/ControlNet/
+-rw-r--r--   0 llewyn     (501) staff       (20)     2071 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/ControlNet/Dockerfile
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394331 rubbrband-0.1.9/rubbrband/models/ControlNet/library-scripts/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/ControlNet/library-scripts/common-debian.sh
+-rw-r--r--   0 llewyn     (501) staff       (20)      429 2023-02-22 18:14:48.000000 rubbrband-0.1.9/rubbrband/models/ControlNet/train.sh
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394674 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/
+-rw-r--r--   0 llewyn     (501) staff       (20)     4750 2023-02-22 18:15:02.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/Dockerfile
+-rw-r--r--   0 llewyn     (501) staff       (20)      762 2023-02-23 01:07:27.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/infer.sh
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.394783 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/common-debian.sh
+-rw-r--r--   0 llewyn     (501) staff       (20)     2130 2023-02-23 01:07:27.000000 rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/train.sh
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.395120 rubbrband-0.1.9/rubbrband/models/LoRA/
+-rw-r--r--   0 llewyn     (501) staff       (20)     1886 2023-02-22 18:14:48.000000 rubbrband-0.1.9/rubbrband/models/LoRA/Dockerfile
+-rwxr-xr-x   0 llewyn     (501) staff       (20)       74 2023-02-23 01:20:39.000000 rubbrband-0.1.9/rubbrband/models/LoRA/infer.sh
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.395339 rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11000 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/common-debian.sh
+-rw-r--r--   0 llewyn     (501) staff       (20)      951 2023-02-23 01:21:11.000000 rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/infer.py
+-rwxr-xr-x   0 llewyn     (501) staff       (20)      824 2023-02-20 19:35:42.000000 rubbrband-0.1.9/rubbrband/models/LoRA/train.sh
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-02-23 01:33:12.393992 rubbrband-0.1.9/rubbrband.egg-info/
+-rw-r--r--   0 llewyn     (501) staff       (20)       53 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)      848 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       49 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/entry_points.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       27 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-02-23 01:33:12.000000 rubbrband-0.1.9/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)      240 2023-02-23 01:33:12.395699 rubbrband-0.1.9/setup.cfg
+-rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-02-21 22:05:53.000000 rubbrband-0.1.9/setup.py
```

### Comparing `rubbrband-0.1.8/rubbrband/cli.py` & `rubbrband-0.1.9/rubbrband/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,30 @@
 
     subprocess.run(["docker", "exec", "-it", container_name, "/bin/bash"])
 
 
 # '''name''' corresponds to the name column in db.csv
 # the option '''-d''' or '''--dataset_dir''' is the path to the dataset directory
 # this directory gets mounted to the container at /home/engineering/data
-@main.command()
+@main.command(
+    context_settings=dict(
+        ignore_unknown_options=True,
+        allow_extra_args=True,
+    )
+)
 @click.argument("model")
 @click.option(
     "-d",
     "--dataset_dir",
+    prompt="Path to dataset directory",
     type=click.Path(exists=True),
     help="Path to the local dataset directory that is mounted to the container at /home/engineering/data.",
 )
-def train(model, dataset_dir):
+@click.pass_context
+def train(ctx, model, dataset_dir):
     """
     Train a MODEL.
 
     MODEL is the name of the model to train. \n
     --dataset_dir is the local path that gets mounted to the container at /home/engineering/data.
 
     Example: rubbrband train --dataset_dir /my_data ControlNet
@@ -185,15 +192,17 @@
     if container.status != "running":
         container.start()
 
     this_dir = os.path.dirname(os.path.abspath(__file__))
 
     with yaspin():
         subprocess.run(["chmod", "a+x", f"{this_dir}/models/{model}/train.sh"])
-        subprocess.run(["/bin/bash", "-c", f"{this_dir}/models/{model}/train.sh"])
+        # ctx.args is a list of arguments passed to the train command
+        subprocess.run(["/bin/bash", f"{this_dir}/models/{model}/train.sh"] + ctx.args)
+
 
 @main.command()
 @click.argument("model")
 @click.argument("prompt")
 def infer(model, prompt):
     model_name = model.lower()
     container = client.containers.get(f"rb-{model_name}")
@@ -202,18 +211,19 @@
         container.start()
 
     this_dir = os.path.dirname(os.path.abspath(__file__))
 
     with yaspin():
         subprocess.run(["chmod", "a+x", f"{this_dir}/models/{model}/infer.sh"])
         # add a parameter for prompt
-        subprocess.run(["/bin/bash", "-c", f"{this_dir}/models/{model}/infer.sh", prompt])
+        subprocess.run(["/bin/bash", f"{this_dir}/models/{model}/infer.sh", f"'{prompt}'"])
 
         # move file from docker container to local directory
         # the file is located at /home/engineering/samples/output.jpg
         # the file is moved to the current directory
         subprocess.run(["docker", "cp", f"rb-{model_name}:/home/engineering/samples/output.jpg", "."])
 
     click.echo("Inference complete. Check the current directory for the output image.")
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `rubbrband-0.1.8/rubbrband/models/ControlNet/Dockerfile` & `rubbrband-0.1.9/rubbrband/models/ControlNet/Dockerfile`

 * *Files identical despite different names*

### Comparing `rubbrband-0.1.8/rubbrband/models/ControlNet/library-scripts/common-debian.sh` & `rubbrband-0.1.9/rubbrband/models/ControlNet/library-scripts/common-debian.sh`

 * *Files identical despite different names*

### Comparing `rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/Dockerfile` & `rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     echo "conda activate base" >> ~/.bashrc && \
     find ${CONDA_INSTALL_PATH}/ -follow -type f -name '*.a' -delete && \
     find ${CONDA_INSTALL_PATH}/ -follow -type f -name '*.js.map' -delete && \
     ${CONDA_INSTALL_PATH}/bin/conda clean -a -f -y
 
 WORKDIR /home/engineering
 RUN sudo ln -fs /usr/share/zoneinfo/America/New_York /etc/localtime
-RUN git clone --depth 1 https://github.com/XavierXiao/Dreambooth-Stable-Diffusion.git
+RUN git clone --depth 1 https://github.com/rubbrband/Dreambooth-Stable-Diffusion.git
 WORKDIR /home/engineering/Dreambooth-Stable-Diffusion
 RUN sudo apt-get update 
 RUN conda config --append channels pytorch 
 RUN conda config --append channels defaults 
 RUN (conda install python=3.8.10 || echo conda install failed)
 RUN (conda install pip=20.3 || echo conda install failed)
 RUN (conda install cudatoolkit=11.3 || echo conda install failed)
```

### Comparing `rubbrband-0.1.8/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/common-debian.sh` & `rubbrband-0.1.9/rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/common-debian.sh`

 * *Files identical despite different names*

### Comparing `rubbrband-0.1.8/rubbrband/models/LoRA/Dockerfile` & `rubbrband-0.1.9/rubbrband/models/LoRA/Dockerfile`

 * *Files identical despite different names*

### Comparing `rubbrband-0.1.8/rubbrband/models/LoRA/library-scripts/common-debian.sh` & `rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/common-debian.sh`

 * *Files identical despite different names*

### Comparing `rubbrband-0.1.8/rubbrband/models/LoRA/library-scripts/infer.py` & `rubbrband-0.1.9/rubbrband/models/LoRA/library-scripts/infer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from diffusers import StableDiffusionPipeline, EulerAncestralDiscreteScheduler
-from lora_diffusion import tune_lora_scale, patch_pipe
 import torch
+from diffusers import EulerAncestralDiscreteScheduler, StableDiffusionPipeline
+from lora_diffusion import patch_pipe, tune_lora_scale
+
 
 def infer(prompt):
     model_id = "runwayml/stable-diffusion-v1-5"
 
-    pipe = StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16).to(
-        "cuda"
-    )
+    pipe = StableDiffusionPipeline.from_pretrained(model_id, torch_dtype=torch.float16).to("cuda")
     pipe.scheduler = EulerAncestralDiscreteScheduler.from_config(pipe.scheduler.config)
 
     patch_pipe(
         pipe,
         "/home/engineering/output/final_lora.safetensors",
         patch_text=True,
         patch_ti=True,
@@ -22,13 +21,15 @@
     tune_lora_scale(pipe.text_encoder, 1.00)
 
     torch.manual_seed(0)
     image = pipe(prompt, num_inference_steps=50, guidance_scale=7).images[0]
     image.save("/home/engineering/samples/output.jpg")
     image
 
+
 if __name__ == "__main__":
     # get arguments from command line
     import sys
+
     prompt = sys.argv[1]
 
-    infer(prompt)
+    infer(prompt)
```

### Comparing `rubbrband-0.1.8/rubbrband/models/LoRA/train.sh` & `rubbrband-0.1.9/rubbrband/models/LoRA/train.sh`

 * *Files identical despite different names*

### Comparing `rubbrband-0.1.8/rubbrband.egg-info/SOURCES.txt` & `rubbrband-0.1.9/rubbrband.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 rubbrband.egg-info/entry_points.txt
 rubbrband.egg-info/requires.txt
 rubbrband.egg-info/top_level.txt
 rubbrband/models/ControlNet/Dockerfile
 rubbrband/models/ControlNet/train.sh
 rubbrband/models/ControlNet/library-scripts/common-debian.sh
 rubbrband/models/Dreambooth-Stable-Diffusion/Dockerfile
+rubbrband/models/Dreambooth-Stable-Diffusion/infer.sh
 rubbrband/models/Dreambooth-Stable-Diffusion/train.sh
 rubbrband/models/Dreambooth-Stable-Diffusion/library-scripts/common-debian.sh
 rubbrband/models/LoRA/Dockerfile
 rubbrband/models/LoRA/infer.sh
 rubbrband/models/LoRA/train.sh
 rubbrband/models/LoRA/library-scripts/common-debian.sh
 rubbrband/models/LoRA/library-scripts/infer.py
```

