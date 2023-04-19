# Comparing `tmp/alphamed-federated-0.4.6.tar.gz` & `tmp/alphamed-federated-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphamed-federated-0.4.6.tar", last modified: Thu Apr 13 12:01:16 2023, max compression
+gzip compressed data, was "alphamed-federated-0.4.7.tar", last modified: Wed Apr 19 06:56:20 2023, max compression
```

## Comparing `alphamed-federated-0.4.6.tar` & `alphamed-federated-0.4.7.tar`

### file list

```diff
@@ -1,215 +1,220 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.250101 alphamed-federated-0.4.6/
--rw-rw-rw-   0        0        0    11357 2023-03-29 15:01:00.000000 alphamed-federated-0.4.6/LICENSE
--rw-rw-rw-   0        0        0    17211 2023-04-13 12:01:16.250101 alphamed-federated-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     3447 2023-03-29 15:01:00.000000 alphamed-federated-0.4.6/README.md
--rw-rw-rw-   0        0        0      945 2023-04-13 12:00:37.000000 alphamed-federated-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 12:01:16.251099 alphamed-federated-0.4.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.919175 alphamed-federated-0.4.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.938176 alphamed-federated-0.4.6/src/alphafed/
--rw-rw-rw-   0        0        0      121 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.945173 alphamed-federated-0.4.6/src/alphafed/auto_ml/
--rw-rw-rw-   0        0        0      180 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/auto_ml/__init__.py
--rw-rw-rw-   0        0        0    14678 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/auto_ml/auto_model.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.950174 alphamed-federated-0.4.6/src/alphafed/auto_ml/cvat/
--rw-rw-rw-   0        0        0        0 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/auto_ml/cvat/__init__.py
--rw-rw-rw-   0        0        0     3578 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/auto_ml/cvat/annotation.py
--rw-rw-rw-   0        0        0      116 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/auto_ml/exceptions.py
--rw-rw-rw-   0        0        0     5758 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/auto_ml/pretrained.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.964172 alphamed-federated-0.4.6/src/alphafed/contractor/
--rw-rw-rw-   0        0        0      116 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/contractor/__init__.py
--rw-rw-rw-   0        0        0     4717 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/contractor/common.py
--rw-rw-rw-   0        0        0     9772 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/contractor/task_contractor.py
--rw-rw-rw-   0        0        0    25099 2023-04-13 03:25:38.000000 alphamed-federated-0.4.6/src/alphafed/contractor/task_message_contractor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.999691 alphamed-federated-0.4.6/src/alphafed/data_channel/
--rw-rw-rw-   0        0        0      125 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/data_channel/__init__.py
--rw-rw-rw-   0        0        0     6048 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/data_channel/data_channel.py
--rw-rw-rw-   0        0        0     2105 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/data_channel/data_channel_pb2.py
--rw-rw-rw-   0        0        0     2534 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/data_channel/data_channel_pb2_grpc.py
--rw-rw-rw-   0        0        0    17562 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/data_channel/grpc_data_channel.py
--rw-rw-rw-   0        0        0    11060 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/data_channel/shared_file_data_channel.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.889093 alphamed-federated-0.4.6/src/alphafed/docs/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.886093 alphamed-federated-0.4.6/src/alphafed/docs/auto_ml/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.002685 alphamed-federated-0.4.6/src/alphafed/docs/auto_ml/res/
--rw-rw-rw-   0        0        0    27911 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/docs/auto_ml/res/auto.py
--rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/docs/auto_ml/res/res_net.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.007686 alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/
--rw-rw-rw-   0        0        0     6225 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/contractor.py
--rw-rw-rw-   0        0        0    18538 2023-04-12 12:57:03.000000 alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/scheduler.py
--rw-rw-rw-   0        0        0     5049 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/simple_task.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.009686 alphamed-federated-0.4.6/src/alphafed/docs/fed_avg/
--rw-rw-rw-   0        0        0      782 2023-03-29 15:01:29.000000 alphamed-federated-0.4.6/src/alphafed/docs/fed_avg/net.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.018179 alphamed-federated-0.4.6/src/alphafed/docs/mock/
--rw-rw-rw-   0        0        0      782 2023-03-29 15:01:30.000000 alphamed-federated-0.4.6/src/alphafed/docs/mock/net.py
--rw-rw-rw-   0        0        0     5008 2023-03-29 15:01:30.000000 alphamed-federated-0.4.6/src/alphafed/docs/mock/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:15.889093 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.020180 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.023179 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_fed_avg/
--rw-rw-rw-   0        0        0    23001 2023-03-29 15:01:30.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py
--rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:30.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.026189 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_local/
--rw-rw-rw-   0        0        0    21045 2023-03-29 15:01:31.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_local/auto.py
--rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:31.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py
--rw-rw-rw-   0        0        0     1481 2023-03-29 15:01:30.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/cnn_net.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.029569 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/simple_fed_avg/
--rw-rw-rw-   0        0        0     3039 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py
--rw-rw-rw-   0        0        0    12837 2023-04-12 12:49:52.000000 alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.031987 alphamed-federated-0.4.6/src/alphafed/examples/
--rw-rw-rw-   0        0        0        0 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.032985 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/
--rw-rw-rw-   0        0        0        0 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.041984 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/
--rw-rw-rw-   0        0        0      732 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py
--rw-rw-rw-   0        0        0      541 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.045410 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/
--rw-rw-rw-   0        0        0    28837 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py
--rw-rw-rw-   0        0        0    15644 2023-03-29 15:03:27.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.049422 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_local/
--rw-rw-rw-   0        0        0    27956 2023-04-07 07:21:53.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py
--rw-rw-rw-   0        0        0    15644 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py
--rw-rw-rw-   0        0        0     1348 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py
--rw-rw-rw-   0        0        0     1308 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py
--rw-rw-rw-   0        0        0     1308 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py
--rw-rw-rw-   0        0        0     1041 2023-03-29 15:03:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.059418 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/
--rw-rw-rw-   0        0        0      732 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py
--rw-rw-rw-   0        0        0      533 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.061421 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/
--rw-rw-rw-   0        0        0    30857 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.067766 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/
--rw-rw-rw-   0        0        0       41 2023-03-29 15:03:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/__init__.py
--rw-rw-rw-   0        0        0    14317 2023-03-29 15:03:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.071774 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/
--rw-rw-rw-   0        0        0        0 2023-03-29 15:03:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/__init__.py
--rw-rw-rw-   0        0        0    22522 2023-03-29 15:03:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py
--rw-rw-rw-   0        0        0    12274 2023-03-29 15:03:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.073774 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/
--rw-rw-rw-   0        0        0    29972 2023-03-29 15:03:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.078842 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/
--rw-rw-rw-   0        0        0       41 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/__init__.py
--rw-rw-rw-   0        0        0    14317 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.081851 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/
--rw-rw-rw-   0        0        0        0 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/__init__.py
--rw-rw-rw-   0        0        0    22522 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py
--rw-rw-rw-   0        0        0    12274 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py
--rw-rw-rw-   0        0        0     1354 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py
--rw-rw-rw-   0        0        0     1314 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py
--rw-rw-rw-   0        0        0     1314 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py
--rw-rw-rw-   0        0        0     1043 2023-03-29 15:03:29.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.090937 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/
--rw-rw-rw-   0        0        0      732 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py
--rw-rw-rw-   0        0        0      533 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.093944 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/
--rw-rw-rw-   0        0        0    27957 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py
--rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.099437 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/
--rw-rw-rw-   0        0        0    27051 2023-03-29 15:03:34.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py
--rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:34.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py
--rw-rw-rw-   0        0        0     1388 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py
--rw-rw-rw-   0        0        0     1292 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py
--rw-rw-rw-   0        0        0     1292 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py
--rw-rw-rw-   0        0        0     1096 2023-03-29 15:03:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.108436 alphamed-federated-0.4.6/src/alphafed/examples/data_channel/
--rw-rw-rw-   0        0        0      578 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/data_channel/__init__.py
--rw-rw-rw-   0        0        0      497 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/data_channel/clean_history_msg.py
--rw-rw-rw-   0        0        0     4544 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/data_channel/run_receiver_2.py
--rw-rw-rw-   0        0        0     3866 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/data_channel/run_receiver_4.py
--rw-rw-rw-   0        0        0     6242 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/data_channel/run_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.122593 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/
--rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/__init__.py
--rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/clean_history_msg.py
--rw-rw-rw-   0        0        0    23586 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/demo_FedIRM.py
--rw-rw-rw-   0        0        0    20482 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/demos.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.125592 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/model/
--rw-rw-rw-   0        0        0     5021 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/model/my_scheduler.py
--rw-rw-rw-   0        0        0      782 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/model/net.py
--rw-rw-rw-   0        0        0     1265 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_aggregator.py
--rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_2.py
--rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_3.py
--rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_4.py
--rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_5.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.134909 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/
--rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/__init__.py
--rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/clean_history_msg.py
--rw-rw-rw-   0        0        0     7556 2023-04-13 06:17:28.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/demos.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.142231 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/
--rw-rw-rw-   0        0        0    10630 2023-04-12 09:11:34.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/contractor.py
--rw-rw-rw-   0        0        0      384 2023-04-12 09:11:32.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/loss.py
--rw-rw-rw-   0        0        0     6818 2023-04-12 09:48:27.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/my_homo_fed_md_impl.py
--rw-rw-rw-   0        0        0      782 2023-04-12 09:11:31.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/net.py
--rw-rw-rw-   0        0        0    31535 2023-04-13 06:16:45.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/scheduler.py
--rw-rw-rw-   0        0        0      514 2023-04-13 06:17:45.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/run_aggregator.py
--rw-rw-rw-   0        0        0      499 2023-04-13 06:17:54.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/run_data_owner_2.py
--rw-rw-rw-   0        0        0      499 2023-04-13 06:18:22.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_md/run_data_owner_4.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.150548 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/
--rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/__init__.py
--rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/clean_history_msg.py
--rw-rw-rw-   0        0        0     5747 2023-04-13 06:05:41.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/demos.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.155939 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/
--rw-rw-rw-   0        0        0     1420 2023-04-11 09:28:02.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/contractor.py
--rw-rw-rw-   0        0        0     5033 2023-04-12 04:47:33.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/my_homo_fed_per_impl.py
--rw-rw-rw-   0        0        0      939 2023-04-11 09:28:02.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/net.py
--rw-rw-rw-   0        0        0    11157 2023-04-13 06:00:22.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/scheduler.py
--rw-rw-rw-   0        0        0      516 2023-04-13 05:55:12.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/run_aggregator.py
--rw-rw-rw-   0        0        0      501 2023-04-13 06:06:23.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/run_data_owner_2.py
--rw-rw-rw-   0        0        0      501 2023-04-13 06:06:34.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_per/run_data_owner_4.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.165189 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/
--rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/__init__.py
--rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/clean_history_msg.py
--rw-rw-rw-   0        0        0     5870 2023-04-13 05:44:09.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/demos.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.169594 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/
--rw-rw-rw-   0        0        0     5124 2023-04-11 08:25:09.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/my_fed_prox_impl.py
--rw-rw-rw-   0        0        0      782 2023-04-10 09:03:18.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/net.py
--rw-rw-rw-   0        0        0     2425 2023-04-10 09:03:17.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/scheduler.py
--rw-rw-rw-   0        0        0      518 2023-04-13 05:55:53.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/run_aggregator.py
--rw-rw-rw-   0        0        0      503 2023-04-13 05:55:51.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/run_data_owner_2.py
--rw-rw-rw-   0        0        0      503 2023-04-13 05:55:48.000000 alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/run_data_owner_4.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.176599 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/
--rw-rw-rw-   0        0        0      389 2023-04-13 04:20:24.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/__init__.py
--rw-rw-rw-   0        0        0      494 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/clean_history_msg.py
--rw-rw-rw-   0        0        0    23092 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/demos.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.188500 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/
--rw-rw-rw-   0        0        0      592 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/demos.py
--rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py
--rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py
--rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py
--rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py
--rw-rw-rw-   0        0        0     1046 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_initiator.py
--rw-rw-rw-   0        0        0     1218 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/run_collaborater.py
--rw-rw-rw-   0        0        0     1117 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/run_host.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.198501 alphamed-federated-0.4.6/src/alphafed/fed_avg/
--rw-rw-rw-   0        0        0      103 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/__init__.py
--rw-rw-rw-   0        0        0     9619 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/contractor.py
--rw-rw-rw-   0        0        0     2026 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/dp_contractor.py
--rw-rw-rw-   0        0        0     8964 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/dp_fed_avg.py
--rw-rw-rw-   0        0        0    33004 2023-04-12 12:58:20.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/fed_avg.py
--rw-rw-rw-   0        0        0    10441 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/secure_contractor.py
--rw-rw-rw-   0        0        0    34059 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/fed_avg/secure_fed_avg.py
--rw-rw-rw-   0        0        0     1827 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/fs.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.206503 alphamed-federated-0.4.6/src/alphafed/hetero_nn/
--rw-rw-rw-   0        0        0      116 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/__init__.py
--rw-rw-rw-   0        0        0    12136 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/contractor.py
--rw-rw-rw-   0        0        0    49980 2023-04-13 11:32:01.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/hetero_nn.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.211501 alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/
--rw-rw-rw-   0        0        0      105 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/__init__.py
--rw-rw-rw-   0        0        0     3489 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/psi.py
--rw-rw-rw-   0        0        0    14497 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/rsa_intersecter.py
--rw-rw-rw-   0        0        0     3753 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py
--rw-rw-rw-   0        0        0    14008 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/secure_contractor.py
--rw-rw-rw-   0        0        0    74408 2023-04-13 11:32:21.000000 alphamed-federated-0.4.6/src/alphafed/hetero_nn/secure_hetero_nn.py
--rw-rw-rw-   0        0        0      741 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/loggers.py
--rw-rw-rw-   0        0        0     6428 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/mock.py
--rw-rw-rw-   0        0        0     5037 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/perf_bench.py
--rw-rw-rw-   0        0        0     6441 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.221810 alphamed-federated-0.4.6/src/alphafed/secure/
--rw-rw-rw-   0        0        0       59 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/secure/__init__.py
--rw-rw-rw-   0        0        0      685 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/secure/aes.py
--rw-rw-rw-   0        0        0     1242 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/secure/ecdhe.py
--rw-rw-rw-   0        0        0     2602 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/secure/shamir.py
--rw-rw-rw-   0        0        0      621 2023-03-29 15:03:36.000000 alphamed-federated-0.4.6/src/alphafed/secure/tools.py
--rw-rw-rw-   0        0        0     1864 2023-03-29 15:01:28.000000 alphamed-federated-0.4.6/src/alphafed/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:01:16.248099 alphamed-federated-0.4.6/src/alphamed_federated.egg-info/
--rw-rw-rw-   0        0        0    17211 2023-04-13 12:01:15.000000 alphamed-federated-0.4.6/src/alphamed_federated.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8530 2023-04-13 12:01:15.000000 alphamed-federated-0.4.6/src/alphamed_federated.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:01:15.000000 alphamed-federated-0.4.6/src/alphamed_federated.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-04-13 12:01:15.000000 alphamed-federated-0.4.6/src/alphamed_federated.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 12:01:15.000000 alphamed-federated-0.4.6/src/alphamed_federated.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.374245 alphamed-federated-0.4.7/
+-rw-rw-rw-   0        0        0    11357 2023-03-29 15:01:00.000000 alphamed-federated-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0    17211 2023-04-19 06:56:20.372245 alphamed-federated-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3447 2023-03-29 15:01:00.000000 alphamed-federated-0.4.7/README.md
+-rw-rw-rw-   0        0        0      945 2023-04-19 06:55:26.000000 alphamed-federated-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 06:56:20.374245 alphamed-federated-0.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:19.987835 alphamed-federated-0.4.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.007298 alphamed-federated-0.4.7/src/alphafed/
+-rw-rw-rw-   0        0        0      121 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.016238 alphamed-federated-0.4.7/src/alphafed/auto_ml/
+-rw-rw-rw-   0        0        0      180 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/auto_ml/__init__.py
+-rw-rw-rw-   0        0        0    14678 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/auto_ml/auto_model.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.019645 alphamed-federated-0.4.7/src/alphafed/auto_ml/cvat/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/auto_ml/cvat/__init__.py
+-rw-rw-rw-   0        0        0     3578 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/auto_ml/cvat/annotation.py
+-rw-rw-rw-   0        0        0      116 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/auto_ml/exceptions.py
+-rw-rw-rw-   0        0        0     5758 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/auto_ml/pretrained.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.028038 alphamed-federated-0.4.7/src/alphafed/contractor/
+-rw-rw-rw-   0        0        0      116 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/contractor/__init__.py
+-rw-rw-rw-   0        0        0     4717 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/contractor/common.py
+-rw-rw-rw-   0        0        0     9772 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/contractor/task_contractor.py
+-rw-rw-rw-   0        0        0    25099 2023-04-13 03:25:38.000000 alphamed-federated-0.4.7/src/alphafed/contractor/task_message_contractor.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.040226 alphamed-federated-0.4.7/src/alphafed/data_channel/
+-rw-rw-rw-   0        0        0      125 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/data_channel/__init__.py
+-rw-rw-rw-   0        0        0     6048 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/data_channel/data_channel.py
+-rw-rw-rw-   0        0        0     2105 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/data_channel/data_channel_pb2.py
+-rw-rw-rw-   0        0        0     2534 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/data_channel/data_channel_pb2_grpc.py
+-rw-rw-rw-   0        0        0    17562 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/data_channel/grpc_data_channel.py
+-rw-rw-rw-   0        0        0    11060 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/data_channel/shared_file_data_channel.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:19.950163 alphamed-federated-0.4.7/src/alphafed/docs/
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:19.944162 alphamed-federated-0.4.7/src/alphafed/docs/auto_ml/
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.044228 alphamed-federated-0.4.7/src/alphafed/docs/auto_ml/res/
+-rw-rw-rw-   0        0        0    27911 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/docs/auto_ml/res/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/docs/auto_ml/res/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.052610 alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/
+-rw-rw-rw-   0        0        0     6225 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/contractor.py
+-rw-rw-rw-   0        0        0    18538 2023-04-12 12:57:03.000000 alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/scheduler.py
+-rw-rw-rw-   0        0        0     5049 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/simple_task.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.055124 alphamed-federated-0.4.7/src/alphafed/docs/fed_avg/
+-rw-rw-rw-   0        0        0      782 2023-03-29 15:01:29.000000 alphamed-federated-0.4.7/src/alphafed/docs/fed_avg/net.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.059124 alphamed-federated-0.4.7/src/alphafed/docs/mock/
+-rw-rw-rw-   0        0        0      782 2023-03-29 15:01:30.000000 alphamed-federated-0.4.7/src/alphafed/docs/mock/net.py
+-rw-rw-rw-   0        0        0     5008 2023-03-29 15:01:30.000000 alphamed-federated-0.4.7/src/alphafed/docs/mock/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:19.950163 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.061761 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.065773 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_fed_avg/
+-rw-rw-rw-   0        0        0    23001 2023-03-29 15:01:30.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:30.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.069783 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_local/
+-rw-rw-rw-   0        0        0    21045 2023-03-29 15:01:31.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_local/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:01:31.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py
+-rw-rw-rw-   0        0        0     1481 2023-03-29 15:01:30.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/cnn_net.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.072771 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/simple_fed_avg/
+-rw-rw-rw-   0        0        0     3039 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py
+-rw-rw-rw-   0        0        0    12837 2023-04-12 12:49:52.000000 alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.073913 alphamed-federated-0.4.7/src/alphafed/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.075923 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.089321 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/
+-rw-rw-rw-   0        0        0      732 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.094645 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/
+-rw-rw-rw-   0        0        0    28837 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py
+-rw-rw-rw-   0        0        0    15644 2023-03-29 15:03:27.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.099146 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_local/
+-rw-rw-rw-   0        0        0    27956 2023-04-07 07:21:53.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py
+-rw-rw-rw-   0        0        0    15644 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py
+-rw-rw-rw-   0        0        0     1348 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py
+-rw-rw-rw-   0        0        0     1308 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1308 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1041 2023-03-29 15:03:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.113911 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/
+-rw-rw-rw-   0        0        0      732 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.115910 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/
+-rw-rw-rw-   0        0        0    30857 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.121175 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/
+-rw-rw-rw-   0        0        0       41 2023-03-29 15:03:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/__init__.py
+-rw-rw-rw-   0        0        0    14317 2023-03-29 15:03:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.125176 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/__init__.py
+-rw-rw-rw-   0        0        0    22522 2023-03-29 15:03:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py
+-rw-rw-rw-   0        0        0    12274 2023-03-29 15:03:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.128636 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/
+-rw-rw-rw-   0        0        0    29972 2023-03-29 15:03:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.133890 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/
+-rw-rw-rw-   0        0        0       41 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/__init__.py
+-rw-rw-rw-   0        0        0    14317 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.138495 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/
+-rw-rw-rw-   0        0        0        0 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/__init__.py
+-rw-rw-rw-   0        0        0    22522 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py
+-rw-rw-rw-   0        0        0    12274 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py
+-rw-rw-rw-   0        0        0     1354 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py
+-rw-rw-rw-   0        0        0     1314 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1314 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1043 2023-03-29 15:03:29.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.155338 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/
+-rw-rw-rw-   0        0        0      732 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.159777 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/
+-rw-rw-rw-   0        0        0    27957 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.163790 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/
+-rw-rw-rw-   0        0        0    27051 2023-03-29 15:03:34.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:34.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py
+-rw-rw-rw-   0        0        0     1388 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py
+-rw-rw-rw-   0        0        0     1292 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1292 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1096 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.173543 alphamed-federated-0.4.7/src/alphafed/examples/data_channel/
+-rw-rw-rw-   0        0        0      578 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/data_channel/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/data_channel/clean_history_msg.py
+-rw-rw-rw-   0        0        0     4544 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/data_channel/run_receiver_2.py
+-rw-rw-rw-   0        0        0     3866 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/data_channel/run_receiver_4.py
+-rw-rw-rw-   0        0        0     6242 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/data_channel/run_sender.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.195758 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/clean_history_msg.py
+-rw-rw-rw-   0        0        0    23586 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/demo_FedIRM.py
+-rw-rw-rw-   0        0        0    20482 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.199766 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/model/
+-rw-rw-rw-   0        0        0     5021 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/model/my_scheduler.py
+-rw-rw-rw-   0        0        0      782 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/model/net.py
+-rw-rw-rw-   0        0        0     1265 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_aggregator.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_2.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_3.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_4.py
+-rw-rw-rw-   0        0        0     1030 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_5.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.211553 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/clean_history_msg.py
+-rw-rw-rw-   0        0        0     7556 2023-04-13 06:17:28.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.222087 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/
+-rw-rw-rw-   0        0        0    10630 2023-04-12 09:11:34.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/contractor.py
+-rw-rw-rw-   0        0        0      384 2023-04-12 09:11:32.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/loss.py
+-rw-rw-rw-   0        0        0     6818 2023-04-12 09:48:27.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/my_homo_fed_md_impl.py
+-rw-rw-rw-   0        0        0      782 2023-04-12 09:11:31.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/net.py
+-rw-rw-rw-   0        0        0    31535 2023-04-13 06:16:45.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/scheduler.py
+-rw-rw-rw-   0        0        0      514 2023-04-13 06:17:45.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/run_aggregator.py
+-rw-rw-rw-   0        0        0      499 2023-04-13 06:17:54.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/run_data_owner_2.py
+-rw-rw-rw-   0        0        0      499 2023-04-13 06:18:22.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_md/run_data_owner_4.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.234094 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/clean_history_msg.py
+-rw-rw-rw-   0        0        0     5747 2023-04-13 06:05:41.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.243097 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/
+-rw-rw-rw-   0        0        0     1420 2023-04-11 09:28:02.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/contractor.py
+-rw-rw-rw-   0        0        0     5033 2023-04-12 04:47:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/my_homo_fed_per_impl.py
+-rw-rw-rw-   0        0        0      939 2023-04-11 09:28:02.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/net.py
+-rw-rw-rw-   0        0        0    11157 2023-04-13 06:00:22.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/scheduler.py
+-rw-rw-rw-   0        0        0      516 2023-04-13 05:55:12.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/run_aggregator.py
+-rw-rw-rw-   0        0        0      501 2023-04-13 06:06:23.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/run_data_owner_2.py
+-rw-rw-rw-   0        0        0      501 2023-04-13 06:06:34.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_per/run_data_owner_4.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.256404 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/
+-rw-rw-rw-   0        0        0      736 2023-04-13 02:23:18.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/__init__.py
+-rw-rw-rw-   0        0        0      492 2023-03-29 15:03:35.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/clean_history_msg.py
+-rw-rw-rw-   0        0        0     5870 2023-04-13 05:44:09.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.262406 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/
+-rw-rw-rw-   0        0        0     5124 2023-04-11 08:25:09.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/my_fed_prox_impl.py
+-rw-rw-rw-   0        0        0      782 2023-04-10 09:03:18.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/net.py
+-rw-rw-rw-   0        0        0     2425 2023-04-10 09:03:17.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/scheduler.py
+-rw-rw-rw-   0        0        0      518 2023-04-13 05:55:53.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/run_aggregator.py
+-rw-rw-rw-   0        0        0      503 2023-04-13 05:55:51.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/run_data_owner_2.py
+-rw-rw-rw-   0        0        0      503 2023-04-13 05:55:48.000000 alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/run_data_owner_4.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.272161 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/
+-rw-rw-rw-   0        0        0      389 2023-04-13 04:20:24.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/clean_history_msg.py
+-rw-rw-rw-   0        0        0    23092 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/demos.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.281161 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/hetero_fed_irm/
+-rw-rw-rw-   0        0        0     7185 2023-04-19 06:15:52.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/hetero_fed_irm/collaborator_scheduler.py
+-rw-rw-rw-   0        0        0      524 2023-04-19 05:59:20.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/hetero_fed_irm/data_checker.py
+-rw-rw-rw-   0        0        0    11895 2023-04-19 06:24:40.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/hetero_fed_irm/host_scheduler.py
+-rw-rw-rw-   0        0        0    11996 2023-03-29 15:03:33.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/hetero_fed_irm/res_net.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.293422 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/
+-rw-rw-rw-   0        0        0      592 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/demos.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py
+-rw-rw-rw-   0        0        0      819 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py
+-rw-rw-rw-   0        0        0     1046 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_initiator.py
+-rw-rw-rw-   0        0        0     1218 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/run_collaborater.py
+-rw-rw-rw-   0        0        0     1117 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/run_host.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.307079 alphamed-federated-0.4.7/src/alphafed/fed_avg/
+-rw-rw-rw-   0        0        0      103 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/__init__.py
+-rw-rw-rw-   0        0        0     9619 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/contractor.py
+-rw-rw-rw-   0        0        0     2026 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/dp_contractor.py
+-rw-rw-rw-   0        0        0     8964 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/dp_fed_avg.py
+-rw-rw-rw-   0        0        0    33004 2023-04-12 12:58:20.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/fed_avg.py
+-rw-rw-rw-   0        0        0    10441 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/secure_contractor.py
+-rw-rw-rw-   0        0        0    34059 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/fed_avg/secure_fed_avg.py
+-rw-rw-rw-   0        0        0     1827 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/fs.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.319247 alphamed-federated-0.4.7/src/alphafed/hetero_nn/
+-rw-rw-rw-   0        0        0      116 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/__init__.py
+-rw-rw-rw-   0        0        0    12136 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/contractor.py
+-rw-rw-rw-   0        0        0    49995 2023-04-19 06:54:23.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/hetero_nn.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.325247 alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/
+-rw-rw-rw-   0        0        0      105 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/__init__.py
+-rw-rw-rw-   0        0        0     3489 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/psi.py
+-rw-rw-rw-   0        0        0    14497 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/rsa_intersecter.py
+-rw-rw-rw-   0        0        0     3753 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py
+-rw-rw-rw-   0        0        0    14008 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/secure_contractor.py
+-rw-rw-rw-   0        0        0    74408 2023-04-13 11:32:21.000000 alphamed-federated-0.4.7/src/alphafed/hetero_nn/secure_hetero_nn.py
+-rw-rw-rw-   0        0        0      741 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/loggers.py
+-rw-rw-rw-   0        0        0     6428 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/mock.py
+-rw-rw-rw-   0        0        0     5037 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/perf_bench.py
+-rw-rw-rw-   0        0        0     6441 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.335531 alphamed-federated-0.4.7/src/alphafed/secure/
+-rw-rw-rw-   0        0        0       59 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/secure/__init__.py
+-rw-rw-rw-   0        0        0      685 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/secure/aes.py
+-rw-rw-rw-   0        0        0     1242 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/secure/ecdhe.py
+-rw-rw-rw-   0        0        0     2602 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/secure/shamir.py
+-rw-rw-rw-   0        0        0      621 2023-03-29 15:03:36.000000 alphamed-federated-0.4.7/src/alphafed/secure/tools.py
+-rw-rw-rw-   0        0        0     1864 2023-03-29 15:01:28.000000 alphamed-federated-0.4.7/src/alphafed/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:56:20.368240 alphamed-federated-0.4.7/src/alphamed_federated.egg-info/
+-rw-rw-rw-   0        0        0    17211 2023-04-19 06:56:19.000000 alphamed-federated-0.4.7/src/alphamed_federated.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8789 2023-04-19 06:56:19.000000 alphamed-federated-0.4.7/src/alphamed_federated.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:56:19.000000 alphamed-federated-0.4.7/src/alphamed_federated.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-04-19 06:56:19.000000 alphamed-federated-0.4.7/src/alphamed_federated.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 06:56:19.000000 alphamed-federated-0.4.7/src/alphamed_federated.egg-info/top_level.txt
```

### Comparing `alphamed-federated-0.4.6/LICENSE` & `alphamed-federated-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/PKG-INFO` & `alphamed-federated-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphamed-federated
-Version: 0.4.6
+Version: 0.4.7
 Summary: AlphaMed Federated Learning Module
 Author-email: Huang Yi Chun <huangyichun@jinghang.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `alphamed-federated-0.4.6/README.md` & `alphamed-federated-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/pyproject.toml` & `alphamed-federated-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphamed-federated"
-version = "0.4.6"
+version = "0.4.7"
 dependencies = [
     "cloudpickle==2.0.0",
     "grpcio==1.47.0",
     "protobuf==3.20.0",
     "pycryptodomex==3.15.0",
     "requests==2.28.1",
     "torch==1.11.0",
```

### Comparing `alphamed-federated-0.4.6/src/alphafed/auto_ml/auto_model.py` & `alphamed-federated-0.4.7/src/alphafed/auto_ml/auto_model.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/auto_ml/cvat/annotation.py` & `alphamed-federated-0.4.7/src/alphafed/auto_ml/cvat/annotation.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/auto_ml/pretrained.py` & `alphamed-federated-0.4.7/src/alphafed/auto_ml/pretrained.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/contractor/common.py` & `alphamed-federated-0.4.7/src/alphafed/contractor/common.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/contractor/task_contractor.py` & `alphamed-federated-0.4.7/src/alphafed/contractor/task_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/contractor/task_message_contractor.py` & `alphamed-federated-0.4.7/src/alphafed/contractor/task_message_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/data_channel/data_channel.py` & `alphamed-federated-0.4.7/src/alphafed/data_channel/data_channel.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/data_channel/data_channel_pb2.py` & `alphamed-federated-0.4.7/src/alphafed/data_channel/data_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/data_channel/data_channel_pb2_grpc.py` & `alphamed-federated-0.4.7/src/alphafed/data_channel/data_channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/data_channel/grpc_data_channel.py` & `alphamed-federated-0.4.7/src/alphafed/data_channel/grpc_data_channel.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/data_channel/shared_file_data_channel.py` & `alphamed-federated-0.4.7/src/alphafed/data_channel/shared_file_data_channel.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/auto_ml/res/auto.py` & `alphamed-federated-0.4.7/src/alphafed/docs/auto_ml/res/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/auto_ml/res/res_net.py` & `alphamed-federated-0.4.7/src/alphafed/docs/auto_ml/res/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/contractor.py` & `alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/customized_scheduler/simple_task.py` & `alphamed-federated-0.4.7/src/alphafed/docs/customized_scheduler/simple_task.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/fed_avg/net.py` & `alphamed-federated-0.4.7/src/alphafed/docs/fed_avg/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/mock/net.py` & `alphamed-federated-0.4.7/src/alphafed/docs/mock/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/mock/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/docs/mock/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_fed_avg/auto_fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_fed_avg/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_local/auto.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/auto_model_local/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/cnn_net.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/cnn_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/simple_fed_avg/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/docs/tutorial/res/simple_fed_avg/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/clean_history_msg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_fed_avg/inception3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/res_local/inception3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/breast_density_classification/run_local.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/clean_history_msg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/convolutions.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/cv/senet.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_fed_avg/senet/layer_factories.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/convolutions.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/cv/senet.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/res_local/senet/layer_factories.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/endoscopic_inbody_classification/run_local.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/clean_history_msg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_fed_avg/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/auto.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/res_local/res_net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py` & `alphamed-federated-0.4.7/src/alphafed/examples/auto_ml/skin_lesion_diagnosis/run_local.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/data_channel/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/data_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/data_channel/run_receiver_2.py` & `alphamed-federated-0.4.7/src/alphafed/examples/data_channel/run_receiver_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/data_channel/run_receiver_4.py` & `alphamed-federated-0.4.7/src/alphafed/examples/data_channel/run_receiver_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/data_channel/run_sender.py` & `alphamed-federated-0.4.7/src/alphafed/examples/data_channel/run_sender.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/demo_FedIRM.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/demo_FedIRM.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/demos.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/model/my_scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/model/my_scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/model/net.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/model/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_2.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_3.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_4.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_avg/run_data_owner_5.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_avg/run_data_owner_5.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/demos.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/contractor.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/my_homo_fed_md_impl.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/my_homo_fed_md_impl.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/net.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/model/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/model/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_md/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_md/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/demos.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/contractor.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/my_homo_fed_per_impl.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/my_homo_fed_per_impl.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/net.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/model/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/model/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_per/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_per/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/__init__.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/demos.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/my_fed_prox_impl.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/my_fed_prox_impl.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/net.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/net.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/model/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/model/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/fed_prox/run_aggregator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/fed_prox/run_aggregator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/demos.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/demos.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/demos.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/psi/run_initiator.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/psi/run_initiator.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/run_collaborater.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/run_collaborater.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/examples/hetero_nn/run_host.py` & `alphamed-federated-0.4.7/src/alphafed/examples/hetero_nn/run_host.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fed_avg/contractor.py` & `alphamed-federated-0.4.7/src/alphafed/fed_avg/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fed_avg/dp_contractor.py` & `alphamed-federated-0.4.7/src/alphafed/fed_avg/dp_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fed_avg/dp_fed_avg.py` & `alphamed-federated-0.4.7/src/alphafed/fed_avg/dp_fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fed_avg/fed_avg.py` & `alphamed-federated-0.4.7/src/alphafed/fed_avg/fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fed_avg/secure_contractor.py` & `alphamed-federated-0.4.7/src/alphafed/fed_avg/secure_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fed_avg/secure_fed_avg.py` & `alphamed-federated-0.4.7/src/alphafed/fed_avg/secure_fed_avg.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/fs.py` & `alphamed-federated-0.4.7/src/alphafed/fs.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/contractor.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/hetero_nn.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/hetero_nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1165,15 +1165,15 @@
     def _close_task(self, is_succ: bool = True):
         """Close the task and upload the final parameters."""
         self.push_log(f'Closing task {self.task_id} ...')
 
         self._switch_status(self._FINISHING)
         if is_succ:
             model_file_path = self._prepare_task_output()
-            self.contractor.upload_metric_report(receivers=[self.id])
+            self.contractor.upload_metric_report(receivers=self.contractor.EVERYONE)
             self.contractor.upload_model(receivers=[self.id],
                                          model_file=model_file_path)
             self.contractor.notify_collaborator_complete(peer_id=self.id, host=self.host)
             self.push_log(f'Task {self.task_id} complete. Byebye!')
         else:
             self.push_log(f'Task {self.task_id} failed. Byebye!')
```

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/psi.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/psi.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/rsa_intersecter.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/rsa_intersecter.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/psi/rsa_psi_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/secure_contractor.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/secure_contractor.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/hetero_nn/secure_hetero_nn.py` & `alphamed-federated-0.4.7/src/alphafed/hetero_nn/secure_hetero_nn.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/loggers.py` & `alphamed-federated-0.4.7/src/alphafed/loggers.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/mock.py` & `alphamed-federated-0.4.7/src/alphafed/mock.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/perf_bench.py` & `alphamed-federated-0.4.7/src/alphafed/perf_bench.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/scheduler.py` & `alphamed-federated-0.4.7/src/alphafed/scheduler.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/secure/aes.py` & `alphamed-federated-0.4.7/src/alphafed/secure/aes.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/secure/ecdhe.py` & `alphamed-federated-0.4.7/src/alphafed/secure/ecdhe.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/secure/shamir.py` & `alphamed-federated-0.4.7/src/alphafed/secure/shamir.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/secure/tools.py` & `alphamed-federated-0.4.7/src/alphafed/secure/tools.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphafed/utils.py` & `alphamed-federated-0.4.7/src/alphafed/utils.py`

 * *Files identical despite different names*

### Comparing `alphamed-federated-0.4.6/src/alphamed_federated.egg-info/PKG-INFO` & `alphamed-federated-0.4.7/src/alphamed_federated.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphamed-federated
-Version: 0.4.6
+Version: 0.4.7
 Summary: AlphaMed Federated Learning Module
 Author-email: Huang Yi Chun <huangyichun@jinghang.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `alphamed-federated-0.4.6/src/alphamed_federated.egg-info/SOURCES.txt` & `alphamed-federated-0.4.7/src/alphamed_federated.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,18 @@
 src/alphafed/examples/fed_prox/model/net.py
 src/alphafed/examples/fed_prox/model/scheduler.py
 src/alphafed/examples/hetero_nn/__init__.py
 src/alphafed/examples/hetero_nn/clean_history_msg.py
 src/alphafed/examples/hetero_nn/demos.py
 src/alphafed/examples/hetero_nn/run_collaborater.py
 src/alphafed/examples/hetero_nn/run_host.py
+src/alphafed/examples/hetero_nn/hetero_fed_irm/collaborator_scheduler.py
+src/alphafed/examples/hetero_nn/hetero_fed_irm/data_checker.py
+src/alphafed/examples/hetero_nn/hetero_fed_irm/host_scheduler.py
+src/alphafed/examples/hetero_nn/hetero_fed_irm/res_net.py
 src/alphafed/examples/hetero_nn/psi/demos.py
 src/alphafed/examples/hetero_nn/psi/run_collaborator_2.py
 src/alphafed/examples/hetero_nn/psi/run_collaborator_3.py
 src/alphafed/examples/hetero_nn/psi/run_collaborator_4.py
 src/alphafed/examples/hetero_nn/psi/run_collaborator_5.py
 src/alphafed/examples/hetero_nn/psi/run_initiator.py
 src/alphafed/fed_avg/__init__.py
```

