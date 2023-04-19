# Comparing `tmp/super_gradients-3.0.8-py3-none-any.whl.zip` & `tmp/super_gradients-3.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,505 +1,531 @@
-Zip file size: 892893 bytes, number of entries: 503
--rw-r--r--  2.0 unx      932 b- defN 23-Apr-02 07:43 super_gradients/__init__.py
--rwxr-xr-x  2.0 unx       44 b- defN 23-Apr-02 07:43 super_gradients/requirements.pro.txt
--rwxr-xr-x  2.0 unx      729 b- defN 23-Apr-02 07:43 super_gradients/requirements.txt
--rw-r--r--  2.0 unx      654 b- defN 23-Apr-02 07:43 super_gradients/train_from_recipe.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Apr-02 07:43 super_gradients/common/__init__.py
--rw-r--r--  2.0 unx    14327 b- defN 23-Apr-02 07:43 super_gradients/common/object_names.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/common/abstractions/__init__.py
--rw-r--r--  2.0 unx      879 b- defN 23-Apr-02 07:43 super_gradients/common/abstractions/abstract_logger.py
--rw-r--r--  2.0 unx     3129 b- defN 23-Apr-02 07:43 super_gradients/common/abstractions/mute_processes.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/common/auto_logging/__init__.py
--rw-r--r--  2.0 unx     4687 b- defN 23-Apr-02 07:43 super_gradients/common/auto_logging/auto_logger.py
--rw-r--r--  2.0 unx     6625 b- defN 23-Apr-02 07:43 super_gradients/common/auto_logging/console_logging.py
--rw-r--r--  2.0 unx      142 b- defN 23-Apr-02 07:43 super_gradients/common/aws_connection/__init__.py
--rw-r--r--  2.0 unx     4182 b- defN 23-Apr-02 07:43 super_gradients/common/aws_connection/aws_connector.py
--rw-r--r--  2.0 unx     7198 b- defN 23-Apr-02 07:43 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
--rw-r--r--  2.0 unx      119 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/crash_handler.py
--rw-r--r--  2.0 unx    11775 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/crash_tips.py
--rw-r--r--  2.0 unx      886 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/crash_tips_setup.py
--rw-r--r--  2.0 unx     1740 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/exception.py
--rw-r--r--  2.0 unx     2357 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/exception_monitoring_setup.py
--rw-r--r--  2.0 unx      789 b- defN 23-Apr-02 07:43 super_gradients/common/crash_handler/utils.py
--rw-r--r--  2.0 unx      140 b- defN 23-Apr-02 07:43 super_gradients/common/data_connection/__init__.py
--rw-r--r--  2.0 unx    17959 b- defN 23-Apr-02 07:43 super_gradients/common/data_connection/s3_connector.py
--rw-r--r--  2.0 unx      325 b- defN 23-Apr-02 07:43 super_gradients/common/data_interface/__init__.py
--rw-r--r--  2.0 unx     9699 b- defN 23-Apr-02 07:43 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
--rw-r--r--  2.0 unx     2050 b- defN 23-Apr-02 07:43 super_gradients/common/data_interface/dataset_data_interface.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/__init__.py
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/__init__.py
--rw-r--r--  2.0 unx      309 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/deep_learning_task.py
--rw-r--r--  2.0 unx      108 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/downsample_mode.py
--rw-r--r--  2.0 unx      317 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/evaluation_type.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/multi_gpu_mode.py
--rw-r--r--  2.0 unx     1200 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/strict_load.py
--rw-r--r--  2.0 unx      160 b- defN 23-Apr-02 07:43 super_gradients/common/data_types/enum/upsample_mode.py
--rw-r--r--  2.0 unx      257 b- defN 23-Apr-02 07:43 super_gradients/common/decorators/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-Apr-02 07:43 super_gradients/common/decorators/code_save_decorator.py
--rw-r--r--  2.0 unx     3663 b- defN 23-Apr-02 07:43 super_gradients/common/decorators/deci_logger.py
--rw-r--r--  2.0 unx     2921 b- defN 23-Apr-02 07:43 super_gradients/common/decorators/explicit_params_validator.py
--rw-r--r--  2.0 unx     1315 b- defN 23-Apr-02 07:43 super_gradients/common/decorators/factory_decorator.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Apr-02 07:43 super_gradients/common/decorators/singleton.py
--rw-r--r--  2.0 unx      202 b- defN 23-Apr-02 07:43 super_gradients/common/environment/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Apr-02 07:43 super_gradients/common/environment/argparse_utils.py
--rw-r--r--  2.0 unx     9170 b- defN 23-Apr-02 07:43 super_gradients/common/environment/cfg_utils.py
--rw-r--r--  2.0 unx     4218 b- defN 23-Apr-02 07:43 super_gradients/common/environment/checkpoints_dir_utils.py
--rw-r--r--  2.0 unx     2682 b- defN 23-Apr-02 07:43 super_gradients/common/environment/ddp_utils.py
--rw-r--r--  2.0 unx      752 b- defN 23-Apr-02 07:43 super_gradients/common/environment/device_utils.py
--rw-r--r--  2.0 unx     1147 b- defN 23-Apr-02 07:43 super_gradients/common/environment/env_variables.py
--rw-r--r--  2.0 unx     1550 b- defN 23-Apr-02 07:43 super_gradients/common/environment/omegaconf_utils.py
--rw-r--r--  2.0 unx      459 b- defN 23-Apr-02 07:43 super_gradients/common/environment/path_utils.py
--rw-r--r--  2.0 unx      112 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/__init__.py
--rw-r--r--  2.0 unx      153 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/cpu.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/data_models.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/disk.py
--rw-r--r--  2.0 unx     5427 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/monitoring.py
--rw-r--r--  2.0 unx      948 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/network.py
--rw-r--r--  2.0 unx      629 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/utils.py
--rw-r--r--  2.0 unx      145 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/virtual_memory.py
--rw-r--r--  2.0 unx      681 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/gpu/__init__.py
--rw-r--r--  2.0 unx     2270 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/gpu/gpu.py
--rw-r--r--  2.0 unx   121647 b- defN 23-Apr-02 07:43 super_gradients/common/environment/monitoring/gpu/pynvml.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/common/exceptions/__init__.py
--rw-r--r--  2.0 unx      926 b- defN 23-Apr-02 07:43 super_gradients/common/exceptions/factory_exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/common/factories/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-Apr-02 07:43 super_gradients/common/factories/activations_type_factory.py
--rw-r--r--  2.0 unx     2881 b- defN 23-Apr-02 07:43 super_gradients/common/factories/base_factory.py
--rw-r--r--  2.0 unx      258 b- defN 23-Apr-02 07:43 super_gradients/common/factories/bbox_format_factory.py
--rw-r--r--  2.0 unx      232 b- defN 23-Apr-02 07:43 super_gradients/common/factories/callbacks_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-Apr-02 07:43 super_gradients/common/factories/collate_functions_factory.py
--rw-r--r--  2.0 unx      292 b- defN 23-Apr-02 07:43 super_gradients/common/factories/context_modules_factory.py
--rw-r--r--  2.0 unx      321 b- defN 23-Apr-02 07:43 super_gradients/common/factories/data_formats_factory.py
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-02 07:43 super_gradients/common/factories/datasets_factory.py
--rw-r--r--  2.0 unx     1014 b- defN 23-Apr-02 07:43 super_gradients/common/factories/detection_modules_factory.py
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-02 07:43 super_gradients/common/factories/list_factory.py
--rw-r--r--  2.0 unx      223 b- defN 23-Apr-02 07:43 super_gradients/common/factories/losses_factory.py
--rw-r--r--  2.0 unx      226 b- defN 23-Apr-02 07:43 super_gradients/common/factories/metrics_factory.py
--rw-r--r--  2.0 unx      467 b- defN 23-Apr-02 07:43 super_gradients/common/factories/optimizers_type_factory.py
--rw-r--r--  2.0 unx      271 b- defN 23-Apr-02 07:43 super_gradients/common/factories/pre_launch_callbacks_factory.py
--rw-r--r--  2.0 unx      229 b- defN 23-Apr-02 07:43 super_gradients/common/factories/samplers_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-Apr-02 07:43 super_gradients/common/factories/target_generator_factory.py
--rw-r--r--  2.0 unx     1873 b- defN 23-Apr-02 07:43 super_gradients/common/factories/transforms_factory.py
--rw-r--r--  2.0 unx     2377 b- defN 23-Apr-02 07:43 super_gradients/common/factories/type_factory.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/common/plugins/__init__.py
--rw-r--r--  2.0 unx    10974 b- defN 23-Apr-02 07:43 super_gradients/common/plugins/deci_client.py
--rw-r--r--  2.0 unx      271 b- defN 23-Apr-02 07:43 super_gradients/common/registry/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Apr-02 07:43 super_gradients/common/registry/albumentation.py
--rw-r--r--  2.0 unx     5918 b- defN 23-Apr-02 07:43 super_gradients/common/registry/registry.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/common/registry/registry_utils.py
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-02 07:43 super_gradients/common/sg_loggers/__init__.py
--rw-r--r--  2.0 unx     7355 b- defN 23-Apr-02 07:43 super_gradients/common/sg_loggers/abstract_sg_logger.py
--rw-r--r--  2.0 unx    14980 b- defN 23-Apr-02 07:43 super_gradients/common/sg_loggers/base_sg_logger.py
--rw-r--r--  2.0 unx    10055 b- defN 23-Apr-02 07:43 super_gradients/common/sg_loggers/clearml_sg_logger.py
--rw-r--r--  2.0 unx     6618 b- defN 23-Apr-02 07:43 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
--rw-r--r--  2.0 unx    13073 b- defN 23-Apr-02 07:43 super_gradients/common/sg_loggers/wandb_sg_logger.py
--rw-r--r--  2.0 unx    85509 b- defN 23-Apr-02 07:43 super_gradients/examples/SG_Walkthrough.ipynb
--rw-r--r--  2.0 unx    69618 b- defN 23-Apr-02 07:43 super_gradients/examples/SG_quickstart_classification.ipynb
--rw-r--r--  2.0 unx    54966 b- defN 23-Apr-02 07:43 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
--rw-r--r--  2.0 unx    65090 b- defN 23-Apr-02 07:43 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/cifar10_training_torch_objects/__init__.py
--rw-r--r--  2.0 unx     2526 b- defN 23-Apr-02 07:43 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/convert_recipe_example/__init__.py
--rw-r--r--  2.0 unx      870 b- defN 23-Apr-02 07:43 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/ddrnet_imagenet/__init__.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Apr-02 07:43 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/deci_lab_export_example/__init__.py
--rw-r--r--  2.0 unx     3562 b- defN 23-Apr-02 07:43 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/early_stop/__init__.py
--rw-r--r--  2.0 unx     1596 b- defN 23-Apr-02 07:43 super_gradients/examples/early_stop/early_stop_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/evaluate_checkpoint_example/__init__.py
--rw-r--r--  2.0 unx     1683 b- defN 23-Apr-02 07:43 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/evaluate_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx     1779 b- defN 23-Apr-02 07:43 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/loggers_examples/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-Apr-02 07:43 super_gradients/examples/loggers_examples/clearml_logger_example.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Apr-02 07:43 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/qat_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-02 07:43 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/non_default_calibrators_example.py
--rw-r--r--  2.0 unx     2310 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/ptq_e2e_example.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
--rw-r--r--  2.0 unx     4923 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/resnet_qat_example.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/skipping_quantization_example.py
--rw-r--r--  2.0 unx      832 b- defN 23-Apr-02 07:43 super_gradients/examples/quantization/vanilla_quantize_all_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/regseg_transfer_learning_example/__init__.py
--rw-r--r--  2.0 unx     2379 b- defN 23-Apr-02 07:43 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/resume_experiment_example/__init__.py
--rw-r--r--  2.0 unx      534 b- defN 23-Apr-02 07:43 super_gradients/examples/resume_experiment_example/resume_experiment.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_kd_recipe_example/__init__.py
--rw-r--r--  2.0 unx      655 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      627 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
--rw-r--r--  2.0 unx     1643 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_with_user_objects/train.py
--rw-r--r--  2.0 unx     2548 b- defN 23-Apr-02 07:43 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
--rw-r--r--  2.0 unx     2589 b- defN 23-Apr-02 07:43 super_gradients/modules/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/modules/all_detection_modules.py
--rw-r--r--  2.0 unx      617 b- defN 23-Apr-02 07:43 super_gradients/modules/anti_alias.py
--rw-r--r--  2.0 unx     2073 b- defN 23-Apr-02 07:43 super_gradients/modules/conv_bn_act_block.py
--rw-r--r--  2.0 unx     1976 b- defN 23-Apr-02 07:43 super_gradients/modules/conv_bn_relu_block.py
--rw-r--r--  2.0 unx    15129 b- defN 23-Apr-02 07:43 super_gradients/modules/detection_modules.py
--rw-r--r--  2.0 unx     4362 b- defN 23-Apr-02 07:43 super_gradients/modules/multi_output_modules.py
--rw-r--r--  2.0 unx     3958 b- defN 23-Apr-02 07:43 super_gradients/modules/pose_estimation_modules.py
--rw-r--r--  2.0 unx    11642 b- defN 23-Apr-02 07:43 super_gradients/modules/qarepvgg_block.py
--rw-r--r--  2.0 unx     8544 b- defN 23-Apr-02 07:43 super_gradients/modules/repvgg_block.py
--rw-r--r--  2.0 unx     1887 b- defN 23-Apr-02 07:43 super_gradients/modules/sampling.py
--rw-r--r--  2.0 unx     1459 b- defN 23-Apr-02 07:43 super_gradients/modules/se_blocks.py
--rw-r--r--  2.0 unx     1403 b- defN 23-Apr-02 07:43 super_gradients/modules/skip_connections.py
--rw-r--r--  2.0 unx     2565 b- defN 23-Apr-02 07:43 super_gradients/modules/utils.py
--rw-r--r--  2.0 unx      716 b- defN 23-Apr-02 07:43 super_gradients/modules/quantization/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 23-Apr-02 07:43 super_gradients/modules/quantization/quantized_skip_connections.py
--rw-r--r--  2.0 unx     4604 b- defN 23-Apr-02 07:43 super_gradients/modules/quantization/quantized_stdc_blocks.py
--rw-r--r--  2.0 unx     1281 b- defN 23-Apr-02 07:43 super_gradients/modules/quantization/resnet_bottleneck.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/recipes/__init__.py
--rw-r--r--  2.0 unx     1516 b- defN 23-Apr-02 07:43 super_gradients/recipes/cifar10_resnet.yaml
--rw-r--r--  2.0 unx     3856 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_ddrnet.yaml
--rw-r--r--  2.0 unx     4072 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_kd_base.yaml
--rw-r--r--  2.0 unx     3615 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_pplite_seg50.yaml
--rw-r--r--  2.0 unx     3514 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_pplite_seg75.yaml
--rw-r--r--  2.0 unx     2771 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_regseg48.yaml
--rw-r--r--  2.0 unx      852 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_stdc_base.yaml
--rw-r--r--  2.0 unx     3175 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_stdc_seg50.yaml
--rw-r--r--  2.0 unx     3369 b- defN 23-Apr-02 07:43 super_gradients/recipes/cityscapes_stdc_seg75.yaml
--rw-r--r--  2.0 unx     2063 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
--rw-r--r--  2.0 unx     3821 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
--rw-r--r--  2.0 unx     2231 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_pose_pppose_l.yaml
--rw-r--r--  2.0 unx     2388 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_ppyoloe_l.yaml
--rw-r--r--  2.0 unx     2388 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_ppyoloe_m.yaml
--rw-r--r--  2.0 unx     2274 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_ppyoloe_s.yaml
--rw-r--r--  2.0 unx     2367 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_ppyoloe_x.yaml
--rw-r--r--  2.0 unx     2202 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
--rw-r--r--  2.0 unx     3053 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco2017_yolox.yaml
--rw-r--r--  2.0 unx     1649 b- defN 23-Apr-02 07:43 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
--rw-r--r--  2.0 unx     1418 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_efficientnet.yaml
--rw-r--r--  2.0 unx     1402 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_mobilenetv2.yaml
--rw-r--r--  2.0 unx      741 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
--rw-r--r--  2.0 unx      992 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
--rw-r--r--  2.0 unx      992 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
--rw-r--r--  2.0 unx     2387 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_regnetY.yaml
--rw-r--r--  2.0 unx     1519 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_repvgg.yaml
--rw-r--r--  2.0 unx     1442 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_resnet50.yaml
--rw-r--r--  2.0 unx     2998 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_resnet50_kd.yaml
--rw-r--r--  2.0 unx     1409 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_vit_base.yaml
--rw-r--r--  2.0 unx     1283 b- defN 23-Apr-02 07:43 super_gradients/recipes/imagenet_vit_large.yaml
--rw-r--r--  2.0 unx     1520 b- defN 23-Apr-02 07:43 super_gradients/recipes/supervisely_unet.yaml
--rw-r--r--  2.0 unx     1906 b- defN 23-Apr-02 07:43 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
--rw-r--r--  2.0 unx     2367 b- defN 23-Apr-02 07:43 super_gradients/recipes/user_recipe_mnist_example.yaml
--rw-r--r--  2.0 unx     2222 b- defN 23-Apr-02 07:43 super_gradients/recipes/anchors/ssd_anchors.yaml
--rw-r--r--  2.0 unx      563 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
--rw-r--r--  2.0 unx      104 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
--rw-r--r--  2.0 unx      194 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
--rw-r--r--  2.0 unx      156 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
--rw-r--r--  2.0 unx      356 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
--rw-r--r--  2.0 unx      281 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
--rw-r--r--  2.0 unx     1245 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
--rw-r--r--  2.0 unx      985 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
--rw-r--r--  2.0 unx     1112 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
--rw-r--r--  2.0 unx      196 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
--rw-r--r--  2.0 unx      204 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
--rw-r--r--  2.0 unx      352 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
--rw-r--r--  2.0 unx       89 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
--rw-r--r--  2.0 unx       95 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
--rw-r--r--  2.0 unx       88 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
--rw-r--r--  2.0 unx       32 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
--rw-r--r--  2.0 unx      655 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
--rw-r--r--  2.0 unx      605 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
--rw-r--r--  2.0 unx     1369 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/unet_arch_params.yaml
--rw-r--r--  2.0 unx     3014 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
--rw-r--r--  2.0 unx     2393 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolo_arch_params.yaml
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
--rw-r--r--  2.0 unx      236 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
--rw-r--r--  2.0 unx      229 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
--rw-r--r--  2.0 unx      228 b- defN 23-Apr-02 07:43 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
--rw-r--r--  2.0 unx      611 b- defN 23-Apr-02 07:43 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
--rw-r--r--  2.0 unx       72 b- defN 23-Apr-02 07:43 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/recipes/conversion_params/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 23-Apr-02 07:43 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
--rw-r--r--  2.0 unx     2040 b- defN 23-Apr-02 07:43 super_gradients/recipes/conversion_params/default_conversion_params.yaml
--rw-r--r--  2.0 unx      869 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
--rw-r--r--  2.0 unx     1530 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
--rw-r--r--  2.0 unx     1056 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
--rw-r--r--  2.0 unx      615 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
--rw-r--r--  2.0 unx      525 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
--rw-r--r--  2.0 unx      706 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx      644 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
--rw-r--r--  2.0 unx      709 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
--rw-r--r--  2.0 unx      708 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx     3946 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     3662 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml
--rw-r--r--  2.0 unx     4202 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
--rw-r--r--  2.0 unx     3590 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
--rw-r--r--  2.0 unx     2461 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
--rw-r--r--  2.0 unx      405 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
--rw-r--r--  2.0 unx     1466 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx      931 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx      732 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
--rw-r--r--  2.0 unx      142 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
--rw-r--r--  2.0 unx      734 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
--rw-r--r--  2.0 unx     1059 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
--rw-r--r--  2.0 unx     1093 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
--rw-r--r--  2.0 unx      845 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
--rw-r--r--  2.0 unx     1762 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
--rw-r--r--  2.0 unx      149 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     1571 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     1414 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx      961 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
--rw-r--r--  2.0 unx      558 b- defN 23-Apr-02 07:43 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx     1155 b- defN 23-Apr-02 07:43 super_gradients/recipes/quantization_params/default_quantization_params.yaml
--rw-r--r--  2.0 unx      591 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
--rw-r--r--  2.0 unx      877 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
--rw-r--r--  2.0 unx     1302 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
--rw-r--r--  2.0 unx      723 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
--rw-r--r--  2.0 unx      956 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
--rw-r--r--  2.0 unx      461 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
--rw-r--r--  2.0 unx     5459 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/default_train_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
--rw-r--r--  2.0 unx      742 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
--rw-r--r--  2.0 unx      549 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
--rw-r--r--  2.0 unx      795 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
--rw-r--r--  2.0 unx      476 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
--rw-r--r--  2.0 unx      484 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
--rw-r--r--  2.0 unx      522 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
--rw-r--r--  2.0 unx      602 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
--rw-r--r--  2.0 unx      519 b- defN 23-Apr-02 07:43 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-02 07:43 super_gradients/sanity_check/__init__.py
--rw-r--r--  2.0 unx     5262 b- defN 23-Apr-02 07:43 super_gradients/sanity_check/env_sanity_check.py
--rw-r--r--  2.0 unx      666 b- defN 23-Apr-02 07:43 super_gradients/training/__init__.py
--rw-r--r--  2.0 unx     4155 b- defN 23-Apr-02 07:43 super_gradients/training/params.py
--rw-r--r--  2.0 unx     5696 b- defN 23-Apr-02 07:43 super_gradients/training/pretrained_models.py
--rw-r--r--  2.0 unx     3228 b- defN 23-Apr-02 07:43 super_gradients/training/dataloaders/__init__.py
--rw-r--r--  2.0 unx    29718 b- defN 23-Apr-02 07:43 super_gradients/training/dataloaders/dataloaders.py
--rw-r--r--  2.0 unx     1714 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/__init__.py
--rw-r--r--  2.0 unx    14162 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/auto_augment.py
--rw-r--r--  2.0 unx     3705 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_augmentation.py
--rw-r--r--  2.0 unx     3484 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/datasets_conf.py
--rw-r--r--  2.0 unx    30279 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/datasets_utils.py
--rw-r--r--  2.0 unx    14663 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/mixup.py
--rw-r--r--  2.0 unx    11746 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/sg_dataset.py
--rw-r--r--  2.0 unx      252 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/classification_datasets/__init__.py
--rw-r--r--  2.0 unx     3096 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/classification_datasets/cifar.py
--rw-r--r--  2.0 unx     1706 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
--rw-r--r--  2.0 unx      363 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/default_formats.py
--rw-r--r--  2.0 unx     3071 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/format_converter.py
--rw-r--r--  2.0 unx     7928 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/formats.py
--rw-r--r--  2.0 unx     1044 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
--rw-r--r--  2.0 unx     2674 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
--rw-r--r--  2.0 unx     5094 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
--rw-r--r--  2.0 unx     2089 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
--rw-r--r--  2.0 unx     2043 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
--rw-r--r--  2.0 unx     5043 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
--rw-r--r--  2.0 unx     2948 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
--rw-r--r--  2.0 unx      575 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
--rw-r--r--  2.0 unx     1792 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
--rw-r--r--  2.0 unx     8384 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
--rw-r--r--  2.0 unx      399 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/detection_datasets/__init__.py
--rw-r--r--  2.0 unx     2511 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/detection_datasets/coco_detection.py
--rw-r--r--  2.0 unx     8762 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
--rw-r--r--  2.0 unx    24762 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/detection_datasets/detection_dataset.py
--rw-r--r--  2.0 unx    11353 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
--rw-r--r--  2.0 unx      502 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
--rw-r--r--  2.0 unx     4899 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
--rw-r--r--  2.0 unx     9066 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
--rw-r--r--  2.0 unx     5929 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
--rw-r--r--  2.0 unx    10167 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
--rw-r--r--  2.0 unx      385 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/samplers/__init__.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/samplers/infinite_sampler.py
--rw-r--r--  2.0 unx     4809 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
--rw-r--r--  2.0 unx     1037 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/__init__.py
--rw-r--r--  2.0 unx     6714 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
--rw-r--r--  2.0 unx     7717 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
--rw-r--r--  2.0 unx     5518 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
--rw-r--r--  2.0 unx    11146 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
--rw-r--r--  2.0 unx     8470 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
--rw-r--r--  2.0 unx     3062 b- defN 23-Apr-02 07:43 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/exceptions/__init__.py
--rw-r--r--  2.0 unx     1761 b- defN 23-Apr-02 07:43 super_gradients/training/exceptions/dataset_exceptions.py
--rw-r--r--  2.0 unx     2826 b- defN 23-Apr-02 07:43 super_gradients/training/exceptions/kd_trainer_exceptions.py
--rw-r--r--  2.0 unx      946 b- defN 23-Apr-02 07:43 super_gradients/training/exceptions/loss_exceptions.py
--rw-r--r--  2.0 unx     1268 b- defN 23-Apr-02 07:43 super_gradients/training/exceptions/sg_trainer_exceptions.py
--rw-r--r--  2.0 unx      132 b- defN 23-Apr-02 07:43 super_gradients/training/kd_trainer/__init__.py
--rw-r--r--  2.0 unx    16582 b- defN 23-Apr-02 07:43 super_gradients/training/kd_trainer/kd_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/legacy/__init__.py
--rw-r--r--  2.0 unx     4198 b- defN 23-Apr-02 07:43 super_gradients/training/legacy/utils.py
--rw-r--r--  2.0 unx     1476 b- defN 23-Apr-02 07:43 super_gradients/training/losses/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/losses/all_losses.py
--rw-r--r--  2.0 unx     1219 b- defN 23-Apr-02 07:43 super_gradients/training/losses/bce_dice_loss.py
--rw-r--r--  2.0 unx      419 b- defN 23-Apr-02 07:43 super_gradients/training/losses/bce_loss.py
--rw-r--r--  2.0 unx     2374 b- defN 23-Apr-02 07:43 super_gradients/training/losses/cwd_loss.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Apr-02 07:43 super_gradients/training/losses/ddrnet_loss.py
--rw-r--r--  2.0 unx     3377 b- defN 23-Apr-02 07:43 super_gradients/training/losses/dekr_loss.py
--rw-r--r--  2.0 unx     5646 b- defN 23-Apr-02 07:43 super_gradients/training/losses/dice_ce_edge_loss.py
--rw-r--r--  2.0 unx     5208 b- defN 23-Apr-02 07:43 super_gradients/training/losses/dice_loss.py
--rw-r--r--  2.0 unx     1214 b- defN 23-Apr-02 07:43 super_gradients/training/losses/focal_loss.py
--rw-r--r--  2.0 unx     5051 b- defN 23-Apr-02 07:43 super_gradients/training/losses/iou_loss.py
--rw-r--r--  2.0 unx     2176 b- defN 23-Apr-02 07:43 super_gradients/training/losses/kd_losses.py
--rw-r--r--  2.0 unx     4177 b- defN 23-Apr-02 07:43 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
--rw-r--r--  2.0 unx      550 b- defN 23-Apr-02 07:43 super_gradients/training/losses/loss_utils.py
--rw-r--r--  2.0 unx     3854 b- defN 23-Apr-02 07:43 super_gradients/training/losses/mask_loss.py
--rw-r--r--  2.0 unx     4129 b- defN 23-Apr-02 07:43 super_gradients/training/losses/ohem_ce_loss.py
--rw-r--r--  2.0 unx    41319 b- defN 23-Apr-02 07:43 super_gradients/training/losses/ppyolo_loss.py
--rw-r--r--  2.0 unx     1010 b- defN 23-Apr-02 07:43 super_gradients/training/losses/r_squared_loss.py
--rw-r--r--  2.0 unx     3453 b- defN 23-Apr-02 07:43 super_gradients/training/losses/seg_kd_loss.py
--rw-r--r--  2.0 unx     1650 b- defN 23-Apr-02 07:43 super_gradients/training/losses/shelfnet_ohem_loss.py
--rw-r--r--  2.0 unx     1949 b- defN 23-Apr-02 07:43 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
--rw-r--r--  2.0 unx     8794 b- defN 23-Apr-02 07:43 super_gradients/training/losses/ssd_loss.py
--rw-r--r--  2.0 unx     9721 b- defN 23-Apr-02 07:43 super_gradients/training/losses/stdc_loss.py
--rw-r--r--  2.0 unx     5771 b- defN 23-Apr-02 07:43 super_gradients/training/losses/structure_loss.py
--rw-r--r--  2.0 unx    50149 b- defN 23-Apr-02 07:43 super_gradients/training/losses/yolox_loss.py
--rw-r--r--  2.0 unx     1052 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/all_metrics.py
--rw-r--r--  2.0 unx     3262 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/classification_metrics.py
--rw-r--r--  2.0 unx    10741 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/detection_metrics.py
--rw-r--r--  2.0 unx     3973 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/metric_utils.py
--rw-r--r--  2.0 unx    15346 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/pose_estimation_metrics.py
--rw-r--r--  2.0 unx    11454 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/pose_estimation_utils.py
--rw-r--r--  2.0 unx    11935 b- defN 23-Apr-02 07:43 super_gradients/training/metrics/segmentation_metrics.py
--rw-r--r--  2.0 unx     8103 b- defN 23-Apr-02 07:43 super_gradients/training/models/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Apr-02 07:43 super_gradients/training/models/arch_params_factory.py
--rw-r--r--  2.0 unx     7060 b- defN 23-Apr-02 07:43 super_gradients/training/models/conversion.py
--rw-r--r--  2.0 unx    11273 b- defN 23-Apr-02 07:43 super_gradients/training/models/model_factory.py
--rw-r--r--  2.0 unx     2998 b- defN 23-Apr-02 07:43 super_gradients/training/models/sg_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/__init__.py
--rw-r--r--  2.0 unx    20025 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/beit.py
--rw-r--r--  2.0 unx     7472 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/densenet.py
--rw-r--r--  2.0 unx     3678 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/dpn.py
--rw-r--r--  2.0 unx    29281 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/efficientnet.py
--rw-r--r--  2.0 unx     8862 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/googlenet.py
--rw-r--r--  2.0 unx      798 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/lenet.py
--rw-r--r--  2.0 unx     2407 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/mobilenet.py
--rw-r--r--  2.0 unx     9472 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/mobilenetv2.py
--rw-r--r--  2.0 unx     8696 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/mobilenetv3.py
--rw-r--r--  2.0 unx     4339 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/pnasnet.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/preact_resnet.py
--rw-r--r--  2.0 unx    13599 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/regnet.py
--rw-r--r--  2.0 unx     7924 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/repvgg.py
--rw-r--r--  2.0 unx    15042 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/resnet.py
--rw-r--r--  2.0 unx     6294 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/resnext.py
--rw-r--r--  2.0 unx     4134 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/senet.py
--rw-r--r--  2.0 unx     3660 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/shufflenet.py
--rw-r--r--  2.0 unx     9768 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/shufflenetv2.py
--rw-r--r--  2.0 unx     1538 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/vgg.py
--rw-r--r--  2.0 unx     9210 b- defN 23-Apr-02 07:43 super_gradients/training/models/classification_models/vit.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/__init__.py
--rw-r--r--  2.0 unx     9502 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/csp_darknet53.py
--rw-r--r--  2.0 unx     9814 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/csp_resnet.py
--rw-r--r--  2.0 unx     3782 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/customizable_detector.py
--rw-r--r--  2.0 unx     4746 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/darknet53.py
--rw-r--r--  2.0 unx     1438 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/ssd.py
--rw-r--r--  2.0 unx    24897 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/yolo_base.py
--rw-r--r--  2.0 unx     2459 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/yolox.py
--rw-r--r--  2.0 unx      155 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
--rw-r--r--  2.0 unx     6984 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
--rw-r--r--  2.0 unx     3487 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
--rw-r--r--  2.0 unx     3725 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
--rw-r--r--  2.0 unx    12334 b- defN 23-Apr-02 07:43 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/models/kd_modules/__init__.py
--rw-r--r--  2.0 unx     3170 b- defN 23-Apr-02 07:43 super_gradients/training/models/kd_modules/kd_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/models/pose_estimation_models/__init__.py
--rw-r--r--  2.0 unx    21231 b- defN 23-Apr-02 07:43 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
--rw-r--r--  2.0 unx      892 b- defN 23-Apr-02 07:43 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
--rw-r--r--  2.0 unx      891 b- defN 23-Apr-02 07:43 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/__init__.py
--rw-r--r--  2.0 unx      964 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/common.py
--rw-r--r--  2.0 unx     5139 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/context_modules.py
--rw-r--r--  2.0 unx    27896 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/ddrnet.py
--rw-r--r--  2.0 unx     2439 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
--rw-r--r--  2.0 unx    21760 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/laddernet.py
--rw-r--r--  2.0 unx    15648 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/ppliteseg.py
--rw-r--r--  2.0 unx    14424 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/regseg.py
--rw-r--r--  2.0 unx     2256 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/segmentation_module.py
--rw-r--r--  2.0 unx    24833 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/shelfnet.py
--rw-r--r--  2.0 unx    29005 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/stdc.py
--rw-r--r--  2.0 unx      260 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/unet/__init__.py
--rw-r--r--  2.0 unx    12324 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/unet/unet.py
--rw-r--r--  2.0 unx     8305 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
--rw-r--r--  2.0 unx    13292 b- defN 23-Apr-02 07:43 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
--rw-r--r--  2.0 unx      119 b- defN 23-Apr-02 07:43 super_gradients/training/models/user_models/__init__.py
--rw-r--r--  2.0 unx      393 b- defN 23-Apr-02 07:43 super_gradients/training/pre_launch_callbacks/__init__.py
--rw-r--r--  2.0 unx    13955 b- defN 23-Apr-02 07:43 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-02 07:43 super_gradients/training/qat_trainer/__init__.py
--rw-r--r--  2.0 unx     9896 b- defN 23-Apr-02 07:43 super_gradients/training/qat_trainer/qat_trainer.py
--rw-r--r--  2.0 unx      184 b- defN 23-Apr-02 07:43 super_gradients/training/sg_trainer/__init__.py
--rw-r--r--  2.0 unx    95882 b- defN 23-Apr-02 07:43 super_gradients/training/sg_trainer/sg_trainer.py
--rw-r--r--  2.0 unx     1685 b- defN 23-Apr-02 07:43 super_gradients/training/training_hyperparams/__init__.py
--rw-r--r--  2.0 unx     3774 b- defN 23-Apr-02 07:43 super_gradients/training/training_hyperparams/training_hyperparams.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Apr-02 07:43 super_gradients/training/transforms/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/transforms/all_transforms.py
--rw-r--r--  2.0 unx    16193 b- defN 23-Apr-02 07:43 super_gradients/training/transforms/keypoint_transforms.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Apr-02 07:43 super_gradients/training/transforms/pipeline_adaptors.py
--rw-r--r--  2.0 unx    57465 b- defN 23-Apr-02 07:43 super_gradients/training/transforms/transforms.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Apr-02 07:43 super_gradients/training/utils/__init__.py
--rw-r--r--  2.0 unx     1673 b- defN 23-Apr-02 07:43 super_gradients/training/utils/activations_utils.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Apr-02 07:43 super_gradients/training/utils/bbox_utils.py
--rw-r--r--  2.0 unx    13875 b- defN 23-Apr-02 07:43 super_gradients/training/utils/checkpoint_utils.py
--rw-r--r--  2.0 unx     9794 b- defN 23-Apr-02 07:43 super_gradients/training/utils/config_utils.py
--rw-r--r--  2.0 unx     1132 b- defN 23-Apr-02 07:43 super_gradients/training/utils/deprecated_utils.py
--rw-r--r--  2.0 unx    53513 b- defN 23-Apr-02 07:43 super_gradients/training/utils/detection_utils.py
--rw-r--r--  2.0 unx    16153 b- defN 23-Apr-02 07:43 super_gradients/training/utils/distributed_training_utils.py
--rw-r--r--  2.0 unx     6352 b- defN 23-Apr-02 07:43 super_gradients/training/utils/early_stopping.py
--rw-r--r--  2.0 unx     9322 b- defN 23-Apr-02 07:43 super_gradients/training/utils/ema.py
--rw-r--r--  2.0 unx     2610 b- defN 23-Apr-02 07:43 super_gradients/training/utils/ema_decay_schedules.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-02 07:43 super_gradients/training/utils/export_utils.py
--rw-r--r--  2.0 unx     7508 b- defN 23-Apr-02 07:43 super_gradients/training/utils/get_model_stats.py
--rw-r--r--  2.0 unx      771 b- defN 23-Apr-02 07:43 super_gradients/training/utils/kd_trainer_utils.py
--rw-r--r--  2.0 unx     5827 b- defN 23-Apr-02 07:43 super_gradients/training/utils/optimizer_utils.py
--rw-r--r--  2.0 unx      839 b- defN 23-Apr-02 07:43 super_gradients/training/utils/regularization_utils.py
--rw-r--r--  2.0 unx    10388 b- defN 23-Apr-02 07:43 super_gradients/training/utils/segmentation_utils.py
--rw-r--r--  2.0 unx    19633 b- defN 23-Apr-02 07:43 super_gradients/training/utils/sg_trainer_utils.py
--rw-r--r--  2.0 unx     6272 b- defN 23-Apr-02 07:43 super_gradients/training/utils/ssd_utils.py
--rw-r--r--  2.0 unx    17925 b- defN 23-Apr-02 07:43 super_gradients/training/utils/utils.py
--rw-r--r--  2.0 unx      303 b- defN 23-Apr-02 07:43 super_gradients/training/utils/version_utils.py
--rw-r--r--  2.0 unx     6209 b- defN 23-Apr-02 07:43 super_gradients/training/utils/weight_averaging_utils.py
--rw-r--r--  2.0 unx     2030 b- defN 23-Apr-02 07:43 super_gradients/training/utils/callbacks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 07:43 super_gradients/training/utils/callbacks/all_callbacks.py
--rw-r--r--  2.0 unx    20126 b- defN 23-Apr-02 07:43 super_gradients/training/utils/callbacks/base_callbacks.py
--rw-r--r--  2.0 unx    31285 b- defN 23-Apr-02 07:43 super_gradients/training/utils/callbacks/callbacks.py
--rw-r--r--  2.0 unx     1169 b- defN 23-Apr-02 07:43 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
--rw-r--r--  2.0 unx      396 b- defN 23-Apr-02 07:43 super_gradients/training/utils/optimizers/__init__.py
--rw-r--r--  2.0 unx     9760 b- defN 23-Apr-02 07:43 super_gradients/training/utils/optimizers/lamb.py
--rw-r--r--  2.0 unx     3008 b- defN 23-Apr-02 07:43 super_gradients/training/utils/optimizers/lion.py
--rw-r--r--  2.0 unx     6834 b- defN 23-Apr-02 07:43 super_gradients/training/utils/optimizers/rmsprop_tf.py
--rw-r--r--  2.0 unx      213 b- defN 23-Apr-02 07:43 super_gradients/training/utils/pose_estimation/__init__.py
--rw-r--r--  2.0 unx    11167 b- defN 23-Apr-02 07:43 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
--rw-r--r--  2.0 unx     7140 b- defN 23-Apr-02 07:43 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
--rw-r--r--  2.0 unx      387 b- defN 23-Apr-02 07:43 super_gradients/training/utils/quantization/__init__.py
--rw-r--r--  2.0 unx     6271 b- defN 23-Apr-02 07:43 super_gradients/training/utils/quantization/calibrator.py
--rw-r--r--  2.0 unx     8417 b- defN 23-Apr-02 07:43 super_gradients/training/utils/quantization/core.py
--rw-r--r--  2.0 unx     2196 b- defN 23-Apr-02 07:43 super_gradients/training/utils/quantization/export.py
--rw-r--r--  2.0 unx    17062 b- defN 23-Apr-02 07:43 super_gradients/training/utils/quantization/selective_quantization_utils.py
--rw-r--r--  2.0 unx    11341 b- defN 23-Apr-02 07:43 super_gradients-3.0.8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    32749 b- defN 23-Apr-02 07:43 super_gradients-3.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-02 07:43 super_gradients-3.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-02 07:43 super_gradients-3.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    58215 b- defN 23-Apr-02 07:43 super_gradients-3.0.8.dist-info/RECORD
-503 files, 2567105 bytes uncompressed, 794993 bytes compressed:  69.0%
+Zip file size: 938547 bytes, number of entries: 529
+-rw-r--r--  2.0 unx      932 b- defN 23-Apr-19 13:58 super_gradients/__init__.py
+-rwxr-xr-x  2.0 unx       44 b- defN 23-Apr-19 13:59 super_gradients/requirements.pro.txt
+-rwxr-xr-x  2.0 unx      729 b- defN 23-Apr-19 13:59 super_gradients/requirements.txt
+-rw-r--r--  2.0 unx      654 b- defN 23-Apr-19 13:58 super_gradients/train_from_recipe.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Apr-19 13:58 super_gradients/common/__init__.py
+-rw-r--r--  2.0 unx    15140 b- defN 23-Apr-19 13:58 super_gradients/common/object_names.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/abstractions/__init__.py
+-rw-r--r--  2.0 unx      879 b- defN 23-Apr-19 13:58 super_gradients/common/abstractions/abstract_logger.py
+-rw-r--r--  2.0 unx     3129 b- defN 23-Apr-19 13:58 super_gradients/common/abstractions/mute_processes.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/auto_logging/__init__.py
+-rw-r--r--  2.0 unx     4687 b- defN 23-Apr-19 13:58 super_gradients/common/auto_logging/auto_logger.py
+-rw-r--r--  2.0 unx     6625 b- defN 23-Apr-19 13:58 super_gradients/common/auto_logging/console_logging.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Apr-19 13:58 super_gradients/common/aws_connection/__init__.py
+-rw-r--r--  2.0 unx     4182 b- defN 23-Apr-19 13:58 super_gradients/common/aws_connection/aws_connector.py
+-rw-r--r--  2.0 unx     7198 b- defN 23-Apr-19 13:58 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/crash_handler.py
+-rw-r--r--  2.0 unx    11775 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/crash_tips.py
+-rw-r--r--  2.0 unx      886 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/crash_tips_setup.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/exception.py
+-rw-r--r--  2.0 unx     2357 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/exception_monitoring_setup.py
+-rw-r--r--  2.0 unx      789 b- defN 23-Apr-19 13:58 super_gradients/common/crash_handler/utils.py
+-rw-r--r--  2.0 unx      140 b- defN 23-Apr-19 13:58 super_gradients/common/data_connection/__init__.py
+-rw-r--r--  2.0 unx    17959 b- defN 23-Apr-19 13:58 super_gradients/common/data_connection/s3_connector.py
+-rw-r--r--  2.0 unx      325 b- defN 23-Apr-19 13:58 super_gradients/common/data_interface/__init__.py
+-rw-r--r--  2.0 unx     9699 b- defN 23-Apr-19 13:58 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-Apr-19 13:58 super_gradients/common/data_interface/dataset_data_interface.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/__init__.py
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/__init__.py
+-rw-r--r--  2.0 unx      309 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/deep_learning_task.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/downsample_mode.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/evaluation_type.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/multi_gpu_mode.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/strict_load.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Apr-19 13:58 super_gradients/common/data_types/enum/upsample_mode.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/code_save_decorator.py
+-rw-r--r--  2.0 unx     3663 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/deci_logger.py
+-rw-r--r--  2.0 unx     2921 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/explicit_params_validator.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/factory_decorator.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Apr-19 13:58 super_gradients/common/decorators/singleton.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Apr-19 13:58 super_gradients/common/environment/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Apr-19 13:58 super_gradients/common/environment/argparse_utils.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-Apr-19 13:58 super_gradients/common/environment/cfg_utils.py
+-rw-r--r--  2.0 unx     4218 b- defN 23-Apr-19 13:58 super_gradients/common/environment/checkpoints_dir_utils.py
+-rw-r--r--  2.0 unx     2682 b- defN 23-Apr-19 13:58 super_gradients/common/environment/ddp_utils.py
+-rw-r--r--  2.0 unx      752 b- defN 23-Apr-19 13:58 super_gradients/common/environment/device_utils.py
+-rw-r--r--  2.0 unx     1147 b- defN 23-Apr-19 13:58 super_gradients/common/environment/env_variables.py
+-rw-r--r--  2.0 unx     1768 b- defN 23-Apr-19 13:58 super_gradients/common/environment/omegaconf_utils.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Apr-19 13:58 super_gradients/common/environment/path_utils.py
+-rw-r--r--  2.0 unx      112 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/__init__.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/cpu.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/data_models.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/disk.py
+-rw-r--r--  2.0 unx     5427 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/monitoring.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/network.py
+-rw-r--r--  2.0 unx      629 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/utils.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/virtual_memory.py
+-rw-r--r--  2.0 unx      681 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/gpu/__init__.py
+-rw-r--r--  2.0 unx     2270 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/gpu/gpu.py
+-rw-r--r--  2.0 unx   121647 b- defN 23-Apr-19 13:58 super_gradients/common/environment/monitoring/gpu/pynvml.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/exceptions/__init__.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Apr-19 13:58 super_gradients/common/exceptions/factory_exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/factories/__init__.py
+-rw-r--r--  2.0 unx     1715 b- defN 23-Apr-19 13:58 super_gradients/common/factories/activations_type_factory.py
+-rw-r--r--  2.0 unx     2881 b- defN 23-Apr-19 13:58 super_gradients/common/factories/base_factory.py
+-rw-r--r--  2.0 unx      258 b- defN 23-Apr-19 13:58 super_gradients/common/factories/bbox_format_factory.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Apr-19 13:58 super_gradients/common/factories/callbacks_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Apr-19 13:58 super_gradients/common/factories/collate_functions_factory.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Apr-19 13:58 super_gradients/common/factories/context_modules_factory.py
+-rw-r--r--  2.0 unx      321 b- defN 23-Apr-19 13:58 super_gradients/common/factories/data_formats_factory.py
+-rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/common/factories/datasets_factory.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-Apr-19 13:58 super_gradients/common/factories/detection_modules_factory.py
+-rw-r--r--  2.0 unx      572 b- defN 23-Apr-19 13:58 super_gradients/common/factories/list_factory.py
+-rw-r--r--  2.0 unx      223 b- defN 23-Apr-19 13:58 super_gradients/common/factories/losses_factory.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Apr-19 13:58 super_gradients/common/factories/metrics_factory.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Apr-19 13:58 super_gradients/common/factories/optimizers_type_factory.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Apr-19 13:58 super_gradients/common/factories/pre_launch_callbacks_factory.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Apr-19 13:58 super_gradients/common/factories/processing_factory.py
+-rw-r--r--  2.0 unx      229 b- defN 23-Apr-19 13:58 super_gradients/common/factories/samplers_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Apr-19 13:58 super_gradients/common/factories/target_generator_factory.py
+-rw-r--r--  2.0 unx     1873 b- defN 23-Apr-19 13:58 super_gradients/common/factories/transforms_factory.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-Apr-19 13:58 super_gradients/common/factories/type_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/plugins/__init__.py
+-rw-r--r--  2.0 unx    10974 b- defN 23-Apr-19 13:58 super_gradients/common/plugins/deci_client.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Apr-19 13:58 super_gradients/common/registry/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Apr-19 13:58 super_gradients/common/registry/albumentation.py
+-rw-r--r--  2.0 unx     6006 b- defN 23-Apr-19 13:58 super_gradients/common/registry/registry.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/common/registry/registry_utils.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/__init__.py
+-rw-r--r--  2.0 unx     7355 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/abstract_sg_logger.py
+-rw-r--r--  2.0 unx    14980 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/base_sg_logger.py
+-rw-r--r--  2.0 unx    10055 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/clearml_sg_logger.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
+-rw-r--r--  2.0 unx    13073 b- defN 23-Apr-19 13:58 super_gradients/common/sg_loggers/wandb_sg_logger.py
+-rw-r--r--  2.0 unx    85509 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_Walkthrough.ipynb
+-rw-r--r--  2.0 unx    69618 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_quickstart_classification.ipynb
+-rw-r--r--  2.0 unx    54966 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
+-rw-r--r--  2.0 unx    65090 b- defN 23-Apr-19 13:58 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/cifar10_training_torch_objects/__init__.py
+-rw-r--r--  2.0 unx     2526 b- defN 23-Apr-19 13:58 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/convert_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      870 b- defN 23-Apr-19 13:58 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/ddrnet_imagenet/__init__.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Apr-19 13:58 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/deci_lab_export_example/__init__.py
+-rw-r--r--  2.0 unx     3562 b- defN 23-Apr-19 13:58 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/early_stop/__init__.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-Apr-19 13:58 super_gradients/examples/early_stop/early_stop_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_checkpoint_example/__init__.py
+-rw-r--r--  2.0 unx     1683 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx     1779 b- defN 23-Apr-19 13:58 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/loggers_examples/__init__.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-Apr-19 13:58 super_gradients/examples/loggers_examples/clearml_logger_example.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Apr-19 13:58 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/qat_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Apr-19 13:58 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/non_default_calibrators_example.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/ptq_e2e_example.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
+-rw-r--r--  2.0 unx     4923 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/resnet_qat_example.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/skipping_quantization_example.py
+-rw-r--r--  2.0 unx      832 b- defN 23-Apr-19 13:58 super_gradients/examples/quantization/vanilla_quantize_all_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/regseg_transfer_learning_example/__init__.py
+-rw-r--r--  2.0 unx     2379 b- defN 23-Apr-19 13:58 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/resume_experiment_example/__init__.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Apr-19 13:58 super_gradients/examples/resume_experiment_example/resume_experiment.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_kd_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      655 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
+-rw-r--r--  2.0 unx     1643 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_user_objects/train.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Apr-19 13:58 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
+-rw-r--r--  2.0 unx      118 b- defN 23-Apr-19 13:58 super_gradients/module_interfaces/__init__.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Apr-19 13:58 super_gradients/module_interfaces/module_interfaces.py
+-rw-r--r--  2.0 unx     2589 b- defN 23-Apr-19 13:58 super_gradients/modules/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/modules/all_detection_modules.py
+-rw-r--r--  2.0 unx      617 b- defN 23-Apr-19 13:58 super_gradients/modules/anti_alias.py
+-rw-r--r--  2.0 unx     2073 b- defN 23-Apr-19 13:58 super_gradients/modules/conv_bn_act_block.py
+-rw-r--r--  2.0 unx     1976 b- defN 23-Apr-19 13:58 super_gradients/modules/conv_bn_relu_block.py
+-rw-r--r--  2.0 unx    15129 b- defN 23-Apr-19 13:58 super_gradients/modules/detection_modules.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-Apr-19 13:58 super_gradients/modules/multi_output_modules.py
+-rw-r--r--  2.0 unx     3958 b- defN 23-Apr-19 13:58 super_gradients/modules/pose_estimation_modules.py
+-rw-r--r--  2.0 unx    11642 b- defN 23-Apr-19 13:58 super_gradients/modules/qarepvgg_block.py
+-rw-r--r--  2.0 unx     8544 b- defN 23-Apr-19 13:58 super_gradients/modules/repvgg_block.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-Apr-19 13:58 super_gradients/modules/sampling.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-Apr-19 13:58 super_gradients/modules/se_blocks.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-Apr-19 13:58 super_gradients/modules/skip_connections.py
+-rw-r--r--  2.0 unx     2565 b- defN 23-Apr-19 13:58 super_gradients/modules/utils.py
+-rw-r--r--  2.0 unx      716 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/quantized_skip_connections.py
+-rw-r--r--  2.0 unx     4604 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/quantized_stdc_blocks.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-Apr-19 13:58 super_gradients/modules/quantization/resnet_bottleneck.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/recipes/__init__.py
+-rw-r--r--  2.0 unx     1516 b- defN 23-Apr-19 13:58 super_gradients/recipes/cifar10_resnet.yaml
+-rw-r--r--  2.0 unx     3856 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_ddrnet.yaml
+-rw-r--r--  2.0 unx     4072 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_kd_base.yaml
+-rw-r--r--  2.0 unx     3615 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_pplite_seg50.yaml
+-rw-r--r--  2.0 unx     3514 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_pplite_seg75.yaml
+-rw-r--r--  2.0 unx     2771 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_regseg48.yaml
+-rw-r--r--  2.0 unx     4293 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_segformer.yaml
+-rw-r--r--  2.0 unx      852 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_stdc_base.yaml
+-rw-r--r--  2.0 unx     3175 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_stdc_seg50.yaml
+-rw-r--r--  2.0 unx     3369 b- defN 23-Apr-19 13:58 super_gradients/recipes/cityscapes_stdc_seg75.yaml
+-rw-r--r--  2.0 unx     2063 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
+-rw-r--r--  2.0 unx     3821 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
+-rw-r--r--  2.0 unx     2231 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_pose_pppose_l.yaml
+-rw-r--r--  2.0 unx     2388 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_l.yaml
+-rw-r--r--  2.0 unx     2388 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_m.yaml
+-rw-r--r--  2.0 unx     2274 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_s.yaml
+-rw-r--r--  2.0 unx     2367 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ppyoloe_x.yaml
+-rw-r--r--  2.0 unx     2202 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
+-rw-r--r--  2.0 unx     3053 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco2017_yolox.yaml
+-rw-r--r--  2.0 unx     1649 b- defN 23-Apr-19 13:58 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
+-rw-r--r--  2.0 unx     1418 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_efficientnet.yaml
+-rw-r--r--  2.0 unx     1402 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv2.yaml
+-rw-r--r--  2.0 unx      741 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
+-rw-r--r--  2.0 unx      992 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
+-rw-r--r--  2.0 unx      992 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
+-rw-r--r--  2.0 unx     2387 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_regnetY.yaml
+-rw-r--r--  2.0 unx     1519 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_repvgg.yaml
+-rw-r--r--  2.0 unx     1442 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_resnet50.yaml
+-rw-r--r--  2.0 unx     2998 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_resnet50_kd.yaml
+-rw-r--r--  2.0 unx     1409 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_vit_base.yaml
+-rw-r--r--  2.0 unx     1283 b- defN 23-Apr-19 13:58 super_gradients/recipes/imagenet_vit_large.yaml
+-rw-r--r--  2.0 unx     2226 b- defN 23-Apr-19 13:58 super_gradients/recipes/roboflow_ppyoloe.yaml
+-rw-r--r--  2.0 unx     2134 b- defN 23-Apr-19 13:58 super_gradients/recipes/roboflow_yolox.yaml
+-rw-r--r--  2.0 unx     1520 b- defN 23-Apr-19 13:58 super_gradients/recipes/supervisely_unet.yaml
+-rw-r--r--  2.0 unx     1906 b- defN 23-Apr-19 13:58 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
+-rw-r--r--  2.0 unx     2367 b- defN 23-Apr-19 13:58 super_gradients/recipes/user_recipe_mnist_example.yaml
+-rw-r--r--  2.0 unx     2222 b- defN 23-Apr-19 13:58 super_gradients/recipes/anchors/ssd_anchors.yaml
+-rw-r--r--  2.0 unx      563 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
+-rw-r--r--  2.0 unx      104 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
+-rw-r--r--  2.0 unx      194 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
+-rw-r--r--  2.0 unx      156 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
+-rw-r--r--  2.0 unx      409 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
+-rw-r--r--  2.0 unx      356 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
+-rw-r--r--  2.0 unx      281 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
+-rw-r--r--  2.0 unx     1245 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
+-rw-r--r--  2.0 unx      985 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
+-rw-r--r--  2.0 unx     1112 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
+-rw-r--r--  2.0 unx      196 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
+-rw-r--r--  2.0 unx      204 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
+-rw-r--r--  2.0 unx      352 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
+-rw-r--r--  2.0 unx       89 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
+-rw-r--r--  2.0 unx       95 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
+-rw-r--r--  2.0 unx       32 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
+-rw-r--r--  2.0 unx      655 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
+-rw-r--r--  2.0 unx      605 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
+-rw-r--r--  2.0 unx     1369 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/unet_arch_params.yaml
+-rw-r--r--  2.0 unx     3014 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
+-rw-r--r--  2.0 unx       63 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
+-rw-r--r--  2.0 unx     2393 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolo_arch_params.yaml
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
+-rw-r--r--  2.0 unx      229 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
+-rw-r--r--  2.0 unx      228 b- defN 23-Apr-19 13:58 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
+-rw-r--r--  2.0 unx      611 b- defN 23-Apr-19 13:58 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
+-rw-r--r--  2.0 unx       72 b- defN 23-Apr-19 13:58 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/recipes/conversion_params/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Apr-19 13:58 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
+-rw-r--r--  2.0 unx     2040 b- defN 23-Apr-19 13:58 super_gradients/recipes/conversion_params/default_conversion_params.yaml
+-rw-r--r--  2.0 unx      869 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
+-rw-r--r--  2.0 unx     1530 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
+-rw-r--r--  2.0 unx      615 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
+-rw-r--r--  2.0 unx      525 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      706 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx      644 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
+-rw-r--r--  2.0 unx      721 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
+-rw-r--r--  2.0 unx      709 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
+-rw-r--r--  2.0 unx      708 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx     3946 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     3661 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml
+-rw-r--r--  2.0 unx     4202 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
+-rw-r--r--  2.0 unx     3590 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
+-rw-r--r--  2.0 unx     2461 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
+-rw-r--r--  2.0 unx      405 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx      931 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx      732 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
+-rw-r--r--  2.0 unx      142 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
+-rw-r--r--  2.0 unx      734 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
+-rw-r--r--  2.0 unx     1059 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
+-rw-r--r--  2.0 unx     1093 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
+-rw-r--r--  2.0 unx      845 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     1762 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
+-rw-r--r--  2.0 unx      149 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     1571 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     1414 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     3398 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx      961 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
+-rw-r--r--  2.0 unx      559 b- defN 23-Apr-19 13:58 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx     1155 b- defN 23-Apr-19 13:58 super_gradients/recipes/quantization_params/default_quantization_params.yaml
+-rw-r--r--  2.0 unx      591 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
+-rw-r--r--  2.0 unx      700 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
+-rw-r--r--  2.0 unx      877 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
+-rw-r--r--  2.0 unx      723 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
+-rw-r--r--  2.0 unx      956 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
+-rw-r--r--  2.0 unx      461 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
+-rw-r--r--  2.0 unx     5459 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/default_train_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
+-rw-r--r--  2.0 unx      742 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
+-rw-r--r--  2.0 unx      549 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
+-rw-r--r--  2.0 unx      795 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
+-rw-r--r--  2.0 unx      476 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
+-rw-r--r--  2.0 unx      484 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
+-rw-r--r--  2.0 unx      522 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
+-rw-r--r--  2.0 unx      602 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
+-rw-r--r--  2.0 unx      519 b- defN 23-Apr-19 13:58 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-19 13:58 super_gradients/sanity_check/__init__.py
+-rw-r--r--  2.0 unx     5262 b- defN 23-Apr-19 13:58 super_gradients/sanity_check/env_sanity_check.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Apr-19 13:58 super_gradients/training/__init__.py
+-rw-r--r--  2.0 unx     4155 b- defN 23-Apr-19 13:58 super_gradients/training/params.py
+-rw-r--r--  2.0 unx     5696 b- defN 23-Apr-19 13:58 super_gradients/training/pretrained_models.py
+-rw-r--r--  2.0 unx     3228 b- defN 23-Apr-19 13:58 super_gradients/training/dataloaders/__init__.py
+-rw-r--r--  2.0 unx    31443 b- defN 23-Apr-19 13:58 super_gradients/training/dataloaders/dataloaders.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/__init__.py
+-rw-r--r--  2.0 unx    14162 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/auto_augment.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_augmentation.py
+-rw-r--r--  2.0 unx     3484 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/datasets_conf.py
+-rw-r--r--  2.0 unx    30279 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/datasets_utils.py
+-rw-r--r--  2.0 unx    14663 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/mixup.py
+-rw-r--r--  2.0 unx    11746 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/sg_dataset.py
+-rw-r--r--  2.0 unx      252 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/classification_datasets/__init__.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/classification_datasets/cifar.py
+-rw-r--r--  2.0 unx     1706 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
+-rw-r--r--  2.0 unx      862 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/__init__.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/default_formats.py
+-rw-r--r--  2.0 unx     3071 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/format_converter.py
+-rw-r--r--  2.0 unx     7928 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/formats.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
+-rw-r--r--  2.0 unx     2674 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
+-rw-r--r--  2.0 unx     5094 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
+-rw-r--r--  2.0 unx     2089 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
+-rw-r--r--  2.0 unx     2948 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
+-rw-r--r--  2.0 unx      575 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
+-rw-r--r--  2.0 unx      683 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/__init__.py
+-rw-r--r--  2.0 unx     2505 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/coco_detection.py
+-rw-r--r--  2.0 unx     9258 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
+-rw-r--r--  2.0 unx    25694 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/detection_dataset.py
+-rw-r--r--  2.0 unx    11353 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
+-rw-r--r--  2.0 unx    10390 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
+-rw-r--r--  2.0 unx    18882 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
+-rw-r--r--  2.0 unx     3504 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
+-rw-r--r--  2.0 unx      502 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
+-rw-r--r--  2.0 unx     4910 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
+-rw-r--r--  2.0 unx     9066 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
+-rw-r--r--  2.0 unx     5929 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
+-rw-r--r--  2.0 unx    10167 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/samplers/__init__.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/samplers/infinite_sampler.py
+-rw-r--r--  2.0 unx     4809 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
+-rw-r--r--  2.0 unx     1037 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/__init__.py
+-rw-r--r--  2.0 unx     6714 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
+-rw-r--r--  2.0 unx     7717 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
+-rw-r--r--  2.0 unx    11146 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
+-rw-r--r--  2.0 unx     8470 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-Apr-19 13:58 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/dataset_exceptions.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/kd_trainer_exceptions.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/loss_exceptions.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Apr-19 13:58 super_gradients/training/exceptions/sg_trainer_exceptions.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Apr-19 13:58 super_gradients/training/kd_trainer/__init__.py
+-rw-r--r--  2.0 unx    16582 b- defN 23-Apr-19 13:58 super_gradients/training/kd_trainer/kd_trainer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/legacy/__init__.py
+-rw-r--r--  2.0 unx     4198 b- defN 23-Apr-19 13:58 super_gradients/training/legacy/utils.py
+-rw-r--r--  2.0 unx     1476 b- defN 23-Apr-19 13:58 super_gradients/training/losses/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/losses/all_losses.py
+-rw-r--r--  2.0 unx     1219 b- defN 23-Apr-19 13:58 super_gradients/training/losses/bce_dice_loss.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Apr-19 13:58 super_gradients/training/losses/bce_loss.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-Apr-19 13:58 super_gradients/training/losses/cwd_loss.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ddrnet_loss.py
+-rw-r--r--  2.0 unx     3377 b- defN 23-Apr-19 13:58 super_gradients/training/losses/dekr_loss.py
+-rw-r--r--  2.0 unx     5618 b- defN 23-Apr-19 13:58 super_gradients/training/losses/dice_ce_edge_loss.py
+-rw-r--r--  2.0 unx     5208 b- defN 23-Apr-19 13:58 super_gradients/training/losses/dice_loss.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-Apr-19 13:58 super_gradients/training/losses/focal_loss.py
+-rw-r--r--  2.0 unx     5051 b- defN 23-Apr-19 13:58 super_gradients/training/losses/iou_loss.py
+-rw-r--r--  2.0 unx     2176 b- defN 23-Apr-19 13:58 super_gradients/training/losses/kd_losses.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-Apr-19 13:58 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
+-rw-r--r--  2.0 unx      550 b- defN 23-Apr-19 13:58 super_gradients/training/losses/loss_utils.py
+-rw-r--r--  2.0 unx     3854 b- defN 23-Apr-19 13:58 super_gradients/training/losses/mask_loss.py
+-rw-r--r--  2.0 unx     4129 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ohem_ce_loss.py
+-rw-r--r--  2.0 unx    41319 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ppyolo_loss.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Apr-19 13:58 super_gradients/training/losses/r_squared_loss.py
+-rw-r--r--  2.0 unx     3453 b- defN 23-Apr-19 13:58 super_gradients/training/losses/seg_kd_loss.py
+-rw-r--r--  2.0 unx     1650 b- defN 23-Apr-19 13:58 super_gradients/training/losses/shelfnet_ohem_loss.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-Apr-19 13:58 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
+-rw-r--r--  2.0 unx     8794 b- defN 23-Apr-19 13:58 super_gradients/training/losses/ssd_loss.py
+-rw-r--r--  2.0 unx     9721 b- defN 23-Apr-19 13:58 super_gradients/training/losses/stdc_loss.py
+-rw-r--r--  2.0 unx     5771 b- defN 23-Apr-19 13:58 super_gradients/training/losses/structure_loss.py
+-rw-r--r--  2.0 unx    50149 b- defN 23-Apr-19 13:58 super_gradients/training/losses/yolox_loss.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/all_metrics.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/classification_metrics.py
+-rw-r--r--  2.0 unx    10741 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/detection_metrics.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/metric_utils.py
+-rw-r--r--  2.0 unx    15346 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/pose_estimation_metrics.py
+-rw-r--r--  2.0 unx    11454 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/pose_estimation_utils.py
+-rw-r--r--  2.0 unx    11935 b- defN 23-Apr-19 13:58 super_gradients/training/metrics/segmentation_metrics.py
+-rw-r--r--  2.0 unx     8368 b- defN 23-Apr-19 13:58 super_gradients/training/models/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Apr-19 13:58 super_gradients/training/models/arch_params_factory.py
+-rw-r--r--  2.0 unx     7060 b- defN 23-Apr-19 13:58 super_gradients/training/models/conversion.py
+-rw-r--r--  2.0 unx    11875 b- defN 23-Apr-19 13:58 super_gradients/training/models/model_factory.py
+-rw-r--r--  2.0 unx    10850 b- defN 23-Apr-19 13:58 super_gradients/training/models/prediction_results.py
+-rw-r--r--  2.0 unx     2054 b- defN 23-Apr-19 13:58 super_gradients/training/models/predictions.py
+-rw-r--r--  2.0 unx     2998 b- defN 23-Apr-19 13:58 super_gradients/training/models/sg_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/__init__.py
+-rw-r--r--  2.0 unx    20025 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/beit.py
+-rw-r--r--  2.0 unx     7472 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/densenet.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/dpn.py
+-rw-r--r--  2.0 unx    36745 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/efficientnet.py
+-rw-r--r--  2.0 unx     8862 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/googlenet.py
+-rw-r--r--  2.0 unx      798 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/lenet.py
+-rw-r--r--  2.0 unx     2407 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/mobilenet.py
+-rw-r--r--  2.0 unx     9472 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/mobilenetv2.py
+-rw-r--r--  2.0 unx     8696 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/mobilenetv3.py
+-rw-r--r--  2.0 unx     4339 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/pnasnet.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/preact_resnet.py
+-rw-r--r--  2.0 unx    13599 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/regnet.py
+-rw-r--r--  2.0 unx     7924 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/repvgg.py
+-rw-r--r--  2.0 unx    15042 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/resnet.py
+-rw-r--r--  2.0 unx     6294 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/resnext.py
+-rw-r--r--  2.0 unx     4134 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/senet.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/shufflenet.py
+-rw-r--r--  2.0 unx     9768 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/shufflenetv2.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/vgg.py
+-rw-r--r--  2.0 unx     9210 b- defN 23-Apr-19 13:58 super_gradients/training/models/classification_models/vit.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/__init__.py
+-rw-r--r--  2.0 unx     9502 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/csp_darknet53.py
+-rw-r--r--  2.0 unx     9814 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/csp_resnet.py
+-rw-r--r--  2.0 unx     8784 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/customizable_detector.py
+-rw-r--r--  2.0 unx     4746 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/darknet53.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/ssd.py
+-rw-r--r--  2.0 unx    29459 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/yolo_base.py
+-rw-r--r--  2.0 unx     2459 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/yolox.py
+-rw-r--r--  2.0 unx      155 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
+-rw-r--r--  2.0 unx     6984 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
+-rw-r--r--  2.0 unx     3487 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
+-rw-r--r--  2.0 unx     8240 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
+-rw-r--r--  2.0 unx    12334 b- defN 23-Apr-19 13:58 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/kd_modules/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Apr-19 13:58 super_gradients/training/models/kd_modules/kd_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/__init__.py
+-rw-r--r--  2.0 unx    21231 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
+-rw-r--r--  2.0 unx     1294 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-Apr-19 13:58 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/__init__.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/common.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/context_modules.py
+-rw-r--r--  2.0 unx    27896 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/ddrnet.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
+-rw-r--r--  2.0 unx    21760 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/laddernet.py
+-rw-r--r--  2.0 unx    15648 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/ppliteseg.py
+-rw-r--r--  2.0 unx    14424 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/regseg.py
+-rw-r--r--  2.0 unx    20334 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/segformer.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/segmentation_module.py
+-rw-r--r--  2.0 unx    24833 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/shelfnet.py
+-rw-r--r--  2.0 unx    29005 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/stdc.py
+-rw-r--r--  2.0 unx      260 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/__init__.py
+-rw-r--r--  2.0 unx    12324 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/unet.py
+-rw-r--r--  2.0 unx     8305 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
+-rw-r--r--  2.0 unx    13292 b- defN 23-Apr-19 13:58 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Apr-19 13:58 super_gradients/training/models/user_models/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/pipelines/__init__.py
+-rw-r--r--  2.0 unx    14399 b- defN 23-Apr-19 13:58 super_gradients/training/pipelines/pipelines.py
+-rw-r--r--  2.0 unx      393 b- defN 23-Apr-19 13:58 super_gradients/training/pre_launch_callbacks/__init__.py
+-rw-r--r--  2.0 unx    13955 b- defN 23-Apr-19 13:58 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Apr-19 13:58 super_gradients/training/processing/__init__.py
+-rw-r--r--  2.0 unx    13178 b- defN 23-Apr-19 13:58 super_gradients/training/processing/processing.py
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-19 13:58 super_gradients/training/qat_trainer/__init__.py
+-rw-r--r--  2.0 unx     9896 b- defN 23-Apr-19 13:58 super_gradients/training/qat_trainer/qat_trainer.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Apr-19 13:58 super_gradients/training/sg_trainer/__init__.py
+-rw-r--r--  2.0 unx    97370 b- defN 23-Apr-19 13:58 super_gradients/training/sg_trainer/sg_trainer.py
+-rw-r--r--  2.0 unx     1685 b- defN 23-Apr-19 13:58 super_gradients/training/training_hyperparams/__init__.py
+-rw-r--r--  2.0 unx     3774 b- defN 23-Apr-19 13:58 super_gradients/training/training_hyperparams/training_hyperparams.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/all_transforms.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/keypoint_transforms.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/pipeline_adaptors.py
+-rw-r--r--  2.0 unx    55085 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/transforms.py
+-rw-r--r--  2.0 unx     6048 b- defN 23-Apr-19 13:58 super_gradients/training/transforms/utils.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Apr-19 13:58 super_gradients/training/utils/__init__.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-Apr-19 13:58 super_gradients/training/utils/activations_utils.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Apr-19 13:58 super_gradients/training/utils/bbox_utils.py
+-rw-r--r--  2.0 unx    14834 b- defN 23-Apr-19 13:58 super_gradients/training/utils/checkpoint_utils.py
+-rw-r--r--  2.0 unx     9794 b- defN 23-Apr-19 13:58 super_gradients/training/utils/config_utils.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Apr-19 13:58 super_gradients/training/utils/deprecated_utils.py
+-rw-r--r--  2.0 unx    53611 b- defN 23-Apr-19 13:58 super_gradients/training/utils/detection_utils.py
+-rw-r--r--  2.0 unx    16195 b- defN 23-Apr-19 13:58 super_gradients/training/utils/distributed_training_utils.py
+-rw-r--r--  2.0 unx     6352 b- defN 23-Apr-19 13:58 super_gradients/training/utils/early_stopping.py
+-rw-r--r--  2.0 unx     9322 b- defN 23-Apr-19 13:58 super_gradients/training/utils/ema.py
+-rw-r--r--  2.0 unx     2610 b- defN 23-Apr-19 13:58 super_gradients/training/utils/ema_decay_schedules.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-19 13:58 super_gradients/training/utils/export_utils.py
+-rw-r--r--  2.0 unx     7508 b- defN 23-Apr-19 13:58 super_gradients/training/utils/get_model_stats.py
+-rw-r--r--  2.0 unx      771 b- defN 23-Apr-19 13:58 super_gradients/training/utils/kd_trainer_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/utils/load_image.py
+-rw-r--r--  2.0 unx     5827 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizer_utils.py
+-rw-r--r--  2.0 unx      839 b- defN 23-Apr-19 13:58 super_gradients/training/utils/regularization_utils.py
+-rw-r--r--  2.0 unx    10388 b- defN 23-Apr-19 13:58 super_gradients/training/utils/segmentation_utils.py
+-rw-r--r--  2.0 unx    19625 b- defN 23-Apr-19 13:58 super_gradients/training/utils/sg_trainer_utils.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Apr-19 13:58 super_gradients/training/utils/ssd_utils.py
+-rw-r--r--  2.0 unx    18273 b- defN 23-Apr-19 13:58 super_gradients/training/utils/utils.py
+-rw-r--r--  2.0 unx      303 b- defN 23-Apr-19 13:58 super_gradients/training/utils/version_utils.py
+-rw-r--r--  2.0 unx     6209 b- defN 23-Apr-19 13:58 super_gradients/training/utils/weight_averaging_utils.py
+-rw-r--r--  2.0 unx     2030 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/all_callbacks.py
+-rw-r--r--  2.0 unx    20126 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/base_callbacks.py
+-rw-r--r--  2.0 unx    32630 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/callbacks.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-Apr-19 13:58 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/__init__.py
+-rw-r--r--  2.0 unx     5775 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/image.py
+-rw-r--r--  2.0 unx     4046 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/stream.py
+-rw-r--r--  2.0 unx     5360 b- defN 23-Apr-19 13:58 super_gradients/training/utils/media/video.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/__init__.py
+-rw-r--r--  2.0 unx     9760 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/lamb.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/lion.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-Apr-19 13:58 super_gradients/training/utils/optimizers/rmsprop_tf.py
+-rw-r--r--  2.0 unx      213 b- defN 23-Apr-19 13:58 super_gradients/training/utils/pose_estimation/__init__.py
+-rw-r--r--  2.0 unx    11167 b- defN 23-Apr-19 13:58 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
+-rw-r--r--  2.0 unx     7140 b- defN 23-Apr-19 13:58 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
+-rw-r--r--  2.0 unx      387 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/__init__.py
+-rw-r--r--  2.0 unx     6271 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/calibrator.py
+-rw-r--r--  2.0 unx     8417 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/core.py
+-rw-r--r--  2.0 unx     2196 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/export.py
+-rw-r--r--  2.0 unx    17062 b- defN 23-Apr-19 13:58 super_gradients/training/utils/quantization/selective_quantization_utils.py
+-rw-r--r--  2.0 unx    11341 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    34221 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    61129 b- defN 23-Apr-19 13:59 super_gradients-3.0.9.dist-info/RECORD
+529 files, 2735180 bytes uncompressed, 835793 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -228,14 +228,17 @@
 
 Filename: super_gradients/common/factories/optimizers_type_factory.py
 Comment: 
 
 Filename: super_gradients/common/factories/pre_launch_callbacks_factory.py
 Comment: 
 
+Filename: super_gradients/common/factories/processing_factory.py
+Comment: 
+
 Filename: super_gradients/common/factories/samplers_factory.py
 Comment: 
 
 Filename: super_gradients/common/factories/target_generator_factory.py
 Comment: 
 
 Filename: super_gradients/common/factories/transforms_factory.py
@@ -411,14 +414,20 @@
 
 Filename: super_gradients/examples/train_from_recipe_with_user_objects/train.py
 Comment: 
 
 Filename: super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
 Comment: 
 
+Filename: super_gradients/module_interfaces/__init__.py
+Comment: 
+
+Filename: super_gradients/module_interfaces/module_interfaces.py
+Comment: 
+
 Filename: super_gradients/modules/__init__.py
 Comment: 
 
 Filename: super_gradients/modules/all_detection_modules.py
 Comment: 
 
 Filename: super_gradients/modules/anti_alias.py
@@ -486,14 +495,17 @@
 
 Filename: super_gradients/recipes/cityscapes_pplite_seg75.yaml
 Comment: 
 
 Filename: super_gradients/recipes/cityscapes_regseg48.yaml
 Comment: 
 
+Filename: super_gradients/recipes/cityscapes_segformer.yaml
+Comment: 
+
 Filename: super_gradients/recipes/cityscapes_stdc_base.yaml
 Comment: 
 
 Filename: super_gradients/recipes/cityscapes_stdc_seg50.yaml
 Comment: 
 
 Filename: super_gradients/recipes/cityscapes_stdc_seg75.yaml
@@ -558,14 +570,20 @@
 
 Filename: super_gradients/recipes/imagenet_vit_base.yaml
 Comment: 
 
 Filename: super_gradients/recipes/imagenet_vit_large.yaml
 Comment: 
 
+Filename: super_gradients/recipes/roboflow_ppyoloe.yaml
+Comment: 
+
+Filename: super_gradients/recipes/roboflow_yolox.yaml
+Comment: 
+
 Filename: super_gradients/recipes/supervisely_unet.yaml
 Comment: 
 
 Filename: super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
 Comment: 
 
 Filename: super_gradients/recipes/user_recipe_mnist_example.yaml
@@ -744,14 +762,17 @@
 
 Filename: super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
@@ -807,14 +828,17 @@
 
 Filename: super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/quantization_params/default_quantization_params.yaml
@@ -978,14 +1002,29 @@
 
 Filename: super_gradients/training/datasets/detection_datasets/detection_dataset.py
 Comment: 
 
 Filename: super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
 Comment: 
 
+Filename: super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
+Comment: 
+
+Filename: super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
+Comment: 
+
+Filename: super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
+Comment: 
+
+Filename: super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
+Comment: 
+
+Filename: super_gradients/training/datasets/detection_datasets/roboflow/utils.py
+Comment: 
+
 Filename: super_gradients/training/datasets/pose_estimation_datasets/__init__.py
 Comment: 
 
 Filename: super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
 Comment: 
 
 Filename: super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
@@ -1161,14 +1200,20 @@
 
 Filename: super_gradients/training/models/conversion.py
 Comment: 
 
 Filename: super_gradients/training/models/model_factory.py
 Comment: 
 
+Filename: super_gradients/training/models/prediction_results.py
+Comment: 
+
+Filename: super_gradients/training/models/predictions.py
+Comment: 
+
 Filename: super_gradients/training/models/sg_module.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/__init__.py
 Comment: 
 
 Filename: super_gradients/training/models/classification_models/beit.py
@@ -1308,14 +1353,17 @@
 
 Filename: super_gradients/training/models/segmentation_models/ppliteseg.py
 Comment: 
 
 Filename: super_gradients/training/models/segmentation_models/regseg.py
 Comment: 
 
+Filename: super_gradients/training/models/segmentation_models/segformer.py
+Comment: 
+
 Filename: super_gradients/training/models/segmentation_models/segmentation_module.py
 Comment: 
 
 Filename: super_gradients/training/models/segmentation_models/shelfnet.py
 Comment: 
 
 Filename: super_gradients/training/models/segmentation_models/stdc.py
@@ -1332,20 +1380,32 @@
 
 Filename: super_gradients/training/models/segmentation_models/unet/unet_encoder.py
 Comment: 
 
 Filename: super_gradients/training/models/user_models/__init__.py
 Comment: 
 
+Filename: super_gradients/training/pipelines/__init__.py
+Comment: 
+
+Filename: super_gradients/training/pipelines/pipelines.py
+Comment: 
+
 Filename: super_gradients/training/pre_launch_callbacks/__init__.py
 Comment: 
 
 Filename: super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
 Comment: 
 
+Filename: super_gradients/training/processing/__init__.py
+Comment: 
+
+Filename: super_gradients/training/processing/processing.py
+Comment: 
+
 Filename: super_gradients/training/qat_trainer/__init__.py
 Comment: 
 
 Filename: super_gradients/training/qat_trainer/qat_trainer.py
 Comment: 
 
 Filename: super_gradients/training/sg_trainer/__init__.py
@@ -1371,14 +1431,17 @@
 
 Filename: super_gradients/training/transforms/pipeline_adaptors.py
 Comment: 
 
 Filename: super_gradients/training/transforms/transforms.py
 Comment: 
 
+Filename: super_gradients/training/transforms/utils.py
+Comment: 
+
 Filename: super_gradients/training/utils/__init__.py
 Comment: 
 
 Filename: super_gradients/training/utils/activations_utils.py
 Comment: 
 
 Filename: super_gradients/training/utils/bbox_utils.py
@@ -1413,14 +1476,17 @@
 
 Filename: super_gradients/training/utils/get_model_stats.py
 Comment: 
 
 Filename: super_gradients/training/utils/kd_trainer_utils.py
 Comment: 
 
+Filename: super_gradients/training/utils/load_image.py
+Comment: 
+
 Filename: super_gradients/training/utils/optimizer_utils.py
 Comment: 
 
 Filename: super_gradients/training/utils/regularization_utils.py
 Comment: 
 
 Filename: super_gradients/training/utils/segmentation_utils.py
@@ -1452,14 +1518,26 @@
 
 Filename: super_gradients/training/utils/callbacks/callbacks.py
 Comment: 
 
 Filename: super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
 Comment: 
 
+Filename: super_gradients/training/utils/media/__init__.py
+Comment: 
+
+Filename: super_gradients/training/utils/media/image.py
+Comment: 
+
+Filename: super_gradients/training/utils/media/stream.py
+Comment: 
+
+Filename: super_gradients/training/utils/media/video.py
+Comment: 
+
 Filename: super_gradients/training/utils/optimizers/__init__.py
 Comment: 
 
 Filename: super_gradients/training/utils/optimizers/lamb.py
 Comment: 
 
 Filename: super_gradients/training/utils/optimizers/lion.py
@@ -1488,23 +1566,23 @@
 
 Filename: super_gradients/training/utils/quantization/export.py
 Comment: 
 
 Filename: super_gradients/training/utils/quantization/selective_quantization_utils.py
 Comment: 
 
-Filename: super_gradients-3.0.8.dist-info/LICENSE.md
+Filename: super_gradients-3.0.9.dist-info/LICENSE.md
 Comment: 
 
-Filename: super_gradients-3.0.8.dist-info/METADATA
+Filename: super_gradients-3.0.9.dist-info/METADATA
 Comment: 
 
-Filename: super_gradients-3.0.8.dist-info/WHEEL
+Filename: super_gradients-3.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: super_gradients-3.0.8.dist-info/top_level.txt
+Filename: super_gradients-3.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: super_gradients-3.0.8.dist-info/RECORD
+Filename: super_gradients-3.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## super_gradients/__init__.py

```diff
@@ -20,10 +20,10 @@
     "is_distributed",
     "train_from_recipe",
     "train_from_kd_recipe",
     "env_sanity_check",
     "setup_device",
 ]
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 
 env_sanity_check()
```

## super_gradients/common/object_names.py

```diff
@@ -139,14 +139,15 @@
     MODEL_CONVERSION_CHECK = "ModelConversionCheckCallback"
     EARLY_STOP = "EarlyStop"
     DETECTION_MULTISCALE_PREPREDICTION = "DetectionMultiscalePrePredictionCallback"
     YOLOX_TRAINING_STAGE_SWITCH = "YoloXTrainingStageSwitchCallback"
     PPYOLOE_TRAINING_STAGE_SWITCH = "PPYoloETrainingStageSwitchCallback"
     DETECTION_VISUALIZATION_CALLBACK = "DetectionVisualizationCallback"
     DEKR_VISUALIZATION = "DEKRVisualizationCallback"
+    ROBOFLOW_RESULT_CALLBACK = "RoboflowResultCallback"
 
 
 class LRSchedulers:
     """Static class to hold all the supported LR Scheduler names"""
 
     STEP = "step"
     POLY = "poly"
@@ -288,14 +289,20 @@
     UNET = "unet"
     STDC_CUSTOM = "stdc_custom"
     STDC_CUSTOM_CLS = "stdc_custom_cls"
     PP_YOLOE_S = "ppyoloe_s"
     PP_YOLOE_M = "ppyoloe_m"
     PP_YOLOE_L = "ppyoloe_l"
     PP_YOLOE_X = "ppyoloe_x"
+    SEGFORMER_B0 = "segformer_b0"
+    SEGFORMER_B1 = "segformer_b1"
+    SEGFORMER_B2 = "segformer_b2"
+    SEGFORMER_B3 = "segformer_b3"
+    SEGFORMER_B4 = "segformer_b4"
+    SEGFORMER_B5 = "segformer_b5"
 
     DEKR_CUSTOM = "dekr_custom"
     DEKR_W32_NO_DC = "dekr_w32_no_dc"
     POSE_PP_YOLO_L = "pose_ppyolo_l"
     POSE_DDRNET_39 = "pose_ddrnet39"
 
 
@@ -367,14 +374,16 @@
     PASCAL_AUG_SEGMENTATION_VAL = "pascal_aug_segmentation_val"
     PASCAL_VOC_SEGMENTATION_TRAIN = "pascal_voc_segmentation_train"
     PASCAL_VOC_SEGMENTATION_VAL = "pascal_voc_segmentation_val"
     SUPERVISELY_PERSONS_TRAIN = "supervisely_persons_train"
     SUPERVISELY_PERSONS_VAL = "supervisely_persons_val"
     PASCAL_VOC_DETECTION_TRAIN = "pascal_voc_detection_train"
     PASCAL_VOC_DETECTION_VAL = "pascal_voc_detection_val"
+    ROBOFLOW_TRAIN_BASE = "roboflow_train_yolox"
+    ROBOFLOW_VAL_BASE = "roboflow_val_yolox"
 
 
 class Datasets:
     CIFAR_10 = "Cifar10"
     CIFAR_100 = "Cifar100"
     IMAGENET_DATASET = "ImageNetDataset"
     COCO_DETECTION_DATASET = "COCODetectionDataset"
@@ -385,7 +394,19 @@
     PASCAL_AUG_2012_SEGMENTATION_DATASET = "PascalAUG2012SegmentationDataSet"
     PASCAL_VOC_2012_SEGMENTATION_DATASET = "PascalVOC2012SegmentationDataSet"
     CITYSCAPES_DATASET = "CityscapesDataset"
     MAPILLARY_DATASET = "MapillaryDataset"
     SUPERVISELY_PERSONS_DATASET = "SuperviselyPersonsDataset"
     PASCAL_VOC_AND_AUG_UNIFIED_DATASET = "PascalVOCAndAUGUnifiedDataset"
     COCO_KEY_POINTS_DATASET = "COCOKeypointsDataset"
+
+
+class Processings:
+    StandardizeImage = "StandardizeImage"
+    DetectionCenterPadding = "DetectionCenterPadding"
+    DetectionLongestMaxSizeRescale = "DetectionLongestMaxSizeRescale"
+    DetectionBottomRightPadding = "DetectionBottomRightPadding"
+    ImagePermute = "ImagePermute"
+    DetectionRescale = "DetectionRescale"
+    ReverseImageChannels = "ReverseImageChannels"
+    NormalizeImage = "NormalizeImage"
+    ComposeProcessing = "ComposeProcessing"
```

## super_gradients/common/environment/omegaconf_utils.py

```diff
@@ -20,14 +20,19 @@
 
 def hydra_output_dir_resolver(ckpt_root_dir: str, experiment_name: str) -> str:
     return get_checkpoints_dir_path(experiment_name=experiment_name, ckpt_root_dir=ckpt_root_dir)
 
 
 def register_hydra_resolvers():
     """Register all the hydra resolvers required for the super-gradients recipes."""
+
+    from super_gradients.training.datasets.detection_datasets.roboflow.utils import get_dataset_num_classes
+
     OmegaConf.register_new_resolver("hydra_output_dir", hydra_output_dir_resolver, replace=True)
     OmegaConf.register_new_resolver("class", lambda *args: get_cls(*args), replace=True)
     OmegaConf.register_new_resolver("add", lambda *args: sum(args), replace=True)
     OmegaConf.register_new_resolver("cond", lambda boolean, x, y: x if boolean else y, replace=True)
     OmegaConf.register_new_resolver("getitem", lambda container, key: container[key], replace=True)  # get item from a container (list, dict...)
     OmegaConf.register_new_resolver("first", lambda lst: lst[0], replace=True)  # get the first item from a list
     OmegaConf.register_new_resolver("last", lambda lst: lst[-1], replace=True)  # get the last item from a list
+
+    OmegaConf.register_new_resolver("roboflow_dataset_num_classes", get_dataset_num_classes, replace=True)
```

## super_gradients/common/registry/registry.py

```diff
@@ -141,7 +141,10 @@
 OPTIMIZERS = {
     Optimizers.SGD: optim.SGD,
     Optimizers.ADAM: optim.Adam,
     Optimizers.ADAMW: optim.AdamW,
     Optimizers.RMS_PROP: optim.RMSprop,
 }
 register_optimizer = create_register_decorator(registry=OPTIMIZERS)
+
+PROCESSINGS = {}
+register_processing = create_register_decorator(registry=PROCESSINGS)
```

## super_gradients/recipes/arch_params/yolox_s_arch_params.yaml

 * *Ordering differences only*

```diff
@@ -5,8 +5,8 @@
   _target_: super_gradients.training.utils.detection_utils.Anchors
   anchors_list: [[0,0], [0,0], [0,0]]
   strides: [8, 16, 32]
 
 yolo_type: 'yoloX'
 
 depth_mult_factor: 0.33
-width_mult_factor: 0.5
+width_mult_factor: 0.5
```

## super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml

```diff
@@ -65,15 +65,15 @@
     - DetectionRGB2BGR:
         prob: 1
     - DetectionPadToSize:
         output_size: [640, 640]
         pad_value: 114
     - DetectionStandardizeImage:
         max_value: 255.
-    - DetectionImagePermute:
+    - DetectionImagePermute
     - DetectionTargetsFormatTransform:
         max_targets: 50
         input_dim: [640, 640]
         output_format: LABEL_NORMALIZED_CXCYWH
   tight_box_rotation: False
   class_inclusion_list:
   max_num_samples:
```

## super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml

 * *Ordering differences only*

```diff
@@ -20,8 +20,8 @@
     - CenterCrop:
         size: 56
     - ToTensor
     - Normalize:
         mean: [0.4802, 0.4481, 0.3975]
         std: [0.2770, 0.2691, 0.2821]
 
-_convert_: all
+_convert_: all
```

## super_gradients/training/dataloaders/dataloaders.py

```diff
@@ -1,27 +1,27 @@
 from typing import Dict, Mapping
 
 import hydra
 import numpy as np
 import torch
-from torch.utils.data import BatchSampler, DataLoader, TensorDataset
+from torch.utils.data import BatchSampler, DataLoader, TensorDataset, RandomSampler
 
 import super_gradients
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.registry.registry import register_dataloader, ALL_DATALOADERS
 from super_gradients.common.factories.collate_functions_factory import CollateFunctionsFactory
 from super_gradients.common.factories.datasets_factory import DatasetsFactory
 from super_gradients.common.factories.samplers_factory import SamplersFactory
 from super_gradients.common.object_names import Dataloaders
 from super_gradients.training.datasets import ImageNetDataset
 from super_gradients.training.datasets.classification_datasets.cifar import (
     Cifar10,
     Cifar100,
 )
-from super_gradients.training.datasets.detection_datasets import COCODetectionDataset
+from super_gradients.training.datasets.detection_datasets import COCODetectionDataset, RoboflowDetectionDataset
 from super_gradients.training.datasets.detection_datasets.pascal_voc_detection import (
     PascalVOCUnifiedDetectionTrainDataset,
     PascalVOCDetectionDataset,
 )
 from super_gradients.training.datasets.pose_estimation_datasets import COCOKeypointsDataset
 from super_gradients.training.datasets.segmentation_datasets import (
     CityscapesDataset,
@@ -92,14 +92,22 @@
 
 def _process_dataloader_params(cfg, dataloader_params, dataset, train):
     default_dataloader_params = cfg.train_dataloader_params if train else cfg.val_dataloader_params
     default_dataloader_params = hydra.utils.instantiate(default_dataloader_params)
     dataloader_params = _process_sampler_params(dataloader_params, dataset, default_dataloader_params)
     dataloader_params = _process_collate_fn_params(dataloader_params)
 
+    # The following check is needed to gracefully handle the rare but possible case when the dataset length
+    # is less than the number of workers. In this case DataLoader will crash.
+    # So we clamp the number of workers to not exceed the dataset length.
+    num_workers = get_param(dataloader_params, "num_workers")
+    if num_workers is not None and num_workers > 0:
+        num_workers = min(num_workers, len(dataset))
+        dataloader_params["num_workers"] = num_workers
+
     return dataloader_params
 
 
 def _process_collate_fn_params(dataloader_params):
     if get_param(dataloader_params, "collate_fn") is not None:
         dataloader_params["collate_fn"] = CollateFunctionsFactory().get(dataloader_params["collate_fn"])
 
@@ -110,14 +118,21 @@
     is_dist = super_gradients.is_distributed()
     dataloader_params = override_default_params_without_nones(dataloader_params, default_dataloader_params)
     if get_param(dataloader_params, "sampler") is not None:
         dataloader_params = _instantiate_sampler(dataset, dataloader_params)
     elif is_dist:
         dataloader_params["sampler"] = {"DistributedSampler": {}}
         dataloader_params = _instantiate_sampler(dataset, dataloader_params)
+    elif get_param(dataloader_params, "min_samples") is not None:
+        min_samples = dataloader_params.pop("min_samples")
+        if len(dataset) < min_samples:
+            dataloader_params["sampler"] = RandomSampler(dataset, replacement=True, num_samples=min_samples)
+            if "shuffle" in dataloader_params.keys():
+                dataloader_params.pop("shuffle")
+            logger.info(f"Using min_samples={min_samples}")
     if get_param(dataloader_params, "batch_sampler"):
         sampler = dataloader_params.pop("sampler")
         batch_size = dataloader_params.pop("batch_size")
         if "drop_last" in dataloader_params:
             drop_last = dataloader_params.pop("drop_last")
         else:
             drop_last = dataloader_params["drop_last"]
@@ -229,14 +244,36 @@
         dataset_cls=COCODetectionDataset,
         train=False,
         dataset_params=dataset_params,
         dataloader_params=dataloader_params,
     )
 
 
+@register_dataloader(Dataloaders.ROBOFLOW_TRAIN_BASE)
+def roboflow_train_yolox(dataset_params: Dict = None, dataloader_params: Dict = None):
+    return get_data_loader(
+        config_name="roboflow_detection_dataset_params",
+        dataset_cls=RoboflowDetectionDataset,
+        train=True,
+        dataset_params=dataset_params,
+        dataloader_params=dataloader_params,
+    )
+
+
+@register_dataloader(Dataloaders.ROBOFLOW_VAL_BASE)
+def roboflow_val_yolox(dataset_params: Dict = None, dataloader_params: Dict = None):
+    return get_data_loader(
+        config_name="roboflow_detection_dataset_params",
+        dataset_cls=RoboflowDetectionDataset,
+        train=False,
+        dataset_params=dataset_params,
+        dataloader_params=dataloader_params,
+    )
+
+
 @register_dataloader(Dataloaders.IMAGENET_TRAIN)
 def imagenet_train(dataset_params: Dict = None, dataloader_params: Dict = None, config_name="imagenet_dataset_params"):
     return get_data_loader(
         config_name=config_name,
         dataset_cls=ImageNetDataset,
         train=True,
         dataset_params=dataset_params,
```

## super_gradients/training/datasets/__init__.py

```diff
@@ -1,14 +1,19 @@
 from __future__ import absolute_import
 import cv2
 
 from super_gradients.training.datasets.data_augmentation import DataAugmentation
 from super_gradients.training.datasets.sg_dataset import ListDataset, DirectoryDataSet
 from super_gradients.training.datasets.classification_datasets import ImageNetDataset, Cifar10, Cifar100
-from super_gradients.training.datasets.detection_datasets import DetectionDataset, COCODetectionDataset, PascalVOCDetectionDataset
+from super_gradients.training.datasets.detection_datasets import (
+    DetectionDataset,
+    COCODetectionDataset,
+    PascalVOCDetectionDataset,
+    YoloDarknetFormatDetectionDataset,
+)
 from super_gradients.training.datasets.segmentation_datasets.segmentation_dataset import SegmentationDataSet
 from super_gradients.training.datasets.segmentation_datasets.pascal_voc_segmentation import (
     PascalVOC2012SegmentationDataSet,
     PascalAUG2012SegmentationDataSet,
     PascalVOCAndAUGUnifiedDataset,
 )
 from super_gradients.training.datasets.segmentation_datasets.cityscape_segmentation import CityscapesDataset
@@ -27,14 +32,15 @@
     "CityscapesDataset",
     "PascalVOC2012SegmentationDataSet",
     "PascalAUG2012SegmentationDataSet",
     "PascalVOCAndAUGUnifiedDataset",
     "CoCoSegmentationDataSet",
     "DetectionDataset",
     "COCODetectionDataset",
+    "YoloDarknetFormatDetectionDataset",
     "PascalVOCDetectionDataset",
     "ImageNetDataset",
     "Cifar10",
     "Cifar100",
     "SuperviselyPersonsDataset",
     "COCOKeypointsDataset",
 ]
```

## super_gradients/training/datasets/data_formats/__init__.py

```diff
@@ -1,5 +1,27 @@
 from .format_converter import ConcatenatedTensorFormatConverter
 from .output_adapters import DetectionOutputAdapter
 from .formats import ConcatenatedTensorFormat, BoundingBoxesTensorSliceItem, TensorSliceItem
+from .bbox_formats import (
+    CXCYWHCoordinateFormat,
+    NormalizedCXCYWHCoordinateFormat,
+    NormalizedXYWHCoordinateFormat,
+    NormalizedXYXYCoordinateFormat,
+    XYWHCoordinateFormat,
+    XYXYCoordinateFormat,
+    YXYXCoordinateFormat,
+)
 
-__all__ = ["ConcatenatedTensorFormatConverter", "DetectionOutputAdapter", "TensorSliceItem", "ConcatenatedTensorFormat", "BoundingBoxesTensorSliceItem"]
+__all__ = [
+    "BoundingBoxesTensorSliceItem",
+    "CXCYWHCoordinateFormat",
+    "ConcatenatedTensorFormat",
+    "ConcatenatedTensorFormatConverter",
+    "DetectionOutputAdapter",
+    "NormalizedCXCYWHCoordinateFormat",
+    "NormalizedXYWHCoordinateFormat",
+    "NormalizedXYXYCoordinateFormat",
+    "TensorSliceItem",
+    "XYWHCoordinateFormat",
+    "XYXYCoordinateFormat",
+    "YXYXCoordinateFormat",
+]
```

## super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py

```diff
@@ -110,15 +110,15 @@
     >>>         BoundingBoxesTensorSliceItem(name="bboxes", format=NormalizedXYWHCoordinateFormat()),
     >>>         TensorSliceItem(name="attributes", length=4),
     >>>         TensorSliceItem(name="label", length=1),
     >>>     )
     >>> )
     >>>
     >>> # Now we can construct output adapter and attach it to the model
-    >>> output_adapter = DetectionOutputAdapter(yolox,
+    >>> output_adapter = DetectionOutputAdapter(
     >>>     input_format=yolox.head.format,
     >>>     output_format=output_format,
     >>>     image_shape=(640, 640)
     >>> )
     >>>
     >>> yolox = nn.Sequential(yolox, output_adapter)
     >>>
@@ -129,22 +129,24 @@
 
         :param input_format: Format definition of the inputs
         :param output_format: Format definition of the outputs
         :param image_shape: Shape of the input image (rows, cols), used for converting bbox coordinates from/to normalized format.
                             If you're not using normalized coordinates you can set this to None
         """
         super().__init__()
-        self.rearrange_outputs, rearranged_format = self.get_rearrange_outputs_module(input_format, output_format)
 
         self.format_conversion: nn.Module = self.get_format_conversion_module(
-            location=rearranged_format.locations[rearranged_format.bboxes_format.name],
-            input_bbox_format=rearranged_format.bboxes_format.format,
+            location=input_format.locations[input_format.bboxes_format.name],
+            input_bbox_format=input_format.bboxes_format.format,
             output_bbox_format=output_format.bboxes_format.format,
             image_shape=image_shape,
         )
+
+        self.rearrange_outputs, rearranged_format = self.get_rearrange_outputs_module(input_format, output_format)
+
         self.input_format = input_format
         self.output_format = output_format
         self.input_length = input_format.num_channels
 
     def forward(self, predictions: Tensor) -> Tensor:
         """
         Convert output detections to the user-specified format
@@ -153,16 +155,16 @@
         """
         if predictions.size(-1) != self.input_length:
             raise RuntimeError(
                 f"Number of channels in last dimension of input tensor ({predictions.size(-1)}) must be "
                 f"equal to {self.input_length} as defined by input format."
             )
 
+        predictions = self.format_conversion(predictions.clone())
         predictions = self.rearrange_outputs(predictions)
-        predictions = self.format_conversion(predictions)
         return predictions
 
     @classmethod
     def get_rearrange_outputs_module(
         cls, input_format: ConcatenatedTensorFormat, output_format: ConcatenatedTensorFormat
     ) -> Tuple[RearrangeOutput, ConcatenatedTensorFormat]:
```

## super_gradients/training/datasets/detection_datasets/__init__.py

```diff
@@ -1,6 +1,7 @@
 from super_gradients.training.datasets.detection_datasets.coco_detection import COCODetectionDataset
 from super_gradients.training.datasets.detection_datasets.pascal_voc_detection import PascalVOCDetectionDataset
 from super_gradients.training.datasets.detection_datasets.detection_dataset import DetectionDataset
+from super_gradients.training.datasets.detection_datasets.roboflow import RoboflowDetectionDataset
+from super_gradients.training.datasets.detection_datasets.yolo_format_detection import YoloDarknetFormatDetectionDataset
 
-
-__all__ = ["COCODetectionDataset", "DetectionDataset", "PascalVOCDetectionDataset"]
+__all__ = ["COCODetectionDataset", "DetectionDataset", "PascalVOCDetectionDataset", "RoboflowDetectionDataset", "YoloDarknetFormatDetectionDataset"]
```

## super_gradients/training/datasets/detection_datasets/coco_detection.py

```diff
@@ -1,19 +1,19 @@
 import os
 
 from super_gradients.common.object_names import Datasets
 from super_gradients.common.registry.registry import register_dataset
 from super_gradients.common.abstractions.abstract_logger import get_logger
-from super_gradients.training.datasets.detection_datasets.coco_format_detection import COCOFormattedDetectionDataset
+from super_gradients.training.datasets.detection_datasets.coco_format_detection import COCOFormatDetectionDataset
 
 logger = get_logger(__name__)
 
 
 @register_dataset(Datasets.COCO_DETECTION_DATASET)
-class COCODetectionDataset(COCOFormattedDetectionDataset):
+class COCODetectionDataset(COCOFormatDetectionDataset):
     """Dataset for COCO object detection.
 
     To use this Dataset you need to:
 
         - Download coco dataset:
             annotations: http://images.cocodataset.org/annotations/annotations_trainval2017.zip
             train2017: http://images.cocodataset.org/zips/train2017.zip
```

## super_gradients/training/datasets/detection_datasets/coco_format_detection.py

```diff
@@ -1,52 +1,57 @@
 import copy
 import os
-from typing import List
 
 import cv2
 import numpy as np
 from pycocotools.coco import COCO
+from typing import List, Optional
 
 from contextlib import redirect_stdout
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.datasets.detection_datasets.detection_dataset import DetectionDataset
 from super_gradients.training.exceptions.dataset_exceptions import DatasetValidationException, ParameterMismatchException
 from super_gradients.training.datasets.data_formats.default_formats import XYXY_LABEL
 
 logger = get_logger(__name__)
 
 
-class COCOFormattedDetectionDataset(DetectionDataset):
+class COCOFormatDetectionDataset(DetectionDataset):
     """Base dataset to load ANY dataset that is with a similar structure to the COCO dataset.
     - Annotation file (.json). It has to respect the exact same format as COCO, for both the json schema and the bbox format (xywh).
     - One folder with all the images.
+
+    Output format: (x, y, x, y, class_id)
     """
 
     def __init__(
         self,
         data_dir: str,
         json_annotation_file: str,
         images_dir: str,
         tight_box_rotation: bool = False,
         with_crowd: bool = True,
+        class_ids_to_ignore: Optional[List[int]] = None,
         *args,
         **kwargs,
     ):
         """
         :param data_dir:                Where the data is stored.
         :param json_annotation_file:    Name of the coco json file. Path relative to data_dir.
         :param images_dir:              Name of the directory that includes all the images. Path relative to data_dir.
         :param tight_box_rotation:      bool, whether to use of segmentation maps convex hull as target_seg
                                             (check get_sample docs).
         :param with_crowd:              Add the crowd groundtruths to __getitem__
+        :param class_ids_to_ignore:     List of class ids to ignore in the dataset. By default, doesnt ignore any class.
         """
         self.images_dir = images_dir
         self.json_annotation_file = json_annotation_file
         self.tight_box_rotation = tight_box_rotation
         self.with_crowd = with_crowd
+        self.class_ids_to_ignore = class_ids_to_ignore or []
 
         target_fields = ["target", "crowd_target"] if self.with_crowd else ["target"]
         kwargs["target_fields"] = target_fields
         kwargs["output_fields"] = ["image", *target_fields]
         kwargs["original_target_format"] = XYXY_LABEL
         super().__init__(data_dir=data_dir, *args, **kwargs)
 
@@ -65,15 +70,15 @@
     def _setup_data_source(self) -> int:
         """Initialize img_and_target_path_list and warn if label file is missing
 
         :return: List of tuples made of (img_path,target_path)
         """
 
         self.coco = self._init_coco()
-        self.class_ids = sorted(self.coco.getCatIds())
+        self.class_ids = sorted(cls_id for cls_id in self.coco.getCatIds() if cls_id not in self.class_ids_to_ignore)
         self.original_classes = list([category["name"] for category in self.coco.loadCats(self.class_ids)])
         self.classes = copy.deepcopy(self.original_classes)
         self.sample_id_to_coco_id = self.coco.getImgIds()
         return len(self.sample_id_to_coco_id)
 
     @property
     def _all_classes(self) -> List[str]:
@@ -148,14 +153,15 @@
 
         crowd_target = np.zeros((len(crowd_annotations), 5))
         for ix, annotation in enumerate(crowd_annotations):
             cls = self.class_ids.index(annotation["category_id"])
             crowd_target[ix, 0:4] = annotation["clean_bbox"]
             crowd_target[ix, 4] = cls
 
+        # Currently, the base class includes a feature to resize the image, so we need to resize the target as well when self.input_dim is set.
         initial_img_shape = (height, width)
         if self.input_dim is not None:
             r = min(self.input_dim[0] / height, self.input_dim[1] / width)
             target[:, :4] *= r
             crowd_target[:, :4] *= r
             target_segmentation *= r
             resized_img_shape = (int(height * r), int(width * r))
```

## super_gradients/training/datasets/detection_datasets/detection_dataset.py

```diff
@@ -9,15 +9,15 @@
 from copy import deepcopy
 import hashlib
 
 import numpy as np
 from tqdm import tqdm
 from torch.utils.data import Dataset
 
-from super_gradients.common.object_names import Datasets
+from super_gradients.common.object_names import Datasets, Processings
 from super_gradients.common.registry.registry import register_dataset
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.training.utils.detection_utils import get_cls_posx_in_target
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.transforms.transforms import DetectionTransform, DetectionTargetsFormatTransform, DetectionTargetsFormat
 from super_gradients.training.exceptions.dataset_exceptions import EmptyDatasetException, DatasetValidationException
 from super_gradients.common.factories.list_factory import ListFactory
@@ -68,19 +68,19 @@
                                 > Therefore, we also have len(self) = 100
     """
 
     @resolve_param("transforms", ListFactory(TransformsFactory()))
     def __init__(
         self,
         data_dir: str,
-        input_dim: Optional[Tuple[int, int]],
         original_target_format: Union[ConcatenatedTensorFormat, DetectionTargetsFormat],
         max_num_samples: int = None,
         cache: bool = False,
         cache_dir: str = None,
+        input_dim: Optional[Tuple[int, int]] = None,
         transforms: List[DetectionTransform] = [],
         all_classes_list: Optional[List[str]] = [],
         class_inclusion_list: Optional[List[str]] = None,
         ignore_empty_annotations: bool = True,
         target_fields: List[str] = None,
         output_fields: List[str] = None,
         verbose: bool = True,
@@ -254,14 +254,16 @@
         logger.warning(
             "\n********************************************************************************\n"
             "You are using cached images in RAM to accelerate training.\n"
             "This requires large system RAM.\n"
             "********************************************************************************"
         )
 
+        if self.input_dim is None:
+            raise RuntimeError("caching is not possible without input_dim is not set")
         max_h, max_w = self.input_dim[0], self.input_dim[1]
 
         # The cache should be the same as long as the images and their sizes are the same
         hash = hashlib.sha256()
         for annotation in self.annotations:
             values_to_hash = [annotation["resized_img_shape"][0], annotation["resized_img_shape"][1], Path(annotation["img_path"]).name]
             for value in values_to_hash:
@@ -467,7 +469,26 @@
             fig.tight_layout()
             plt.show()
             plt.close()
 
             plot_counter += 1
             if plot_counter == n_plots:
                 return
+
+    def get_dataset_preprocessing_params(self):
+        """
+        Return any hardcoded preprocessing + adaptation for PIL.Image image reading (RGB).
+         image_processor as returned as as list of dicts to be resolved by processing factory.
+        :return:
+        """
+        pipeline = [Processings.ReverseImageChannels]
+        if self.input_dim is not None:
+            pipeline += [{Processings.DetectionLongestMaxSizeRescale: {"output_shape": self.input_dim}}]
+        for t in self.transforms:
+            pipeline += t.get_equivalent_preprocessing()
+        params = dict(
+            class_names=self.classes,
+            image_processor={Processings.ComposeProcessing: {"processings": pipeline}},
+            iou=0.65,
+            conf=0.5,
+        )
+        return params
```

## super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py

```diff
@@ -1,13 +1,13 @@
 import abc
 from typing import Tuple, List, Mapping, Any, Dict
 
 import numpy as np
 import torch
-from torch.utils.data import default_collate, Dataset
+from torch.utils.data.dataloader import default_collate, Dataset
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.registry.registry import register_collate_function
 from super_gradients.training.datasets.pose_estimation_datasets.target_generators import KeypointsTargetsGenerator
 from super_gradients.training.transforms.keypoint_transforms import KeypointsCompose, KeypointTransform
 
 logger = get_logger(__name__)
```

## super_gradients/training/losses/dice_ce_edge_loss.py

```diff
@@ -22,23 +22,31 @@
         dice_ce_weights: Union[tuple, list] = (1, 1),
         ignore_index: int = -100,
         edge_kernel: int = 3,
         ce_edge_weights: Union[tuple, list] = (0.5, 0.5),
     ):
         """
         Total loss is computed as follows:
-                Loss-cls-edge = λ1 * CE + λ2 * M * CE , where [λ1, λ2] are ce_edge_weights.
-            For each Main feature maps and auxiliary heads the loss is calculated as:
-                Loss-main-aux = λ3 * Loss-cls-edge + λ4 * Loss-Dice, where [λ3, λ4] are dice_ce_weights.
-            For Feature maps defined as detail maps that predicts only the edge mask, the loss is computed as follow:
-                Loss-detail = BinaryCE + BinaryDice
-            Finally the total loss is computed as follows for the whole feature maps:
-                Loss = Σw[i] * Loss-main-aux[i] + Σw[j] * Loss-detail[j], where `w` is defined as the `weights` argument
-                    `i` in [0, 1 + num_aux_heads], 1 is for the main feature map.
-                    `j` in [1 + num_aux_heads, 1 + num_aux_heads + num_detail_heads].
+
+            Loss-cls-edge = λ1 * CE + λ2 * M * CE , where [λ1, λ2] are ce_edge_weights.
+
+        For each Main feature maps and auxiliary heads the loss is calculated as:
+
+            Loss-main-aux = λ3 * Loss-cls-edge + λ4 * Loss-Dice, where [λ3, λ4] are dice_ce_weights.
+
+        For Feature maps defined as detail maps that predicts only the edge mask, the loss is computed as follow:
+
+            Loss-detail = BinaryCE + BinaryDice
+
+        Finally the total loss is computed as follows for the whole feature maps:
+
+            Loss = Σw[i] * Loss-main-aux[i] + Σw[j] * Loss-detail[j], where `w` is defined as the `weights` argument
+                `i` in [0, 1 + num_aux_heads], 1 is for the main feature map.
+                `j` in [1 + num_aux_heads, 1 + num_aux_heads + num_detail_heads].
+
 
         :param num_aux_heads: num of auxiliary heads.
         :param num_detail_heads: num of detail heads.
         :param weights: Loss lambda weights.
         :param dice_ce_weights: weights lambdas between (Dice, CE) losses.
         :param edge_kernel: kernel size of dilation erosion convolutions for creating the edge feature map.
         :param ce_edge_weights: weights lambdas between regular CE and edge attention CE.
```

## super_gradients/training/models/__init__.py

```diff
@@ -92,14 +92,15 @@
     STDCClassification,
     STDC1Classification,
     STDCClassificationBase,
     STDC2Classification,
     STDCSegmentationBase,
     CustomSTDCSegmentation,
 )
+from super_gradients.training.models.segmentation_models.segformer import SegFormerB0, SegFormerB1, SegFormerB2, SegFormerB3, SegFormerB4, SegFormerB5
 
 # Pose estimation
 from super_gradients.training.models.pose_estimation_models.pose_ppyolo import PosePPYoloL
 from super_gradients.training.models.pose_estimation_models.pose_ddrnet39 import PoseDDRNet39
 from super_gradients.training.models.pose_estimation_models.dekr_hrnet import DEKRPoseEstimationModel, DEKRW32
 
 # KD
@@ -254,8 +255,14 @@
     "get_model_name",
     "get_arch_params",
     "convert_to_onnx",
     "convert_from_config",
     "ARCHITECTURES",
     "Models",
     "user_models",
+    "SegFormerB0",
+    "SegFormerB1",
+    "SegFormerB2",
+    "SegFormerB3",
+    "SegFormerB4",
+    "SegFormerB5",
 ]
```

## super_gradients/training/models/model_factory.py

```diff
@@ -2,28 +2,30 @@
 from typing import Tuple, Type, Optional, Union
 
 import hydra
 import torch
 
 from super_gradients.common.data_types.enum.strict_load import StrictLoad
 from super_gradients.common.plugins.deci_client import DeciClient, client_enabled
+from super_gradients.module_interfaces import HasPredict
 from super_gradients.training import utils as core_utils
 from super_gradients.common.exceptions.factory_exceptions import UnknownTypeException
 from super_gradients.training.models import SgModule
 from super_gradients.common.registry.registry import ARCHITECTURES
 from super_gradients.training.pretrained_models import PRETRAINED_NUM_CLASSES
 from super_gradients.training.utils import HpmStruct, get_param
 from super_gradients.training.utils.checkpoint_utils import (
     load_checkpoint_to_model,
     load_pretrained_weights,
     read_ckpt_state_dict,
     load_pretrained_weights_local,
 )
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.utils.sg_trainer_utils import get_callable_param_names
+from super_gradients.training.processing.processing import get_pretrained_processing_params
 
 logger = get_logger(__name__)
 
 
 def get_architecture(model_name: str, arch_params: HpmStruct, download_required_code: bool = True) -> Tuple[Type[torch.nn.Module], HpmStruct, str, bool]:
     """
     Get the corresponding architecture class.
@@ -131,14 +133,19 @@
             else:
                 load_pretrained_weights(net, model_name, pretrained_weights)
 
             if num_classes_new_head != arch_params.num_classes:
                 net.replace_head(new_num_classes=num_classes_new_head)
                 arch_params.num_classes = num_classes_new_head
 
+            # STILL NEED TO GET PREPROCESSING PARAMS IN CASE CHECKPOINT HAS NO RECIPE
+            if isinstance(net, HasPredict):
+                processing_params = get_pretrained_processing_params(model_name, pretrained_weights)
+                net.set_dataset_processing_params(**processing_params)
+
     _add_model_name_attribute(net, model_name)
 
     return net
 
 
 def _add_model_name_attribute(model: torch.nn.Module, model_name: str) -> None:
     """Add an attribute to a model.
@@ -191,20 +198,23 @@
     else:
         net = instantiate_model(model_name, arch_params, num_classes, pretrained_weights, download_required_code)
 
     if load_backbone and not checkpoint_path:
         raise ValueError("Please set checkpoint_path when load_backbone=True")
 
     if checkpoint_path:
-        load_ema_as_net = "ema_net" in read_ckpt_state_dict(ckpt_path=checkpoint_path).keys()
+        ckpt_entries = read_ckpt_state_dict(ckpt_path=checkpoint_path).keys()
+        load_processing = "processing_params" in ckpt_entries
+        load_ema_as_net = "ema_net" in ckpt_entries
         _ = load_checkpoint_to_model(
             ckpt_local_path=checkpoint_path,
             load_backbone=load_backbone,
             net=net,
             strict=strict_load.value if hasattr(strict_load, "value") else strict_load,
             load_weights_only=True,
             load_ema_as_net=load_ema_as_net,
+            load_processing_params=load_processing,
         )
     if checkpoint_num_classes != num_classes:
         net.replace_head(new_num_classes=num_classes)
 
     return net
```

## super_gradients/training/models/classification_models/dpn.py

```diff
@@ -1,15 +1,18 @@
 """
 Dual Path Networks in PyTorch.
 
 Credits: https://github.com/kuangliu/pytorch-cifar/blob/master/models/dpn.py
 """
+from typing import Tuple
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+
 from super_gradients.training.models.sg_module import SgModule
 
 
 class Bottleneck(nn.Module):
     def __init__(self, last_planes, in_planes, out_planes, dense_depth, stride, first_layer):
         super(Bottleneck, self).__init__()
         self.out_planes = out_planes
@@ -36,18 +39,22 @@
         d = self.out_planes
         out = torch.cat([x[:, :d, :, :] + out[:, :d, :, :], x[:, d:, :, :], out[:, d:, :, :]], 1)
         out = F.relu(out)
         return out
 
 
 class DPN(SgModule):
-    def __init__(self, cfg):
+    def __init__(
+        self,
+        in_planes: Tuple[int, int, int, int],
+        out_planes: Tuple[int, int, int, int],
+        num_blocks: Tuple[int, int, int, int],
+        dense_depth: Tuple[int, int, int, int],
+    ):
         super(DPN, self).__init__()
-        in_planes, out_planes = cfg["in_planes"], cfg["out_planes"]
-        num_blocks, dense_depth = cfg["num_blocks"], cfg["dense_depth"]
 
         self.conv1 = nn.Conv2d(3, 64, kernel_size=3, stride=1, padding=1, bias=False)
         self.bn1 = nn.BatchNorm2d(64)
         self.last_planes = 64
         self.layer1 = self._make_layer(in_planes[0], out_planes[0], num_blocks[0], dense_depth[0], stride=1)
         self.layer2 = self._make_layer(in_planes[1], out_planes[1], num_blocks[1], dense_depth[1], stride=2)
         self.layer3 = self._make_layer(in_planes[2], out_planes[2], num_blocks[2], dense_depth[2], stride=2)
@@ -71,21 +78,19 @@
         out = F.avg_pool2d(out, 4)
         out = out.view(out.size(0), -1)
         out = self.linear(out)
         return out
 
 
 def DPN26():
-    cfg = {"in_planes": (96, 192, 384, 768), "out_planes": (256, 512, 1024, 2048), "num_blocks": (2, 2, 2, 2), "dense_depth": (16, 32, 24, 128)}
-    return DPN(cfg)
+    return DPN(in_planes=(96, 192, 384, 768), out_planes=(256, 512, 1024, 2048), num_blocks=(2, 2, 2, 2), dense_depth=(16, 32, 24, 128))
 
 
 def DPN92():
-    cfg = {"in_planes": (96, 192, 384, 768), "out_planes": (256, 512, 1024, 2048), "num_blocks": (3, 4, 20, 3), "dense_depth": (16, 32, 24, 128)}
-    return DPN(cfg)
+    return DPN(in_planes=(96, 192, 384, 768), out_planes=(256, 512, 1024, 2048), num_blocks=(3, 4, 20, 3), dense_depth=(16, 32, 24, 128))
 
 
 def test():
     net = DPN92()
     x = torch.randn(1, 3, 32, 32)
     y = net(x)
     print(y)
```

## super_gradients/training/models/classification_models/efficientnet.py

```diff
@@ -396,79 +396,98 @@
 class EfficientNet(SgModule):
     """
     EfficientNet model.
 
     References:
         [1] https://arxiv.org/abs/1905.11946 (EfficientNet)
 
-    :param blocks_args: A list of BlockArgs to construct blocks. (list[namedtuple])
-    :param arch_params: A set of global params shared between blocks.
+
+    :param width_coefficient:   model's width coefficient. Used as the multiplier.
+    :param depth_coefficient:   model's depth coefficient. Used as the multiplier.
+    :param image_size:          Size of input image.
+    :param dropout_rate:        Dropout probability in final layer
+    :param num_classes:         Number of classes.
+    :param batch_norm_momentum: Value used for the running_mean and running_var computation
+    :param batch_norm_epsilon:  Value added to the denominator for numerical stability
+    :param drop_connect_rate:   Connection dropout probability
+    :param depth_divisor:       Model's depth divisor. Used as the divisor.
+    :param min_depth:           Model's minimal depth, if given.
+    :param backbone_mode:       If true, dropping the final linear layer
+    :param blocks_args:         List of BlockArgs to construct blocks. (list[namedtuple])
     """
 
-    def __init__(self, blocks_args: Optional[List] = None, arch_params: Optional[HpmStruct] = None):
+    def __init__(
+        self,
+        width_coefficient: float,
+        depth_coefficient: float,
+        image_size: int,
+        dropout_rate: float,
+        num_classes: int,
+        batch_norm_momentum: Optional[float] = 0.99,
+        batch_norm_epsilon: Optional[float] = 1e-3,
+        drop_connect_rate: Optional[float] = 0.2,
+        depth_divisor: Optional[int] = 8,
+        min_depth: Optional[int] = None,
+        backbone_mode: Optional[bool] = False,
+        blocks_args: Optional[list] = None,
+    ):
         super().__init__()
         assert isinstance(blocks_args, list), "blocks_args should be a list"
         assert len(blocks_args) > 0, "block args must be greater than 0"
-        self._arch_params = arch_params
+
         self._blocks_args = blocks_args
-        self.backbone_mode = arch_params.backbone_mode
+        self.backbone_mode = backbone_mode
+        self.drop_connect_rate = drop_connect_rate
 
         # Batch norm parameters
-        bn_mom = 1 - self._arch_params.batch_norm_momentum
-        bn_eps = self._arch_params.batch_norm_epsilon
+        bn_mom = 1 - batch_norm_momentum
+        bn_eps = batch_norm_epsilon
 
         # Get stem static or dynamic convolution depending on image size
-        image_size = arch_params.image_size
         Conv2d = get_same_padding_conv2d(image_size=image_size)
 
         # Stem
         in_channels = 3  # rgb
-        out_channels = round_filters(
-            32, self._arch_params.width_coefficient, self._arch_params.depth_divisor, self._arch_params.min_depth
-        )  # number of output channels
+        out_channels = round_filters(32, width_coefficient, depth_divisor, min_depth)  # number of output channels
         self._conv_stem = Conv2d(in_channels, out_channels, kernel_size=3, stride=2, bias=False)
         self._bn0 = nn.BatchNorm2d(num_features=out_channels, momentum=bn_mom, eps=bn_eps)
         image_size = calculate_output_image_size(image_size, 2)
 
         # Build blocks
         self._blocks = nn.ModuleList([])
         for block_args in self._blocks_args:
 
             # Update block input and output filters based on depth multiplier.
             block_args = block_args._replace(
-                input_filters=round_filters(
-                    block_args.input_filters, self._arch_params.width_coefficient, self._arch_params.depth_divisor, self._arch_params.min_depth
-                ),
-                output_filters=round_filters(
-                    block_args.output_filters, self._arch_params.width_coefficient, self._arch_params.depth_divisor, self._arch_params.min_depth
-                ),
-                num_repeat=round_repeats(block_args.num_repeat, self._arch_params.depth_coefficient),
+                input_filters=round_filters(block_args.input_filters, width_coefficient, depth_divisor, min_depth),
+                output_filters=round_filters(block_args.output_filters, width_coefficient, depth_divisor, min_depth),
+                num_repeat=round_repeats(block_args.num_repeat, depth_coefficient),
             )
 
             # The first block needs to take care of stride and filter size increase.
-            self._blocks.append(MBConvBlock(block_args, self._arch_params.batch_norm_momentum, self._arch_params.batch_norm_epsilon, image_size=image_size))
+            self._blocks.append(MBConvBlock(block_args, batch_norm_momentum, batch_norm_epsilon, image_size=image_size))
             image_size = calculate_output_image_size(image_size, block_args.stride)
             if block_args.num_repeat > 1:  # modify block_args to keep same output size
                 block_args = block_args._replace(input_filters=block_args.output_filters, stride=1)
             for _ in range(block_args.num_repeat - 1):
-                self._blocks.append(MBConvBlock(block_args, self._arch_params.batch_norm_momentum, self._arch_params.batch_norm_epsilon, image_size=image_size))
+                self._blocks.append(MBConvBlock(block_args, batch_norm_momentum, batch_norm_epsilon, image_size=image_size))
                 # image_size = calculate_output_image_size(image_size, block_args.stride)  # stride = 1
 
         # Head
         in_channels = block_args.output_filters  # output of final block
-        out_channels = round_filters(1280, self._arch_params.width_coefficient, self._arch_params.depth_divisor, self._arch_params.min_depth)
+        out_channels = round_filters(1280, width_coefficient, depth_divisor, min_depth)
         Conv2d = get_same_padding_conv2d(image_size=image_size)
         self._conv_head = Conv2d(in_channels, out_channels, kernel_size=1, bias=False)
         self._bn1 = nn.BatchNorm2d(num_features=out_channels, momentum=bn_mom, eps=bn_eps)
 
         # Final linear layer
         if not self.backbone_mode:
             self._avg_pooling = nn.AdaptiveAvgPool2d(1)
-            self._dropout = nn.Dropout(self._arch_params.dropout_rate)
-            self._fc = nn.Linear(out_channels, self._arch_params.num_classes)
+            self._dropout = nn.Dropout(dropout_rate)
+            self._fc = nn.Linear(out_channels, num_classes)
         self._swish = nn.functional.silu
 
     def extract_features(self, inputs: torch.Tensor) -> torch.Tensor:
         """
         Use convolution layer to extract feature.
 
         :param inputs: Input tensor.
@@ -476,15 +495,15 @@
         """
 
         # Stem
         x = self._swish(self._bn0(self._conv_stem(inputs)))
 
         # Blocks
         for idx, block in enumerate(self._blocks):
-            drop_connect_rate = self._arch_params.drop_connect_rate
+            drop_connect_rate = self.drop_connect_rate
             if drop_connect_rate:
                 drop_connect_rate *= float(idx) / len(self._blocks)  # scale drop connect_rate
             x = block(x, drop_connect_rate=drop_connect_rate)
 
         # Head
         x = self._swish(self._bn1(self._conv_head(x)))
 
@@ -508,23 +527,23 @@
             x = self._avg_pooling(x)
             x = x.view(bs, -1)
             x = self._dropout(x)
             x = self._fc(x)
 
         return x
 
-    def replace_head(self, new_num_classes=None, new_head=None):
+    def replace_head(self, new_num_classes: Optional[int] = None, new_head: Optional[nn.Module] = None):
         if new_num_classes is None and new_head is None:
             raise ValueError("At least one of new_num_classes, new_head must be given to replace output layer.")
         if new_head is not None:
             self._fc = new_head
         else:
             self._fc = nn.Linear(self._fc.in_features, new_num_classes)
 
-    def load_state_dict(self, state_dict, strict=True):
+    def load_state_dict(self, state_dict: dict, strict: bool = True):
         """
         load_state_dict - Overloads the base method and calls it to load a modified dict for usage as a backbone
         :param state_dict:  The state_dict to load
         :param strict:      strict loading (see super() docs)
         """
         pretrained_model_weights_dict = state_dict.copy()
 
@@ -584,86 +603,229 @@
     # Update arch_params
     arch_params_new.override(**arch_params.to_dict())
     return blocks_args, arch_params_new
 
 
 @register_model(Models.EFFICIENTNET_B0)
 class EfficientNetB0(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.0, depth=1.0, res=224, dropout=0.2, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B1)
 class EfficientNetB1(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.0, depth=1.1, res=240, dropout=0.2, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B2)
 class EfficientNetB2(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.1, depth=1.2, res=260, dropout=0.3, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B3)
 class EfficientNetB3(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.2, depth=1.4, res=300, dropout=0.3, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B4)
 class EfficientNetB4(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.4, depth=1.8, res=380, dropout=0.4, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B5)
 class EfficientNetB5(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.6, depth=2.2, res=456, dropout=0.4, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B6)
 class EfficientNetB6(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=1.8, depth=2.6, res=528, dropout=0.5, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B7)
 class EfficientNetB7(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=2.0, depth=3.1, res=600, dropout=0.5, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_B8)
 class EfficientNetB8(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=2.2, depth=3.6, res=672, dropout=0.5, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.EFFICIENTNET_L2)
 class EfficientNetL2(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(width=4.3, depth=5.3, res=800, dropout=0.5, arch_params=arch_params)
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
 
 
 @register_model(Models.CUSTOMIZEDEFFICIENTNET)
 class CustomizedEfficientnet(EfficientNet):
-    def __init__(self, arch_params):
+    def __init__(self, arch_params: HpmStruct):
         blocks_args, arch_params = get_efficientnet_params(
             width=arch_params.width_coefficient,
             depth=arch_params.depth_coefficient,
             res=arch_params.res,
             dropout=arch_params.dropout_rate,
             arch_params=arch_params,
         )
-        super().__init__(blocks_args=blocks_args, arch_params=arch_params)
+        super().__init__(
+            blocks_args=blocks_args,
+            num_classes=arch_params.num_classes,
+            backbone_mode=arch_params.backbone_mode,
+            batch_norm_momentum=arch_params.batch_norm_momentum,
+            batch_norm_epsilon=arch_params.batch_norm_epsilon,
+            image_size=arch_params.image_size,
+            width_coefficient=arch_params.width_coefficient,
+            depth_divisor=arch_params.depth_divisor,
+            min_depth=arch_params.min_depth,
+            depth_coefficient=arch_params.depth_coefficient,
+            dropout_rate=arch_params.dropout_rate,
+            drop_connect_rate=arch_params.drop_connect_rate,
+        )
```

## super_gradients/training/models/detection_models/customizable_detector.py

```diff
@@ -1,83 +1,177 @@
 """
 A base for a detection network built according to the following scheme:
  * constructed from nested arch_params;
  * inside arch_params each nested level (module) has an explicit type and its required parameters
  * each module accepts in_channels and other parameters
  * each module defines out_channels property on construction
 """
-
-
-from typing import Union
+from typing import Union, Optional, List
 
 from torch import nn
 from omegaconf import DictConfig
 
-from super_gradients.training.utils.utils import HpmStruct, get_param
+from super_gradients.common.decorators.factory_decorator import resolve_param
+from super_gradients.common.factories.processing_factory import ProcessingFactory
+from super_gradients.training.utils.utils import HpmStruct
 from super_gradients.training.models.sg_module import SgModule
 import super_gradients.common.factories.detection_modules_factory as det_factory
+from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
+from super_gradients.training.pipelines.pipelines import DetectionPipeline
+from super_gradients.training.processing.processing import Processing
+from super_gradients.training.utils.detection_utils import DetectionPostPredictionCallback
+from super_gradients.training.utils.media.image import ImageSource
 
 
 class CustomizableDetector(SgModule):
     """
     A customizable detector with backbone -> neck -> heads
     Each submodule with its parameters must be defined explicitly.
     Modules should follow the interface of BaseDetectionModule
     """
 
-    def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
+    def __init__(
+        self,
+        backbone: Union[str, dict, HpmStruct, DictConfig],
+        heads: Union[str, dict, HpmStruct, DictConfig],
+        neck: Optional[Union[str, dict, HpmStruct, DictConfig]] = None,
+        num_classes: int = None,
+        bn_eps: Optional[float] = None,
+        bn_momentum: Optional[float] = None,
+        inplace_act: Optional[bool] = True,
+        in_channels: int = 3,
+    ):
         """
-        :param type_mapping: can be passed to resolve string type names in arch_params to actual types
+        :param backbone:    Backbone configuration.
+        :param heads:       Head configuration.
+        :param neck:        Neck configuration.
+        :param num_classes: num classes to predict.
+        :param bn_eps:      Epsilon for batch norm.
+        :param bn_momentum: Momentum for batch norm.
+        :param inplace_act: If True, do the operations operation in-place when possible.
+        :param in_channels: number of input channels
         """
         super().__init__()
 
+        self.heads_params = heads
+        self.bn_eps = bn_eps
+        self.bn_momentum = bn_momentum
+        self.inplace_act = inplace_act
         factory = det_factory.DetectionModulesFactory()
 
         # move num_classes into heads params
-        if get_param(arch_params, "num_classes"):
-            arch_params.heads = factory.insert_module_param(arch_params.heads, "num_classes", arch_params.num_classes)
+        if num_classes is not None:
+            self.heads_params = factory.insert_module_param(self.heads_params, "num_classes", num_classes)
 
-        self.arch_params = arch_params
-        self.backbone = factory.get(factory.insert_module_param(arch_params.backbone, "in_channels", in_channels))
-        if hasattr(arch_params, "neck"):
-            self.neck = factory.get(factory.insert_module_param(arch_params.neck, "in_channels", self.backbone.out_channels))
-            self.heads = factory.get(factory.insert_module_param(arch_params.heads, "in_channels", self.neck.out_channels))
+        self.backbone = factory.get(factory.insert_module_param(backbone, "in_channels", in_channels))
+        if neck is not None:
+            self.neck = factory.get(factory.insert_module_param(neck, "in_channels", self.backbone.out_channels))
+            self.heads = factory.get(factory.insert_module_param(heads, "in_channels", self.neck.out_channels))
         else:
             self.neck = nn.Identity()
-            self.heads = factory.get(factory.insert_module_param(arch_params.heads, "in_channels", self.backbone.out_channels))
+            self.heads = factory.get(factory.insert_module_param(heads, "in_channels", self.backbone.out_channels))
+
+        self._initialize_weights(bn_eps, bn_momentum, inplace_act)
 
-        self._initialize_weights(arch_params)
+        # Processing params
+        self._class_names: Optional[List[str]] = None
+        self._image_processor: Optional[Processing] = None
+        self._default_nms_iou: Optional[float] = None
+        self._default_nms_conf: Optional[float] = None
 
     def forward(self, x):
         x = self.backbone(x)
         x = self.neck(x)
         return self.heads(x)
 
-    def _initialize_weights(self, arch_params: Union[HpmStruct, DictConfig]):
-
-        bn_eps = get_param(arch_params, "bn_eps", None)
-        bn_momentum = get_param(arch_params, "bn_momentum", None)
-        inplace_act = get_param(arch_params, "inplace_act", True)
-
+    def _initialize_weights(self, bn_eps: Optional[float] = None, bn_momentum: Optional[float] = None, inplace_act: Optional[bool] = True):
         for m in self.modules():
             t = type(m)
             if t is nn.BatchNorm2d:
                 m.eps = bn_eps if bn_eps else m.eps
                 m.momentum = bn_momentum if bn_momentum else m.momentum
             elif inplace_act and t in [nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, nn.Mish]:
                 m.inplace = True
 
-    def prep_model_for_conversion(self, input_size: Union[tuple, list] = None, **kwargs):
+    def prep_model_for_conversion(self, input_size: Optional[Union[tuple, list]] = None, **kwargs):
         for module in self.modules():
             if module != self and hasattr(module, "prep_model_for_conversion"):
                 module.prep_model_for_conversion(input_size, **kwargs)
 
-    def replace_head(self, new_num_classes: int = None, new_head: nn.Module = None):
+    def replace_head(self, new_num_classes: Optional[int] = None, new_head: Optional[nn.Module] = None):
         if new_num_classes is None and new_head is None:
             raise ValueError("At least one of new_num_classes, new_head must be given to replace output layer.")
         if new_head is not None:
             self.heads = new_head
         else:
             factory = det_factory.DetectionModulesFactory()
-            self.arch_params.heads = factory.insert_module_param(self.arch_params.heads, "num_classes", new_num_classes)
-            self.heads = factory.get(factory.insert_module_param(self.arch_params.heads, "in_channels", self.neck.out_channels))
-            self._initialize_weights(self.arch_params)
+            self.heads_params = factory.insert_module_param(self.heads_params, "num_classes", new_num_classes)
+            self.heads = factory.get(factory.insert_module_param(self.heads_params, "in_channels", self.neck.out_channels))
+            self._initialize_weights(self.bn_eps, self.bn_momentum, self.inplace_act)
+
+    @staticmethod
+    def get_post_prediction_callback(conf: float, iou: float) -> DetectionPostPredictionCallback:
+        raise NotImplementedError
+
+    @resolve_param("image_processor", ProcessingFactory())
+    def set_dataset_processing_params(
+        self,
+        class_names: Optional[List[str]] = None,
+        image_processor: Optional[Processing] = None,
+        iou: Optional[float] = None,
+        conf: Optional[float] = None,
+    ) -> None:
+        """Set the processing parameters for the dataset.
+
+        :param class_names:     (Optional) Names of the dataset the model was trained on.
+        :param image_processor: (Optional) Image processing objects to reproduce the dataset preprocessing used for training.
+        :param iou:             (Optional) IoU threshold for the nms algorithm
+        :param conf:            (Optional) Below the confidence threshold, prediction are discarded
+        """
+        self._class_names = class_names or self._class_names
+        self._image_processor = image_processor or self._image_processor
+        self._default_nms_iou = iou or self._default_nms_iou
+        self._default_nms_conf = conf or self._default_nms_conf
+
+    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None) -> DetectionPipeline:
+        """Instantiate the prediction pipeline of this model.
+
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        if None in (self._class_names, self._image_processor, self._default_nms_iou, self._default_nms_conf):
+            raise RuntimeError(
+                "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
+            )
+
+        iou = iou or self._default_nms_iou
+        conf = conf or self._default_nms_conf
+
+        pipeline = DetectionPipeline(
+            model=self,
+            image_processor=self._image_processor,
+            post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
+            class_names=self._class_names,
+        )
+        return pipeline
+
+    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None) -> ImagesDetectionPrediction:
+        """Predict an image or a list of images.
+
+        :param images:  Images to predict.
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        return pipeline(images)  # type: ignore
+
+    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None):
+        """Predict using webcam.
+
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline.predict_webcam()
```

## super_gradients/training/models/detection_models/ssd.py

```diff
@@ -2,29 +2,47 @@
 from typing import Union
 
 from omegaconf import DictConfig
 
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.training.models.arch_params_factory import get_arch_params
-from super_gradients.training.utils.utils import HpmStruct
+from super_gradients.training.utils.utils import HpmStruct, get_param
 from super_gradients.training.models.detection_models.customizable_detector import CustomizableDetector
 
 
 DEFAULT_SSD_MOBILENET_V1_ARCH_PARAMS = get_arch_params("ssd_mobilenetv1_arch_params")
 DEFAULT_SSD_LITE_MOBILENET_V2_ARCH_PARAMS = get_arch_params("ssd_lite_mobilenetv2_arch_params")
 
 
 @register_model(Models.SSD_MOBILENET_V1)
 class SSDMobileNetV1(CustomizableDetector):
     def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
         merged_arch_params = HpmStruct(**copy.deepcopy(DEFAULT_SSD_MOBILENET_V1_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
-        super().__init__(merged_arch_params, in_channels=in_channels)
+        super().__init__(
+            backbone=merged_arch_params.backbone,
+            neck=merged_arch_params.neck,
+            heads=merged_arch_params.heads,
+            num_classes=get_param(merged_arch_params, "num_classes", None),
+            bn_eps=get_param(merged_arch_params, "bn_eps", None),
+            bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
+            inplace_act=get_param(merged_arch_params, "inplace_act", True),
+            in_channels=in_channels,
+        )
 
 
 @register_model(Models.SSD_LITE_MOBILENET_V2)
 class SSDLiteMobileNetV2(CustomizableDetector):
     def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
         merged_arch_params = HpmStruct(**copy.deepcopy(DEFAULT_SSD_LITE_MOBILENET_V2_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
-        super().__init__(merged_arch_params, in_channels=in_channels)
+        super().__init__(
+            backbone=merged_arch_params.backbone,
+            neck=merged_arch_params.neck,
+            heads=merged_arch_params.heads,
+            num_classes=get_param(merged_arch_params, "num_classes", None),
+            bn_eps=get_param(merged_arch_params, "bn_eps", None),
+            bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
+            inplace_act=get_param(merged_arch_params, "inplace_act", True),
+            in_channels=in_channels,
+        )
```

## super_gradients/training/models/detection_models/yolo_base.py

```diff
@@ -1,20 +1,26 @@
 import math
-from typing import Union, Type, List, Tuple
+from typing import Union, Type, List, Tuple, Optional
 
 import torch
 import torch.nn as nn
 
+from super_gradients.common.decorators.factory_decorator import resolve_param
+from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.modules import CrossModelSkipConnection
 from super_gradients.training.models.classification_models.regnet import AnyNetX, Stage
 from super_gradients.training.models.detection_models.csp_darknet53 import Conv, GroupedConvBlock, CSPDarknet53, get_yolo_type_params, SPP
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.utils import torch_version_is_greater_or_equal
 from super_gradients.training.utils.detection_utils import non_max_suppression, matrix_non_max_suppression, NMS_Type, DetectionPostPredictionCallback, Anchors
 from super_gradients.training.utils.utils import HpmStruct, check_img_size_divisibility, get_param
+from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
+from super_gradients.training.pipelines.pipelines import DetectionPipeline
+from super_gradients.training.processing.processing import Processing
+from super_gradients.training.utils.media.image import ImageSource
 
 COCO_DETECTION_80_CLASSES_BBOX_ANCHORS = Anchors(
     [[10, 13, 16, 30, 33, 23], [30, 61, 62, 45, 59, 119], [116, 90, 156, 198, 373, 326]], strides=[8, 16, 32]
 )  # output strides of all yolo outputs
 
 ANCHORSLESS_DUMMY_ANCHORS = Anchors([[0, 0], [0, 0], [0, 0]], strides=[8, 16, 32])
 
@@ -76,25 +82,29 @@
         self.iou = iou
         self.classes = classes
         self.nms_type = nms_type
         self.max_pred = max_predictions
         self.with_confidence = with_confidence
 
     def forward(self, x, device: str = None):
+        """Apply NMS to the raw output of the model and keep only top `max_predictions` results.
+
+        :param x: Raw output of the model, with x[0] expected to be a list of Tensors of shape (cx, cy, w, h, confidence, cls0, cls1, ...)
+        :return: List of Tensors of shape (x1, y1, x2, y2, conf, cls)
+        """
 
         if self.nms_type == NMS_Type.ITERATIVE:
             nms_result = non_max_suppression(x[0], conf_thres=self.conf, iou_thres=self.iou, with_confidence=self.with_confidence)
         else:
             nms_result = matrix_non_max_suppression(x[0], conf_thres=self.conf, max_num_of_detections=self.max_pred)
 
         return self._filter_max_predictions(nms_result)
 
     def _filter_max_predictions(self, res: List) -> List:
         res[:] = [im[: self.max_pred] if (im is not None and im.shape[0] > self.max_pred) else im for im in res]
-
         return res
 
 
 class Concat(nn.Module):
     """CONCATENATE A LIST OF TENSORS ALONG DIMENSION"""
 
     def __init__(self, dimension=1):
@@ -404,14 +414,87 @@
         # A FLAG TO DEFINE augment_forward IN INFERENCE
         self.augmented_inference = False
 
         if initialize_module:
             self._head = YoloHead(self.arch_params)
             self._initialize_module()
 
+        self._class_names: Optional[List[str]] = None
+        self._image_processor: Optional[Processing] = None
+        self._default_nms_iou: Optional[float] = None
+        self._default_nms_conf: Optional[float] = None
+
+    @staticmethod
+    def get_post_prediction_callback(conf: float, iou: float) -> DetectionPostPredictionCallback:
+        return YoloPostPredictionCallback(conf=conf, iou=iou)
+
+    @resolve_param("image_processor", ProcessingFactory())
+    def set_dataset_processing_params(
+        self,
+        class_names: Optional[List[str]] = None,
+        image_processor: Optional[Processing] = None,
+        iou: Optional[float] = None,
+        conf: Optional[float] = None,
+    ) -> None:
+        """Set the processing parameters for the dataset.
+
+        :param class_names:     (Optional) Names of the dataset the model was trained on.
+        :param image_processor: (Optional) Image processing objects to reproduce the dataset preprocessing used for training.
+        :param iou:             (Optional) IoU threshold for the nms algorithm
+        :param conf:            (Optional) Below the confidence threshold, prediction are discarded
+        """
+        self._class_names = class_names or self._class_names
+        self._image_processor = image_processor or self._image_processor
+        self._default_nms_iou = iou or self._default_nms_iou
+        self._default_nms_conf = conf or self._default_nms_conf
+
+    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None) -> DetectionPipeline:
+        """Instantiate the prediction pipeline of this model.
+
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        if None in (self._class_names, self._image_processor, self._default_nms_iou, self._default_nms_conf):
+            raise RuntimeError(
+                "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
+            )
+
+        iou = iou or self._default_nms_iou
+        conf = conf or self._default_nms_conf
+
+        pipeline = DetectionPipeline(
+            model=self,
+            image_processor=self._image_processor,
+            post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
+            class_names=self._class_names,
+        )
+        return pipeline
+
+    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None) -> ImagesDetectionPrediction:
+        """Predict an image or a list of images.
+
+        :param images:  Images to predict.
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        return pipeline(images)  # type: ignore
+
+    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None):
+        """Predict using webcam.
+
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline.predict_webcam()
+
     def forward(self, x):
         out = self._backbone(x)
         out = self._head(out)
         # THIS HAS NO EFFECT IF add_nms() WAS NOT DONE
         out = self._nms(out)
         return out
 
@@ -425,17 +508,15 @@
             )
 
     def _initialize_module(self):
         self._check_strides()
         self._initialize_biases()
         self._initialize_weights()
         if self.arch_params.add_nms:
-            nms_conf = self.arch_params.nms_conf
-            nms_iou = self.arch_params.nms_iou
-            self._nms = YoloPostPredictionCallback(nms_conf, nms_iou)
+            self._nms = self.get_post_prediction_callback(conf=self.arch_params.nms_conf, iou=self.arch_params.nms_iou)
 
     def _check_strides(self):
         m = self._head._modules_list[-1]  # DetectX()
         # Do inference in train mode on a dummy image to get output stride of each head output layer
         s = 128  # twice the minimum acceptable image size
         dummy_input = torch.zeros(1, self.arch_params.channels_in, s, s)
         dummy_input = dummy_input.to(next(self._backbone.parameters()).device)
```

## super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py

```diff
@@ -1,32 +1,111 @@
-from typing import Union
+from typing import Union, Optional, List
 
 from torch import Tensor
-
+from super_gradients.common.decorators.factory_decorator import resolve_param
+from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.modules import RepVGGBlock
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.models.detection_models.csp_resnet import CSPResNetBackbone
 from super_gradients.training.models.detection_models.pp_yolo_e.pan import CustomCSPPAN
 from super_gradients.training.models.detection_models.pp_yolo_e.pp_yolo_head import PPYOLOEHead
 from super_gradients.training.utils import HpmStruct
 from super_gradients.training.models.arch_params_factory import get_arch_params
+from super_gradients.training.models.detection_models.pp_yolo_e.post_prediction_callback import PPYoloEPostPredictionCallback, DetectionPostPredictionCallback
+from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
+from super_gradients.training.pipelines.pipelines import DetectionPipeline
+from super_gradients.training.processing.processing import Processing
+from super_gradients.training.utils.media.image import ImageSource
 
 
 class PPYoloE(SgModule):
     def __init__(self, arch_params):
         super().__init__()
         if isinstance(arch_params, HpmStruct):
             arch_params = arch_params.to_dict()
 
         self.backbone = CSPResNetBackbone(**arch_params["backbone"], depth_mult=arch_params["depth_mult"], width_mult=arch_params["width_mult"])
         self.neck = CustomCSPPAN(**arch_params["neck"], depth_mult=arch_params["depth_mult"], width_mult=arch_params["width_mult"])
         self.head = PPYOLOEHead(**arch_params["head"], width_mult=arch_params["width_mult"], num_classes=arch_params["num_classes"])
 
+        self._class_names: Optional[List[str]] = None
+        self._image_processor: Optional[Processing] = None
+        self._default_nms_iou: Optional[float] = None
+        self._default_nms_conf: Optional[float] = None
+
+    @staticmethod
+    def get_post_prediction_callback(conf: float, iou: float) -> DetectionPostPredictionCallback:
+        return PPYoloEPostPredictionCallback(score_threshold=conf, nms_threshold=iou, nms_top_k=1000, max_predictions=300)
+
+    @resolve_param("image_processor", ProcessingFactory())
+    def set_dataset_processing_params(
+        self,
+        class_names: Optional[List[str]] = None,
+        image_processor: Optional[Processing] = None,
+        iou: Optional[float] = None,
+        conf: Optional[float] = None,
+    ) -> None:
+        """Set the processing parameters for the dataset.
+
+        :param class_names:     (Optional) Names of the dataset the model was trained on.
+        :param image_processor: (Optional) Image processing objects to reproduce the dataset preprocessing used for training.
+        :param iou:             (Optional) IoU threshold for the nms algorithm
+        :param conf:            (Optional) Below the confidence threshold, prediction are discarded
+        """
+        self._class_names = class_names or self._class_names
+        self._image_processor = image_processor or self._image_processor
+        self._default_nms_iou = iou or self._default_nms_iou
+        self._default_nms_conf = conf or self._default_nms_conf
+
+    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None) -> DetectionPipeline:
+        """Instantiate the prediction pipeline of this model.
+
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        if None in (self._class_names, self._image_processor, self._default_nms_iou, self._default_nms_conf):
+            raise RuntimeError(
+                "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
+            )
+
+        iou = iou or self._default_nms_iou
+        conf = conf or self._default_nms_conf
+
+        pipeline = DetectionPipeline(
+            model=self,
+            image_processor=self._image_processor,
+            post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
+            class_names=self._class_names,
+        )
+        return pipeline
+
+    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None) -> ImagesDetectionPrediction:
+        """Predict an image or a list of images.
+
+        :param images:  Images to predict.
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        return pipeline(images)  # type: ignore
+
+    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None):
+        """Predict using webcam.
+
+        :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
+        :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
+                        If None, the default value associated to the training is used.
+        """
+        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline.predict_webcam()
+
     def forward(self, x: Tensor):
         features = self.backbone(x)
         features = self.neck(features)
         return self.head(features)
 
     def prep_model_for_conversion(self, input_size: Union[tuple, list] = None, **kwargs):
         """
```

## super_gradients/training/models/kd_modules/kd_module.py

```diff
@@ -20,26 +20,28 @@
 
     attributes:
         student: SgModule - the student model
         teacher: torch.nn.Module- the teacher model
         run_teacher_on_eval: bool- whether to run self.teacher at eval mode regardless of self.train(mode)
         arch_params: HpmStruct- Architecture H.P.
 
-        Additionally, by passing teacher_input_adapter (torch.nn.Module) one can modify the teacher net s.t
-        teacher = torch.nn.Sequential(teacher_input_adapter, teacher). This is useful when teacher net expects a
-        different input format from the student (for example different normalization).
+            Additionally, by passing teacher_input_adapter (torch.nn.Module) one can modify the teacher net to act as if
+            teacher = torch.nn.Sequential(teacher_input_adapter, teacher). This is useful when teacher net expects a
+            different input format from the student (for example different normalization).
+            Equivalent arg for the student model, can be passed through student_input_adapter.
 
     """
 
     def __init__(self, arch_params: HpmStruct, student: SgModule, teacher: torch.nn.Module, run_teacher_on_eval=False):
         super(KDModule, self).__init__()
         self.arch_params = arch_params
         self.student = student
         self.teacher = teacher
         self.teacher_input_adapter = get_param(self.arch_params, "teacher_input_adapter")
+        self.student_input_adapter = get_param(self.arch_params, "student_input_adapter")
         self.run_teacher_on_eval = run_teacher_on_eval
         self._freeze_teacher()
 
         # WHEN CREATING A MODULE SELF.TRAIN() ISN'T CALLED AND SO THE TEACHER MUST BE MOVED TO EVAL MODE EXPLICITLY
         if self.run_teacher_on_eval:
             self.teacher.eval()
 
@@ -58,18 +60,25 @@
             self.teacher.train(mode)
 
     def eval(self):
         self.student.eval()
         self.teacher.eval()
 
     def forward(self, x):
+        if self.student_input_adapter is not None:
+            student_output = self.student(self.student_input_adapter(x))
+        else:
+            student_output = self.student(x)
+
         if self.teacher_input_adapter is not None:
-            return KDOutput(student_output=self.student(x), teacher_output=self.teacher(self.teacher_input_adapter(x)))
+            teacher_output = self.teacher(self.teacher_input_adapter(x))
         else:
-            return KDOutput(student_output=self.student(x), teacher_output=self.teacher(x))
+            teacher_output = self.teacher(x)
+
+        return KDOutput(student_output=student_output, teacher_output=teacher_output)
 
     def initialize_param_groups(self, lr: float, training_params: HpmStruct) -> list:
         return self.student.initialize_param_groups(lr, training_params)
 
     def update_param_groups(self, param_groups: list, lr: float, epoch: int, iter: int, training_params: HpmStruct, total_batch: int) -> list:
         return self.student.update_param_groups(param_groups, lr, epoch, iter, training_params, total_batch)
```

## super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py

```diff
@@ -3,18 +3,26 @@
 
 from omegaconf import DictConfig
 
 from super_gradients.common.object_names import Models
 from super_gradients.common.registry.registry import register_model
 from super_gradients.training.models.arch_params_factory import get_arch_params
 from super_gradients.training.models.detection_models.customizable_detector import CustomizableDetector
-from super_gradients.training.utils import HpmStruct
+from super_gradients.training.utils import HpmStruct, get_param
 
 POSE_DDRNET39_ARCH_PARAMS = get_arch_params("pose_ddrnet39_arch_params")
 
 
 @register_model(Models.POSE_DDRNET_39)
 class PoseDDRNet39(CustomizableDetector):
     def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
         merged_arch_params = HpmStruct(**copy.deepcopy(POSE_DDRNET39_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
-        super().__init__(merged_arch_params, in_channels=in_channels)
+        super().__init__(
+            backbone=merged_arch_params.backbone,
+            heads=merged_arch_params.heads,
+            num_classes=get_param(merged_arch_params, "num_classes", None),
+            bn_eps=get_param(merged_arch_params, "bn_eps", None),
+            bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
+            inplace_act=get_param(merged_arch_params, "inplace_act", True),
+            in_channels=in_channels,
+        )
```

## super_gradients/training/models/pose_estimation_models/pose_ppyolo.py

```diff
@@ -3,18 +3,27 @@
 
 from omegaconf import DictConfig
 
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.training.models.arch_params_factory import get_arch_params
 from super_gradients.training.models.detection_models.customizable_detector import CustomizableDetector
-from super_gradients.training.utils import HpmStruct
+from super_gradients.training.utils import HpmStruct, get_param
 
 DEKR_PPPOSE_L_ARCH_PARAMS = get_arch_params("pose_pppose_l_arch_params")
 
 
 @register_model(Models.POSE_PP_YOLO_L)
 class PosePPYoloL(CustomizableDetector):
     def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
         merged_arch_params = HpmStruct(**copy.deepcopy(DEKR_PPPOSE_L_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
-        super().__init__(merged_arch_params, in_channels=in_channels)
+        super().__init__(
+            backbone=merged_arch_params.backbone,
+            neck=merged_arch_params.neck,
+            heads=merged_arch_params.heads,
+            num_classes=get_param(merged_arch_params, "num_classes", None),
+            bn_eps=get_param(merged_arch_params, "bn_eps", None),
+            bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
+            inplace_act=get_param(merged_arch_params, "inplace_act", True),
+            in_channels=in_channels,
+        )
```

## super_gradients/training/sg_trainer/sg_trainer.py

```diff
@@ -14,14 +14,15 @@
 from torch.cuda.amp import GradScaler, autocast
 from torch.utils.data import DataLoader, SequentialSampler
 from torch.utils.data.distributed import DistributedSampler
 from torchmetrics import MetricCollection
 from tqdm import tqdm
 
 from super_gradients.common.environment.checkpoints_dir_utils import get_checkpoints_dir_path, get_ckpt_local_path
+from super_gradients.module_interfaces import HasPreprocessingParams, HasPredict
 
 from super_gradients.training.utils.sg_trainer_utils import get_callable_param_names
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.sg_loggers.abstract_sg_logger import AbstractSGLogger
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.data_types.enum import MultiGPUMode, StrictLoad, EvaluationType
 from super_gradients.common.decorators.factory_decorator import resolve_param
@@ -190,14 +191,16 @@
         self.train_metrics, self.valid_metrics = default_train_metrics, default_valid_metrics
 
         self.train_monitored_values = {}
         self.valid_monitored_values = {}
         self.max_train_batches = None
         self.max_valid_batches = None
 
+        self._epoch_start_logging_values = {}
+
     @property
     def device(self) -> str:
         return device_config.device
 
     @classmethod
     def train_from_config(cls, cfg: Union[DictConfig, dict]) -> Tuple[nn.Module, Tuple]:
         """
@@ -438,17 +441,16 @@
 
                 # COMPUTE THE LOSS FOR BACK PROP + EXTRA METRICS COMPUTED DURING THE LOSS FORWARD PASS
                 loss, loss_log_items = self._get_losses(outputs, targets)
 
             context.update_context(preds=outputs, loss_log_items=loss_log_items)
             self.phase_callback_handler.on_train_batch_loss_end(context)
 
-            # LOG LR THAT WILL BE USED IN CURRENT EPOCH AND AFTER FIRST WARMUP/LR_SCHEDULER UPDATE BEFORE WEIGHT UPDATE
             if not self.ddp_silent_mode and batch_idx == 0:
-                self._write_lrs(epoch)
+                self._epoch_start_logging_values = self._get_epoch_start_logging_values()
 
             self._backward_step(loss, epoch, batch_idx, context)
 
             # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
             logging_values = loss_avg_meter.average + get_metrics_results_tuple(self.train_metrics)
             gpu_memory_utilization = get_gpu_mem_utilization() / 1e9 if torch.cuda.is_available() else 0
 
@@ -594,14 +596,18 @@
             state["optimizer_state_dict"] = optimizer.state_dict()
 
         if self.scaler is not None:
             state["scaler_state_dict"] = self.scaler.state_dict()
 
         if self.ema:
             state["ema_net"] = self.ema_model.ema.state_dict()
+
+        if isinstance(self.net.module, HasPredict) and isinstance(self.valid_loader.dataset, HasPreprocessingParams):
+            state["processing_params"] = self.valid_loader.dataset.get_dataset_preprocessing_params()
+
         # SAVES CURRENT MODEL AS ckpt_latest
         self.sg_logger.add_checkpoint(tag="ckpt_latest.pth", state_dict=state, global_step=epoch)
 
         # SAVE MODEL AT SPECIFIC EPOCHS DETERMINED BY save_ckpt_epoch_list
         if epoch in self.training_params.save_ckpt_epoch_list:
             self.sg_logger.add_checkpoint(tag=f"ckpt_epoch_{epoch}.pth", state_dict=state, global_step=epoch)
 
@@ -1209,17 +1215,19 @@
         inputs, _, _ = sg_trainer_utils.unpack_batch_items(first_batch)
 
         log_main_training_params(
             multi_gpu=device_config.multi_gpu,
             num_gpus=get_world_size(),
             batch_size=len(inputs),
             batch_accumulate=self.batch_accumulate,
-            len_train_set=len(self.train_loader.dataset),
+            train_dataset_length=len(self.train_loader.dataset),
+            train_dataloader_len=len(self.train_loader),
         )
 
+        self._set_net_preprocessing_from_valid_loader()
         try:
             # HEADERS OF THE TRAINING PROGRESS
             if not silent_mode:
                 logger.info(f"Started training for {self.max_epochs - self.start_epoch} epochs ({self.start_epoch}/" f"{self.max_epochs - 1})\n")
             for epoch in range(self.start_epoch, self.max_epochs):
                 if context.stop_training:
                     logger.info("Request to stop training has been received, stopping training")
@@ -1283,15 +1291,22 @@
                     self.phase_callback_handler.on_validation_loader_end(context)
 
                 if self.ema:
                     self.net = keep_model
 
                 if not self.ddp_silent_mode:
                     # SAVING AND LOGGING OCCURS ONLY IN THE MAIN PROCESS (IN CASES THERE ARE SEVERAL PROCESSES - DDP)
-                    self._write_to_disk_operations(train_metrics_tuple, validation_results_tuple, inf_time, epoch, context)
+                    self._write_to_disk_operations(
+                        train_metrics=train_metrics_tuple,
+                        validation_results=validation_results_tuple,
+                        lr_dict=self._epoch_start_logging_values,
+                        inf_time=inf_time,
+                        epoch=epoch,
+                        context=context,
+                    )
                     self.sg_logger.upload()
 
             # Evaluating the average model and removing snapshot averaging file if training is completed
             if self.training_params.average_best_models:
                 self._validate_final_average_model(cleanup_snapshots_pkl_file=True)
 
         except KeyboardInterrupt:
@@ -1309,14 +1324,24 @@
 
             # PHASE.TRAIN_END
             self.phase_callback_handler.on_training_end(context)
 
             if not self.ddp_silent_mode:
                 self.sg_logger.close()
 
+    def _set_net_preprocessing_from_valid_loader(self):
+        if isinstance(self.net.module, HasPredict) and isinstance(self.valid_loader.dataset, HasPreprocessingParams):
+            try:
+                self.net.module.set_dataset_processing_params(**self.valid_loader.dataset.get_dataset_preprocessing_params())
+            except Exception as e:
+                logger.warning(
+                    f"Could not set preprocessing pipeline from the validation dataset:\n {e}.\n Before calling"
+                    "predict make sure to call set_dataset_processing_params."
+                )
+
     def _reset_best_metric(self):
         self.best_metric = -1 * np.inf if self.greater_metric_to_watch_is_better else np.inf
 
     def _reset_metrics(self):
         for metric in ("train_metrics", "valid_metrics", "test_metrics"):
             if hasattr(self, metric) and getattr(self, metric) is not None:
                 getattr(self, metric).reset()
@@ -1628,32 +1653,35 @@
             "checkpoint_params": self.checkpoint_params.__dict__,
             "training_hyperparams": self.training_params.__dict__,
             "dataset_params": self.dataset_params.__dict__,
             "additional_log_items": additional_log_items,
         }
         return hyper_param_config
 
-    def _write_to_disk_operations(self, train_metrics: tuple, validation_results: tuple, inf_time: float, epoch: int, context: PhaseContext):
+    def _write_to_disk_operations(self, train_metrics: tuple, validation_results: tuple, lr_dict: dict, inf_time: float, epoch: int, context: PhaseContext):
         """Run the various logging operations, e.g.: log file, Tensorboard, save checkpoint etc."""
         # STORE VALUES IN A TENSORBOARD FILE
         train_results = list(train_metrics) + list(validation_results) + [inf_time]
         all_titles = self.results_titles + ["Inference Time"]
 
         result_dict = {all_titles[i]: train_results[i] for i in range(len(train_results))}
         self.sg_logger.add_scalars(tag_scalar_dict=result_dict, global_step=epoch)
+        self.sg_logger.add_scalars(tag_scalar_dict=lr_dict, global_step=epoch)
 
         # SAVE THE CHECKPOINT
         if self.training_params.save_model:
             self._save_checkpoint(self.optimizer, epoch + 1, validation_results, context)
 
-    def _write_lrs(self, epoch):
+    def _get_epoch_start_logging_values(self) -> dict:
+        """Get all the values that should be logged at the start of each epoch.
+        This is useful for values like Learning Rate that can change over an epoch."""
         lrs = [self.optimizer.param_groups[i]["lr"] for i in range(len(self.optimizer.param_groups))]
         lr_titles = ["LR/Param_group_" + str(i) for i in range(len(self.optimizer.param_groups))] if len(self.optimizer.param_groups) > 1 else ["LR"]
         lr_dict = {lr_titles[i]: lrs[i] for i in range(len(lrs))}
-        self.sg_logger.add_scalars(tag_scalar_dict=lr_dict, global_step=epoch)
+        return lr_dict
 
     def test(
         self,
         model: nn.Module = None,
         test_loader: torch.utils.data.DataLoader = None,
         loss: torch.nn.modules.loss._Loss = None,
         silent_mode: bool = False,
```

## super_gradients/training/transforms/transforms.py

```diff
@@ -7,25 +7,34 @@
 import cv2
 import numpy as np
 import torch.nn
 from PIL import Image, ImageFilter, ImageOps
 from torchvision import transforms as transforms
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
-from super_gradients.common.object_names import Transforms
+from super_gradients.common.object_names import Transforms, Processings
 from super_gradients.common.registry.registry import register_transform
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.data_formats_factory import ConcatenatedTensorFormatFactory
-from super_gradients.training.utils.detection_utils import get_mosaic_coordinate, adjust_box_anns, xyxy2cxcywh, cxcywh2xyxy, DetectionTargetsFormat
+from super_gradients.training.utils.detection_utils import get_mosaic_coordinate, adjust_box_anns, DetectionTargetsFormat
 from super_gradients.training.datasets.data_formats import ConcatenatedTensorFormatConverter
 from super_gradients.training.datasets.data_formats.formats import filter_on_bboxes, ConcatenatedTensorFormat
 from super_gradients.training.datasets.data_formats.default_formats import XYXY_LABEL, LABEL_CXCYWH
+from super_gradients.training.transforms.utils import (
+    _rescale_and_pad_to_size,
+    _rescale_image,
+    _rescale_bboxes,
+    _get_center_padding_coordinates,
+    _pad_image,
+    _shift_bboxes,
+    _rescale_xyxy_bboxes,
+)
 
-image_resample = Image.BILINEAR
-mask_resample = Image.NEAREST
+IMAGE_RESAMPLE_MODE = Image.BILINEAR
+MASK_RESAMPLE_MODE = Image.NEAREST
 
 logger = get_logger(__name__)
 
 
 class SegmentationTransform:
     def __call__(self, *args, **kwargs):
         raise NotImplementedError
@@ -39,16 +48,16 @@
     def __init__(self, h, w):
         self.h = h
         self.w = w
 
     def __call__(self, sample):
         image = sample["image"]
         mask = sample["mask"]
-        sample["image"] = image.resize((self.w, self.h), image_resample)
-        sample["mask"] = mask.resize((self.w, self.h), mask_resample)
+        sample["image"] = image.resize((self.w, self.h), IMAGE_RESAMPLE_MODE)
+        sample["mask"] = mask.resize((self.w, self.h), MASK_RESAMPLE_MODE)
         return sample
 
 
 @register_transform(Transforms.SegRandomFlip)
 class SegRandomFlip(SegmentationTransform):
     """
     Randomly flips the image and mask (synchronously) with probability 'prob'.
@@ -102,16 +111,16 @@
             scale = self.short_size / short_size
         else:
             long_size = max(w, h)
             scale = self.long_size / long_size
 
         out_size = int(scale * w), int(scale * h)
 
-        image = image.resize(out_size, image_resample)
-        mask = mask.resize(out_size, mask_resample)
+        image = image.resize(out_size, IMAGE_RESAMPLE_MODE)
+        mask = mask.resize(out_size, MASK_RESAMPLE_MODE)
 
         sample["image"] = image
         sample["mask"] = mask
 
         return sample
 
     def check_valid_arguments(self):
@@ -145,16 +154,16 @@
         image = sample["image"]
         mask = sample["mask"]
         w, h = image.size
 
         scale = random.uniform(self.scales[0], self.scales[1])
         out_size = int(scale * w), int(scale * h)
 
-        image = image.resize(out_size, image_resample)
-        mask = mask.resize(out_size, mask_resample)
+        image = image.resize(out_size, IMAGE_RESAMPLE_MODE)
+        mask = mask.resize(out_size, MASK_RESAMPLE_MODE)
 
         sample["image"] = image
         sample["mask"] = mask
 
         return sample
 
     def check_valid_arguments(self):
@@ -190,16 +199,16 @@
         self.check_valid_arguments()
 
     def __call__(self, sample: dict) -> dict:
         image = sample["image"]
         mask = sample["mask"]
 
         deg = random.uniform(self.min_deg, self.max_deg)
-        image = image.rotate(deg, resample=image_resample, fillcolor=self.fill_image)
-        mask = mask.rotate(deg, resample=mask_resample, fillcolor=self.fill_mask)
+        image = image.rotate(deg, resample=IMAGE_RESAMPLE_MODE, fillcolor=self.fill_image)
+        mask = mask.rotate(deg, resample=MASK_RESAMPLE_MODE, fillcolor=self.fill_mask)
 
         sample["image"] = image
         sample["mask"] = mask
 
         return sample
 
     def check_valid_arguments(self):
@@ -286,18 +295,17 @@
     """
     Pads image to 'crop_size'.
     Should be called only after "SegRescale" or "SegRandomRescale" in augmentations pipeline.
     """
 
     def __init__(self, crop_size: Union[float, Tuple, List], fill_mask: int = 0, fill_image: Union[int, Tuple, List] = 0):
         """
-        :param crop_size: tuple of (width, height) for the final crop size, if is scalar size is a
-            square (crop_size, crop_size)
-        :param fill_mask: value to fill mask labels background.
-        :param fill_image: grey value to fill image padded background.
+        :param crop_size:   Tuple of (width, height) for the final crop size, if is scalar size is a square (crop_size, crop_size)
+        :param fill_mask:   Value to fill mask labels background.
+        :param fill_image:  Grey value to fill image padded background.
         """
         # CHECK IF CROP SIZE IS A ITERABLE OR SCALAR
         self.crop_size = crop_size
         self.fill_mask = fill_mask
         self.fill_image = tuple(fill_image) if isinstance(fill_image, Sequence) else fill_image
 
         self.check_valid_arguments()
@@ -412,14 +420,17 @@
 
     def __call__(self, sample: Union[dict, list]):
         raise NotImplementedError
 
     def __repr__(self):
         return self.__class__.__name__ + str(self.__dict__).replace("{", "(").replace("}", ")")
 
+    def get_equivalent_preprocessing(self) -> List:
+        raise NotImplementedError
+
 
 @register_transform(Transforms.DetectionStandardize)
 class DetectionStandardize(DetectionTransform):
     """
     Standardize image pixel values with img/max_val
 
     :param max_val: Current maximum value of the image pixels. (usually 255)
@@ -429,14 +440,17 @@
         super().__init__()
         self.max_value = max_value
 
     def __call__(self, sample: dict) -> dict:
         sample["image"] = (sample["image"] / self.max_value).astype(np.float32)
         return sample
 
+    def get_equivalent_preprocessing(self) -> List[Dict]:
+        return [{Processings.StandardizeImage: {"max_value": self.max_value}}]
+
 
 @register_transform(Transforms.DetectionMosaic)
 class DetectionMosaic(DetectionTransform):
     """
     DetectionMosaic detection transform
 
     :param input_dim:       Input dimension.
@@ -705,14 +719,17 @@
         super().__init__()
         self.dims = tuple(dims)
 
     def __call__(self, sample: Dict[str, np.array]) -> dict:
         sample["image"] = np.ascontiguousarray(sample["image"].transpose(*self.dims))
         return sample
 
+    def get_equivalent_preprocessing(self) -> List[Dict]:
+        return [{Processings.ImagePermute: {"permutation": self.dims}}]
+
 
 @register_transform(Transforms.DetectionPadToSize)
 class DetectionPadToSize(DetectionTransform):
     """
     Preprocessing transform to pad image and bboxes to `input_dim` shape (rows, cols).
     Transform does center padding, so that input image with bboxes located in the center of the produced image.
 
@@ -727,53 +744,25 @@
         :param pad_value: Padding value for image
         """
         super().__init__()
         self.output_size = output_size
         self.pad_value = pad_value
 
     def __call__(self, sample: dict) -> dict:
-        img, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
-        img, shift_w, shift_h = self._apply_to_image(img, final_shape=self.output_size, pad_value=self.pad_value)
-        sample["image"] = img
-        sample["target"] = self._apply_to_bboxes(targets, shift_w, shift_h)
+        image, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
+        padding_coordinates = _get_center_padding_coordinates(input_shape=image.shape, output_shape=self.output_size)
+
+        sample["image"] = _pad_image(image=image, padding_coordinates=padding_coordinates, pad_value=self.pad_value)
+        sample["target"] = _shift_bboxes(targets=targets, shift_w=padding_coordinates.left, shift_h=padding_coordinates.top)
         if crowd_targets is not None:
-            sample["crowd_target"] = self._apply_to_bboxes(crowd_targets, shift_w, shift_h)
+            sample["crowd_target"] = _shift_bboxes(targets=crowd_targets, shift_w=padding_coordinates.left, shift_h=padding_coordinates.top)
         return sample
 
-    def _apply_to_bboxes(self, targets: np.array, shift_w: float, shift_h: float) -> np.array:
-        """Translate bboxes with respect to padding values.
-
-        :param targets:  Bboxes to transform of shape (N, 5).
-                         Bboxes expected to have format [x1, y1, x2, y2, class_id, ...]
-        :param shift_w:  shift width in pixels
-        :param shift_h:  shift height in pixels
-        :return:         Bboxes to transform of shape (N, 5)
-                         Bboxes will have same format [x1, y1, x2, y2, class_id, ...]
-        """
-        targets = targets.copy() if len(targets) > 0 else np.zeros((0, 5), dtype=np.float32)
-        boxes, labels = targets[:, :4], targets[:, 4:]
-        boxes[:, [0, 2]] += shift_w
-        boxes[:, [1, 3]] += shift_h
-        return np.concatenate((boxes, labels), 1)
-
-    def _apply_to_image(self, image, final_shape: Tuple[int, int], pad_value: int):
-        """
-        Pad image to final_shape.
-        :param image:
-        :param final_shape: Output image size (rows, cols).
-        :param pad_value:
-        :return:
-        """
-        pad_h, pad_w = final_shape[0] - image.shape[0], final_shape[1] - image.shape[1]
-        shift_h, shift_w = pad_h // 2, pad_w // 2
-        pad_h = (shift_h, pad_h - shift_h)
-        pad_w = (shift_w, pad_w - shift_w)
-
-        image = np.pad(image, (pad_h, pad_w, (0, 0)), "constant", constant_values=pad_value)
-        return image, shift_w, shift_h
+    def get_equivalent_preprocessing(self) -> List:
+        return [{Processings.DetectionCenterPadding: {"output_shape": self.output_size, "pad_value": self.pad_value}}]
 
 
 @register_transform(Transforms.DetectionPaddedRescale)
 class DetectionPaddedRescale(DetectionTransform):
     """
     Preprocessing transform to be applied last of all transforms for validation.
 
@@ -790,37 +779,28 @@
         self.swap = swap
         self.input_dim = input_dim
         self.max_targets = max_targets
         self.pad_value = pad_value
 
     def __call__(self, sample: dict) -> dict:
         img, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
-        img, r = rescale_and_pad_to_size(img, self.input_dim, self.swap, self.pad_value)
+        img, r = _rescale_and_pad_to_size(img, self.input_dim, self.swap, self.pad_value)
 
         sample["image"] = img
-        sample["target"] = self._rescale_target(targets, r)
+        sample["target"] = _rescale_xyxy_bboxes(targets, r)
         if crowd_targets is not None:
-            sample["crowd_target"] = self._rescale_target(crowd_targets, r)
+            sample["crowd_target"] = _rescale_xyxy_bboxes(crowd_targets, r)
         return sample
 
-    def _rescale_target(self, targets: np.array, r: float) -> np.array:
-        """SegRescale the target according to a coefficient used to rescale the image.
-        This is done to have images and targets at the same scale.
-
-        :param targets:  Targets to rescale, shape (batch_size, 6)
-        :param r:        SegRescale coefficient that was applied to the image
-
-        :return:         Rescaled targets, shape (batch_size, 6)
-        """
-        targets = targets.copy() if len(targets) > 0 else np.zeros((self.max_targets, 5), dtype=np.float32)
-        boxes, labels = targets[:, :4], targets[:, 4]
-        boxes = xyxy2cxcywh(boxes)
-        boxes *= r
-        boxes = cxcywh2xyxy(boxes)
-        return np.concatenate((boxes, labels[:, np.newaxis]), 1)
+    def get_equivalent_preprocessing(self) -> List[Dict]:
+        return [
+            {Processings.DetectionLongestMaxSizeRescale: {"output_shape": self.input_dim}},
+            {Processings.DetectionBottomRightPadding: {"output_shape": self.input_dim, "pad_value": self.pad_value}},
+            {Processings.ImagePermute: {"permutation": self.swap}},
+        ]
 
 
 @register_transform(Transforms.DetectionHorizontalFlip)
 class DetectionHorizontalFlip(DetectionTransform):
     """
     Horizontal Flip for Detection
 
@@ -855,47 +835,26 @@
     """
 
     def __init__(self, output_shape: Tuple[int, int]):
         super().__init__()
         self.output_shape = output_shape
 
     def __call__(self, sample: dict) -> dict:
-        img, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
+        image, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
 
-        img_resized, scale_factors = self._rescale_image(img)
+        sy, sx = (self.output_shape[0] / image.shape[0], self.output_shape[1] / image.shape[1])
 
-        sample["image"] = img_resized
-        sample["target"] = self._rescale_target(targets, scale_factors)
+        sample["image"] = _rescale_image(image=image, target_shape=self.output_shape)
+        sample["target"] = _rescale_bboxes(targets, scale_factors=(sy, sx))
         if crowd_targets is not None:
-            sample["crowd_target"] = self._rescale_target(crowd_targets, scale_factors)
+            sample["crowd_target"] = _rescale_bboxes(crowd_targets, scale_factors=(sy, sx))
         return sample
 
-    def _rescale_image(self, image):
-        sy, sx = self.output_shape[0] / image.shape[0], self.output_shape[1] / image.shape[1]
-        resized_img = cv2.resize(
-            image,
-            dsize=(int(self.output_shape[1]), int(self.output_shape[0])),
-            interpolation=cv2.INTER_LINEAR,
-        )
-        scale_factors = sy, sx
-        return resized_img, scale_factors
-
-    def _rescale_target(self, targets: np.array, scale_factors: Tuple[float, float]) -> np.array:
-        """SegRescale the target according to a coefficient used to rescale the image.
-        This is done to have images and targets at the same scale.
-
-        :param targets:  Target XYXY bboxes to rescale, shape (num_boxes, 5)
-        :param r:        SegRescale coefficient that was applied to the image
-
-        :return:         Rescaled targets, shape (num_boxes, 5)
-        """
-        sy, sx = scale_factors
-        targets = targets.astype(np.float32, copy=True) if len(targets) > 0 else np.zeros((0, 5), dtype=np.float32)
-        targets[:, 0:4] *= np.array([[sx, sy, sx, sy]], dtype=targets.dtype)
-        return targets
+    def get_equivalent_preprocessing(self) -> List[Dict]:
+        return [{Processings.DetectionRescale: {"output_shape": self.output_size}}]
 
 
 @register_transform(Transforms.DetectionRandomRotate90)
 class DetectionRandomRotate90(DetectionTransform):
     def __init__(self, prob: float = 0.5):
         super().__init__()
         self.prob = prob
@@ -966,14 +925,19 @@
         if sample["image"].shape[2] < 3:
             raise ValueError("DetectionRGB2BGR transform expects at least 3 channels, got: " + str(sample["image"].shape[2]))
 
         if random.random() < self.prob:
             sample["image"] = sample["image"][..., ::-1]
         return sample
 
+    def get_equivalent_preprocessing(self) -> List:
+        if self.prob < 1:
+            raise RuntimeError("Cannot set preprocessing pipeline with randomness. Set prob to 1.")
+        return [{Processings.ReverseImageChannels}]
+
 
 @register_transform(Transforms.DetectionHSV)
 class DetectionHSV(DetectionTransform):
     """
     Detection HSV transform.
 
     :param prob:            Probability to apply the transform.
@@ -1020,14 +984,17 @@
         self.mean = np.array(list(mean)).reshape((1, 1, -1)).astype(np.float32)
         self.std = np.array(list(std)).reshape((1, 1, -1)).astype(np.float32)
 
     def __call__(self, sample: dict) -> dict:
         sample["image"] = (sample["image"] - self.mean) / self.std
         return sample
 
+    def get_equivalent_preprocessing(self) -> List[Dict]:
+        return [{Processings.NormalizeImage: {"mean": self.mean, "std": self.std}}]
+
 
 @register_transform(Transforms.DetectionTargetsFormatTransform)
 class DetectionTargetsFormatTransform(DetectionTransform):
     """
     Detection targets format transform
 
     Convert targets in input_format to output_format, filter small bboxes and pad targets.
@@ -1104,14 +1071,17 @@
     def pad_targets(self, targets: np.ndarray) -> np.ndarray:
         """Pad targets."""
         padded_targets = np.zeros((self.max_targets, targets.shape[-1]))
         padded_targets[range(len(targets))[: self.max_targets]] = targets[: self.max_targets]
         padded_targets = np.ascontiguousarray(padded_targets, dtype=np.float32)
         return padded_targets
 
+    def get_equivalent_preprocessing(self) -> List:
+        return []
+
 
 def get_aug_params(value: Union[tuple, float], center: float = 0) -> float:
     """
     Generates a random value for augmentations as described below
 
     :param value:       Range of values for generation. Wen tuple-drawn uniformly between (value[0], value[1]), and (center - value, center + value) when float.
     :param center:      Center to subtract when value is float.
@@ -1331,42 +1301,14 @@
     img_hsv[..., 0] = (img_hsv[..., 0] + hsv_augs[0]) % 180
     img_hsv[..., 1] = np.clip(img_hsv[..., 1] + hsv_augs[1], 0, 255)
     img_hsv[..., 2] = np.clip(img_hsv[..., 2] + hsv_augs[2], 0, 255)
 
     img[..., bgr_channels] = cv2.cvtColor(img_hsv.astype(img.dtype), cv2.COLOR_HSV2BGR)  # no return needed
 
 
-def rescale_and_pad_to_size(img, input_size, swap=(2, 0, 1), pad_val=114):
-    """
-    Rescales image according to minimum ratio between the target height /image height, target width / image width,
-    and pads the image to the target size.
-
-    :param img: Image to be rescaled
-    :param input_size: Target size
-    :param swap: Axis's to be rearranged.
-    :return: rescaled image, ratio
-    """
-    if len(img.shape) == 3:
-        padded_img = np.ones((input_size[0], input_size[1], img.shape[-1]), dtype=np.uint8) * pad_val
-    else:
-        padded_img = np.ones(input_size, dtype=np.uint8) * pad_val
-
-    r = min(input_size[0] / img.shape[0], input_size[1] / img.shape[1])
-    resized_img = cv2.resize(
-        img,
-        (int(img.shape[1] * r), int(img.shape[0] * r)),
-        interpolation=cv2.INTER_LINEAR,
-    ).astype(np.uint8)
-    padded_img[: int(img.shape[0] * r), : int(img.shape[1] * r)] = resized_img
-
-    padded_img = padded_img.transpose(swap)
-    padded_img = np.ascontiguousarray(padded_img, dtype=np.float32)
-    return padded_img, r
-
-
 @register_transform(Transforms.Standardize)
 class Standardize(torch.nn.Module):
     """
     Standardize image pixel values.
     :return img/max_val
 
     attributes:
```

## super_gradients/training/utils/checkpoint_utils.py

```diff
@@ -3,14 +3,15 @@
 import pkg_resources
 import collections
 import torch
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.data_interface.adnn_model_repository_data_interface import ADNNModelRepositoryDataInterfaces
 from super_gradients.common.decorators.explicit_params_validator import explicit_params_validation
+from super_gradients.module_interfaces import HasPredict
 from super_gradients.training.pretrained_models import MODEL_URLS
 from super_gradients.common.data_types import StrictLoad
 
 from torch import nn, Tensor
 from typing import Union, Mapping
 
 try:
@@ -182,24 +183,28 @@
 def load_checkpoint_to_model(
     net: torch.nn.Module,
     ckpt_local_path: str,
     load_backbone: bool = False,
     strict: Union[str, StrictLoad] = StrictLoad.NO_KEY_MATCHING,
     load_weights_only: bool = False,
     load_ema_as_net: bool = False,
+    load_processing_params: bool = False,
 ):
     """
     Loads the state dict in ckpt_local_path to net and returns the checkpoint's state dict.
 
+
     :param load_ema_as_net: Will load the EMA inside the checkpoint file to the network when set
     :param ckpt_local_path: local path to the checkpoint file
     :param load_backbone: whether to load the checkpoint as a backbone
     :param net: network to load the checkpoint to
     :param strict:
-    :param load_weights_only:
+    :param load_weights_only: Whether to ignore all other entries other then "net".
+    :param load_processing_params: Whether to call set_dataset_processing_params on "processing_params" entry inside the
+     checkpoint file (default=False).
     :return:
     """
     if isinstance(strict, str):
         strict = StrictLoad(strict)
 
     if ckpt_local_path is None or not os.path.exists(ckpt_local_path):
         error_msg = "Error - loading Model Checkpoint: Path {} does not exist".format(ckpt_local_path)
@@ -223,14 +228,25 @@
     else:
         adaptive_load_state_dict(net, checkpoint, strict)
 
     message_suffix = " checkpoint." if not load_ema_as_net else " EMA checkpoint."
     message_model = "model" if not load_backbone else "model's backbone"
     logger.info("Successfully loaded " + message_model + " weights from " + ckpt_local_path + message_suffix)
 
+    if (isinstance(net, HasPredict) or (hasattr(net, "module") and isinstance(net.module, HasPredict))) and load_processing_params:
+        if "processing_params" not in checkpoint.keys():
+            raise ValueError("Can't load processing params - could not find any stored in checkpoint file.")
+        try:
+            net.set_dataset_processing_params(**checkpoint["processing_params"])
+        except Exception as e:
+            logger.warning(
+                f"Could not set preprocessing pipeline from the checkpoint dataset: {e}. Before calling"
+                "predict make sure to call set_dataset_processing_params."
+            )
+
     if load_weights_only or load_backbone:
         # DISCARD ALL THE DATA STORED IN CHECKPOINT OTHER THAN THE WEIGHTS
         [checkpoint.pop(key) for key in list(checkpoint.keys()) if key != "net"]
 
     return checkpoint
```

## super_gradients/training/utils/detection_utils.py

```diff
@@ -55,17 +55,17 @@
 
 def _set_batch_labels_index(labels_batch):
     for i, labels in enumerate(labels_batch):
         labels[:, 0] = i
     return labels_batch
 
 
-def convert_xywh_bbox_to_xyxy(input_bbox: torch.Tensor):
+def convert_cxcywh_bbox_to_xyxy(input_bbox: torch.Tensor):
     """
-    Converts bounding box format from [x, y, w, h] to [x1, y1, x2, y2]
+    Converts bounding box format from [cx, cy, w, h] to [x1, y1, x2, y2]
         :param input_bbox:  input bbox either 2-dimensional (for all boxes of a single image) or 3-dimensional (for
                             boxes of a batch of images)
         :return:            Converted bbox in same dimensions as the original
     """
     need_squeeze = False
     # the input is always processed as a batch. in case it not a batch, it is unsqueezed, process and than squeeze back.
     if input_bbox.dim() < 3:
@@ -230,15 +230,15 @@
     inter = (torch.min(box1[:, None, 2:], box2[:, 2:]) - torch.max(box1[:, None, :2], box2[:, :2])).clamp(0).prod(2)
     return inter / (area1[:, None] + area2 - inter)  # iou = inter / (area1 + area2 - inter)
 
 
 def non_max_suppression(prediction, conf_thres=0.1, iou_thres=0.6, multi_label_per_box: bool = True, with_confidence: bool = False):
     """
     Performs Non-Maximum Suppression (NMS) on inference results
-        :param prediction: raw model prediction
+        :param prediction: raw model prediction. Should be a list of Tensors of shape (cx, cy, w, h, confidence, cls0, cls1, ...)
         :param conf_thres: below the confidence threshold - prediction are discarded
         :param iou_thres: IoU threshold for the nms algorithm
         :param multi_label_per_box: whether to use re-use each box with all possible labels
                                     (instead of the maximum confidence all confidences above threshold
                                     will be sent to NMS); by default is set to True
         :param with_confidence: whether to multiply objectness score with class score.
                                 usually valid for Yolo models only.
@@ -253,15 +253,15 @@
 
         if not pred.shape[0]:  # If none remain process next image
             continue
 
         if with_confidence:
             pred[:, 5:] *= pred[:, 4:5]  # multiply objectness score with class score
 
-        box = convert_xywh_bbox_to_xyxy(pred[:, :4])  # xywh to xyxy
+        box = convert_cxcywh_bbox_to_xyxy(pred[:, :4])  # cxcywh to xyxy
 
         # Detections matrix nx6 (xyxy, conf, cls)
         if multi_label_per_box:  # try for all good confidence classes
             i, j = (pred[:, 5:] > conf_thres).nonzero(as_tuple=False).T
             pred = torch.cat((box[i], pred[i, j + 5, None], j[:, None].float()), 1)
 
         else:  # best class only
@@ -298,15 +298,15 @@
     :return: Detections list with shape (x1, y1, x2, y2, object_conf, class_conf, class)
     """
     # MULTIPLY CONF BY CLASS CONF TO GET COMBINED CONFIDENCE
     class_conf, class_pred = pred[:, :, 5:].max(2)
     pred[:, :, 4] *= class_conf
 
     # BOX (CENTER X, CENTER Y, WIDTH, HEIGHT) TO (X1, Y1, X2, Y2)
-    pred[:, :, :4] = convert_xywh_bbox_to_xyxy(pred[:, :, :4])
+    pred[:, :, :4] = convert_cxcywh_bbox_to_xyxy(pred[:, :, :4])
 
     # DETECTIONS ORDERED AS (x1y1x2y2, obj_conf, class_conf, class_pred)
     pred = torch.cat((pred[:, :, :5], class_pred.unsqueeze(2)), 2)
 
     # SORT DETECTIONS BY DECREASING CONFIDENCE SCORES
     sort_ind = (-pred[:, :, 4]).argsort()
     pred = torch.stack([pred[i, sort_ind[i]] for i in range(pred.shape[0])])[:, 0:max_num_of_detections]
@@ -818,15 +818,15 @@
 
     # inter(N,M) = (rb(N,M,2) - lt(N,M,2)).clamp(0).prod(2)
     inter = (torch.min(det_box[:, None, 2:], crowd_box[:, 2:]) - torch.max(det_box[:, None, :2], crowd_box[:, :2])).clamp(0).prod(2)
     return inter / det_area[:, None]  # crowd_ioa = inter / det_area
 
 
 def compute_detection_matching(
-    output: torch.Tensor,
+    output: List[torch.Tensor],
     targets: torch.Tensor,
     height: int,
     width: int,
     iou_thresholds: torch.Tensor,
     denormalize_targets: bool,
     device: str,
     crowd_targets: Optional[torch.Tensor] = None,
```

## super_gradients/training/utils/distributed_training_utils.py

```diff
@@ -228,15 +228,15 @@
         multi_gpu, num_gpus, device = MultiGPUMode.DISTRIBUTED_DATA_PARALLEL, None, "cuda"
 
     if device is None:
         device = "cuda"
 
     if device == "cuda" and not torch.cuda.is_available():
         logger.warning("CUDA device is not available on your device... Moving to CPU.")
-        device = "cpu"
+        multi_gpu, num_gpus, device = MultiGPUMode.OFF, 0, "cpu"
 
     if device == "cpu":
         setup_cpu(multi_gpu, num_gpus)
     elif device == "cuda":
         setup_gpu(multi_gpu, num_gpus)
     else:
         raise ValueError(f"Only valid values for device are: 'cpu' and 'cuda'. Received: '{device}'")
```

## super_gradients/training/utils/sg_trainer_utils.py

```diff
@@ -445,22 +445,24 @@
     """Get the param names of a given callable (function, class, ...)
     :param obj: Object to inspect
     :return: Param names of that object
     """
     return tuple(inspect.signature(obj).parameters)
 
 
-def log_main_training_params(multi_gpu: MultiGPUMode, num_gpus: int, batch_size: int, batch_accumulate: int, len_train_set: int):
+def log_main_training_params(
+    multi_gpu: MultiGPUMode, num_gpus: int, batch_size: int, batch_accumulate: int, train_dataset_length: int, train_dataloader_len: int
+):
     """Log training parameters"""
     msg = (
         "TRAINING PARAMETERS:\n"
         f"    - Mode:                         {multi_gpu.name if multi_gpu else 'Single GPU'}\n"
         f"    - Number of GPUs:               {num_gpus if 'cuda' in device_config.device  else 0:<10} ({torch.cuda.device_count()} available on the machine)\n"
-        f"    - Dataset size:                 {len_train_set:<10} (len(train_set))\n"
+        f"    - Dataset size:                 {train_dataset_length:<10} (len(train_set))\n"
         f"    - Batch size per GPU:           {batch_size:<10} (batch_size)\n"
         f"    - Batch Accumulate:             {batch_accumulate:<10} (batch_accumulate)\n"
         f"    - Total batch size:             {num_gpus * batch_size:<10} (num_gpus * batch_size)\n"
         f"    - Effective Batch size:         {num_gpus * batch_size * batch_accumulate:<10} (num_gpus * batch_size * batch_accumulate)\n"
-        f"    - Iterations per epoch:         {int(len_train_set / (num_gpus * batch_size)):<10} (len(train_set) / total_batch_size)\n"
-        f"    - Gradient updates per epoch:   {int(len_train_set / (num_gpus * batch_size * batch_accumulate)):<10} (len(train_set) / effective_batch_size)\n"
+        f"    - Iterations per epoch:         {int(train_dataloader_len):<10} (len(train_loader))\n"
+        f"    - Gradient updates per epoch:   {int(train_dataloader_len / batch_accumulate):<10} (len(train_loader) / batch_accumulate)\n"
     )
     logger.info(msg)
```

## super_gradients/training/utils/utils.py

```diff
@@ -1,22 +1,23 @@
+import os
+import tarfile
+import re
 import math
 import time
 from functools import lru_cache
 from pathlib import Path
-from typing import Mapping, Optional, Tuple, Union, List, Dict, Any
+from typing import Mapping, Optional, Tuple, Union, List, Dict, Any, Iterable
 from zipfile import ZipFile
-import os
 from jsonschema import validate
-import tarfile
+from itertools import islice
+
 from PIL import Image, ExifTags
-import re
 import torch
 import torch.nn as nn
 
-
 # These functions changed from torch 1.2 to torch 1.3
 
 import random
 import numpy as np
 from importlib import import_module
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
@@ -522,7 +523,18 @@
     :param default_params: dict, dictionary for the defaults.
     :return: dict, params after manipulation,
     """
     for key, val in default_params.items():
         if key not in params.keys() or params[key] is None:
             params[key] = val
     return params
+
+
+def generate_batch(iterable: Iterable, batch_size: int) -> Iterable:
+    """Batch data into tuples of length n. The last batch may be shorter."""
+    it = iter(iterable)
+    while True:
+        batch = tuple(islice(it, batch_size))
+        if batch:
+            yield batch
+        else:
+            return
```

## super_gradients/training/utils/callbacks/callbacks.py

```diff
@@ -1,28 +1,32 @@
 import copy
 import math
 import os
 import signal
 import time
-from typing import List, Union
+from typing import List, Union, Optional
 
+import csv
 import cv2
 import numpy as np
 import onnx
 import onnxruntime
 import torch
 from deprecate import deprecated
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.plugins.deci_client import DeciClient
 from super_gradients.common.registry.registry import register_lr_scheduler, register_lr_warmup, register_callback
 from super_gradients.common.object_names import LRSchedulers, LRWarmups, Callbacks
 from super_gradients.training.utils.callbacks.base_callbacks import PhaseCallback, PhaseContext, Phase, Callback
 from super_gradients.training.utils.detection_utils import DetectionVisualization, DetectionPostPredictionCallback
 from super_gradients.training.utils.segmentation_utils import BinarySegmentationVisualization
+from super_gradients.common.environment.ddp_utils import multi_process_safe
+from super_gradients.common.environment.checkpoints_dir_utils import get_project_checkpoints_dir_path
+
 
 logger = get_logger(__name__)
 
 
 class ContextSgMethods:
     """
     Class for delegating Trainer's methods, so that only the relevant ones are ("phase wise") are accessible.
@@ -688,14 +692,41 @@
         for transform in context.train_loader.dataset.transforms:
             if hasattr(transform, "close"):
                 transform.close()
         iter(context.train_loader)
         context.criterion.use_l1 = True
 
 
+@register_callback(Callbacks.ROBOFLOW_RESULT_CALLBACK)
+class RoboflowResultCallback(Callback):
+    """Append the training results to a csv file. Be aware that this does not fully overwrite the existing file, just appends."""
+
+    def __init__(self, dataset_name: str, output_path: Optional[str] = None):
+        """
+        :param dataset_name:    Name of the dataset that was used to train the model.
+        :param output_path:     Full path to the output csv file. By default, save at 'checkpoint_dir/results.csv'
+        """
+        self.dataset_name = dataset_name
+        self.output_path = output_path or os.path.join(get_project_checkpoints_dir_path(), "results.csv")
+
+        if self.output_path is None:
+            raise ValueError("Output path must be specified")
+
+        super(RoboflowResultCallback, self).__init__()
+
+    @multi_process_safe
+    def on_training_end(self, context: PhaseContext):
+
+        with open(self.output_path, mode="a", newline="") as csv_file:
+            writer = csv.writer(csv_file)
+
+            mAP = context.metrics_dict["mAP@0.50:0.95"].item()
+            writer.writerow([self.dataset_name, mAP])
+
+
 class TestLRCallback(PhaseCallback):
     """
     Phase callback that collects the learning rates in lr_placeholder at the end of each epoch (used for testing). In
      the case of multiple parameter groups (i.e multiple learning rates) the learning rate is collected from the first
      one. The phase is VALIDATION_EPOCH_END to ensure all lr updates have been performed before calling this callback.
     """
```

## Comparing `super_gradients-3.0.8.dist-info/LICENSE.md` & `super_gradients-3.0.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.0.8.dist-info/METADATA` & `super_gradients-3.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-gradients
-Version: 3.0.8
+Version: 3.0.9
 Summary: SuperGradients
 Home-page: https://deci-ai.github.io/super-gradients/welcome.html
 Author: Deci AI
 Author-email: rnd@deci.ai
 License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre Trained,Models
 Platform: UNKNOWN
@@ -95,15 +95,15 @@
 ```python
 # Load model with pretrained weights
 from super_gradients.training import models
 from super_gradients.common.object_names import Models
 
 model = models.get(Models.YOLOX_S, pretrained_weights="coco")
 ```
-#### All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](https://github.com/Deci-AI/super-gradients/blob/master/documentation/source/model_zoo.md)
+#### All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
 
 #### Classification
 <div align="center">
 <img src="./docs/assets/SG_img/Classification@2xDark.png" width="800px">
 </div>
 
 #### Semantic Segmentation
@@ -156,31 +156,34 @@
 __________________________________________________________________________________________________________
 
 
 ```bash
 pip install super-gradients
 ```
 
-## What's New
+## What's New - Version 3.0.8
 __________________________________________________________________________________________________________
-* 【17/11/2022】 Integration with ClearML
-* 【06/9/2022】 PP-LiteSeg - new pre-trained [checkpoints](http://bit.ly/3EGfKD4) and [recipes](http://bit.ly/3gfLw07) for Cityscapes with SOTA mIoU scores (~1.5% above paper)🎯
-* 【07/08/2022】DDRNet23 -  new pre-trained [checkpoints](http://bit.ly/3EGfKD4) and [recipes](http://bit.ly/3gfLw07) for Cityscapes with SOTA mIoU scores (~1% above paper)🎯
-* 【27/07/2022】YOLOX models (object detection) - recipes and pre-trained checkpoints.
-* 【07/07/2022】SSD Lite MobileNet V2,V1 - Training [recipes](http://bit.ly/3gfLw07) and pre-trained [checkpoints](http://bit.ly/3EGfKD4) on COCO - Tailored for edge devices! 📱
-* 【07/07/2022】 STDC  - new pre-trained [checkpoints](http://bit.ly/3EGfKD4) and [recipes](http://bit.ly/3gfLw07) for Cityscapes with super SOTA mIoU scores (~2.5% above paper)🎯
+*  [QAT&PTQ](https://bit.ly/41hC8uI)
+* [Pose estimation](http://bit.ly/3o0xHq2)
+* [New documentation](http://bit.ly/3KYVCiJ)
+* [New semantic segmentation dataset - Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py)
+*  Lion optimizer
+* PP-YoloE pre-trained - new pre-trained [checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for COCO2017 🎯
+* DDRNet pre-trained segmentation model - new pre-trained [checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for Cityscapes and  [Knowledge distillation recipe for DDRNet](http://bit.ly/3GzZHHo)🎯
+
 
 Check out SG full [release notes](https://github.com/Deci-AI/super-gradients/releases).
 
 ## Coming soon
 __________________________________________________________________________________________________________
-- [ ] PP-Yolo-E implementation
-- [ ] Quantization aware training (QAT)
-- [ ] Tools for faster training 
-- [ ] Integration with more professional tools.
+- [ ] Pre-trained pose estimation model
+- [ ] New predict function on detection models
+- [ ] RoboFlow100 datasets integration 
+- [ ] A new documentation hub
+- [ ] LR finder
 
 
 ## Table of Content
 __________________________________________________________________________________________________________
 <!-- toc -->
 
 - [Getting Started](#getting-started)
@@ -205,15 +208,15 @@
 
 Just make sure that you [setup your dataset](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/Dataset_Setup_Instructions.md) according to the data dir specified in the recipe.
 
 ```bash
 python -m super_gradients.examples.train_from_recipe_example.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
 ```
 ### Quickly Load Pre-Trained Weights for Your Desired Model with SOTA Performance
-Want to try our pre-trained models on your machine? Import SuperGradients, initialize your Trainer, and load your desired architecture and pre-trained weights from our [SOTA model zoo](http://bit.ly/3EGfKD4)
+Want to try our pre-trained models on your machine? Import SuperGradients, initialize your Trainer, and load your desired architecture and pre-trained weights from our [SOTA model zoo](http://bit.ly/41dkt89)
 
 ```python
 # The pretrained_weights argument will load a pre-trained architecture on the provided dataset
 
 import super_gradients
 
 model = models.get("model-name", pretrained_weights="pretrained-model-name")
@@ -313,14 +316,25 @@
  </td>
 </table>
  </br></br>
 
 
 ## Advanced Features
 __________________________________________________________________________________________________________
+### Post Training Quantization and Quantization Aware Training
+Quantization involves representing weights and biases in lower precision, resulting in reduced memory and computational requirements, making it useful for deploying models on devices with limited resources. The process can be done during training, called Quantization aware training, or after training, called post-training quantization. A full tutorial can be found [here](http://bit.ly/41hC8uI).
+  <table class=“tfo-notebook-buttons” align=“left”>
+ <td width=“500”>
+   <a target="_blank" href="http://bit.ly/3KrN6an"><img src="./docs/assets/SG_img/colab_logo.png" /> Post Training Quantization and Quantization Aware Training</a>
+  </td>
+ <td width=“200”>
+<a target="_blank" href="http://bit.ly/3nUGzxb"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
+ </td>
+</table>
+
 ### Knowledge Distillation Training
 Knowledge Distillation is a training technique that uses a large model, teacher model, to improve the performance of a smaller model, the student model.
 Learn more about SuperGradients knowledge distillation training with our pre-trained BEiT base teacher model and Resnet18 student model on CIFAR10 example notebook on Google Colab for an easy to use tutorial using free GPU hardware
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
    <a target="_blank" href="https://bit.ly/3BLA5oR"><img src="./docs/assets/SG_img/colab_logo.png" /> Knowledge Distillation Training</a>
   </td>
@@ -396,14 +410,15 @@
 
 
 Please note that if you work with `torch<1.9.0` (deprecated), you will have to launch your training with either 
 `torch.distributed.launch` or `torchrun`, in which case `nproc_per_node` will overwrite the value  set with `gpu_mode`:
 ```bash
 python -m torch.distributed.launch --nproc_per_node=4 main.py
 ```
+
 ```bash
 torchrun --nproc_per_node=4 main.py
 ```
 
 #### Calling functions on a single node
 
 It is often in DDP training that we want to execute code on the master rank (i.e rank 0).
@@ -605,15 +620,15 @@
 
 </details> 
 
 
 ## Implemented Model Architectures 
 __________________________________________________________________________________________________________
 
-All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/3EGfKD4)
+All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
 
 Detailed list can be found [here](http://bit.ly/3GnJwgZ) 
 
 ### Image Classification
 
 - [DensNet (Densely Connected Convolutional Networks)](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/densenet.py) 
 - [DPN](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/dpn.py) 
@@ -667,14 +682,15 @@
 
 ### Semantic Segmentation 
 
 - [Cityscapes](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py)
 - [Coco](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py) 
 - [PascalVOC 2012 / PascalAUG 2012](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py)
 - [SuperviselyPersons](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py)
+- [Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py)
 
 
 ### Object Detection
 
 - [Coco](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/detection_datasets/coco_detection.py)
 - [PascalVOC 2007 & 2012](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py)
 
@@ -719,26 +735,47 @@
 
 * For a short meeting with us, use this [link](https://calendly.com/ofer-baratz-deci/15min) and choose your preferred time.
 
 ## License
 
 This project is released under the [Apache 2.0 license](LICENSE).
 
+## Citing
+
+### BibTeX
+
+```bibtex
+
+@misc{supergradients,
+  doi = {10.5281/ZENODO.7789328},
+  url = {https://zenodo.org/record/7789328},
+  author = {Aharon,  Shay and {Louis-Dupont} and {Ofri Masad} and Yurkova,  Kate and {Lotem Fridman} and {Lkdci} and Khvedchenya,  Eugene and Rubin,  Ran and Bagrov,  Natan and Tymchenko,  Borys and Keren,  Tomer and Zhilko,  Alexander and {Eran-Deci}},
+  title = {Super-Gradients},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  year = {2021},
+}
+```
+
+### Latest DOI
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7789328.svg)](https://doi.org/10.5281/zenodo.7789328)
 
 
 __________________________________________________________________________________________________________
 
 
 ## Deci Platform
 
 Deci Platform is our end to end platform for building, optimizing and deploying deep learning models to production.
 
 [Request free trial](https://bit.ly/3qO3icq) to enjoy immediate improvement in throughput, latency, memory footprint and model size.
 
-Features:
+Features
+
 - Automatically compile and quantize your models with just a few clicks (TensorRT, OpenVINO).
 - Gain up to 10X improvement in throughput, latency, memory and model size. 
 - Easily benchmark your models’ performance on different hardware and batch sizes.
 - Invite co-workers to collaborate on models and communicate your progress.
 - Deci supports all common frameworks and Hardware, from Intel CPUs to Nvidia's GPUs and Jetsons.
 ֿ
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: super-gradients Version: 3.0.8 Summary:
+Metadata-Version: 2.1 Name: super-gradients Version: 3.0.9 Summary:
 SuperGradients Home-page: https://deci-ai.github.io/super-gradients/
 welcome.html Author: Deci AI Author-email: rnd@deci.ai License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer
 Vision,PyTorch,SOTA,Recipes,Pre Trained,Models Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: torch (<1.14,>=1.9.0) Requires-Dist:
 tqdm (>=4.57.0) Requires-Dist: boto3 (>=1.17.15) Requires-Dist: jsonschema
 (>=3.2.0) Requires-Dist: Deprecated (>=1.2.11) Requires-Dist: opencv-python
@@ -50,17 +50,16 @@
  master/docs/assets/SG_img/Object detection 1500X900.png] [https://github.com/
      Deci-AI/super-gradients/raw/master/docs/assets/SG_img/Classification
                                  1500x900.png]
 ### Ready to deploy pre-trained SOTA models ```python # Load model with
 pretrained weights from super_gradients.training import models from
 super_gradients.common.object_names import Models model = models.get
 (Models.YOLOX_S, pretrained_weights="coco") ``` #### All Computer Vision Models
-- Pretrained Checkpoints can be found in the [Model Zoo](https://github.com/
-Deci-AI/super-gradients/blob/master/documentation/source/model_zoo.md) ####
-Classification
+- Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
+#### Classification
                [./docs/assets/SG_img/Classification@2xDark.png]
 #### Semantic Segmentation
             [./docs/assets/SG_img/Semantic Segmentation@2xDark.png]
 #### Object Detection
               [./docs/assets/SG_img/Object Detection@2xDark.png]
 ### Easy to train SOTA Models Easily load and fine-tune production-ready, pre-
 trained SOTA models that incorporate best practices and validated hyper-
@@ -80,33 +79,31 @@
 Input size is in format of [Batch x Channels x Width x Height] where 640 is the
 standart COCO dataset dimensions model.eval() model.prep_model_for_conversion
 (input_size=[1, 3, 640, 640]) # Create dummy_input # Convert model to onnx
 torch.onnx.export(model, dummy_input, "yolox_s.onnx") ``` More information on
 how to take your model to production can be found in [Getting Started]
 (#getting-started) notebooks ## Quick Installation
 __________________________________________________________________________________________________________
-```bash pip install super-gradients ``` ## What's New
+```bash pip install super-gradients ``` ## What's New - Version 3.0.8
 __________________________________________________________________________________________________________
-* ã17/11/2022ã Integration with ClearML * ã06/9/2022ã PP-LiteSeg - new
-pre-trained [checkpoints](http://bit.ly/3EGfKD4) and [recipes](http://bit.ly/
-3gfLw07) for Cityscapes with SOTA mIoU scores (~1.5% above paper)ð¯ * ã07/
-08/2022ãDDRNet23 - new pre-trained [checkpoints](http://bit.ly/3EGfKD4) and
-[recipes](http://bit.ly/3gfLw07) for Cityscapes with SOTA mIoU scores (~1%
-above paper)ð¯ * ã27/07/2022ãYOLOX models (object detection) - recipes
-and pre-trained checkpoints. * ã07/07/2022ãSSD Lite MobileNet V2,V1 -
-Training [recipes](http://bit.ly/3gfLw07) and pre-trained [checkpoints](http://
-bit.ly/3EGfKD4) on COCO - Tailored for edge devices! ð± * ã07/07/2022ã
-STDC - new pre-trained [checkpoints](http://bit.ly/3EGfKD4) and [recipes](http:
-//bit.ly/3gfLw07) for Cityscapes with super SOTA mIoU scores (~2.5% above
-paper)ð¯ Check out SG full [release notes](https://github.com/Deci-AI/super-
-gradients/releases). ## Coming soon
-__________________________________________________________________________________________________________
-- [ ] PP-Yolo-E implementation - [ ] Quantization aware training (QAT) - [ ]
-Tools for faster training - [ ] Integration with more professional tools. ##
-Table of Content
+* [QAT&PTQ](https://bit.ly/41hC8uI) * [Pose estimation](http://bit.ly/3o0xHq2)
+* [New documentation](http://bit.ly/3KYVCiJ) * [New semantic segmentation
+dataset - Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/
+blob/master/src/super_gradients/training/datasets/segmentation_datasets/
+mapillary_dataset.py) * Lion optimizer * PP-YoloE pre-trained - new pre-trained
+[checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for
+COCO2017 ð¯ * DDRNet pre-trained segmentation model - new pre-trained
+[checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for
+Cityscapes and [Knowledge distillation recipe for DDRNet](http://bit.ly/
+3GzZHHo)ð¯ Check out SG full [release notes](https://github.com/Deci-AI/
+super-gradients/releases). ## Coming soon
+__________________________________________________________________________________________________________
+- [ ] Pre-trained pose estimation model - [ ] New predict function on detection
+models - [ ] RoboFlow100 datasets integration - [ ] A new documentation hub -
+[ ] LR finder ## Table of Content
 __________________________________________________________________________________________________________
 - [Getting Started](#getting-started) - [Advanced Features](#advanced-features)
 - [Installation Methods](#installation-methods) - [Prerequisites]
 (#prerequisites) - [Quick Installation](#quick-installation) - [Implemented
 Model Architectures](#implemented-model-architectures) - [Contributing]
 (#contributing) - [Citation](#citation) - [Community](#community) - [License]
 (#license) - [Deci Platform](#deci-platform)  ## Getting Started
@@ -120,27 +117,34 @@
 to the data dir specified in the recipe. ```bash python -
 m super_gradients.examples.train_from_recipe_example.train_from_recipe --
 config-name=imagenet_regnetY architecture=regnetY800
 dataset_interface.data_dir= ckpt_root_dir= ``` ### Quickly Load Pre-Trained
 Weights for Your Desired Model with SOTA Performance Want to try our pre-
 trained models on your machine? Import SuperGradients, initialize your Trainer,
 and load your desired architecture and pre-trained weights from our [SOTA model
-zoo](http://bit.ly/3EGfKD4) ```python # The pretrained_weights argument will
+zoo](http://bit.ly/41dkt89) ```python # The pretrained_weights argument will
 load a pre-trained architecture on the provided dataset import super_gradients
 model = models.get("model-name", pretrained_weights="pretrained-model-name")
 ``` ### Classification #### Transfer Learning
  ### Semantic Segmentation #### Quick Start
  #### Transfer Learning
  #### How to Connect Custom Dataset
  ### Object Detection #### Transfer Learning
  #### How to Connect Custom Dataset
  ### How to Predict Using Pre-trained Model #### Segmentation, Detection and
 Classification Prediction
  ## Advanced Features
 __________________________________________________________________________________________________________
+### Post Training Quantization and Quantization Aware Training Quantization
+involves representing weights and biases in lower precision, resulting in
+reduced memory and computational requirements, making it useful for deploying
+models on devices with limited resources. The process can be done during
+training, called Quantization aware training, or after training, called post-
+training quantization. A full tutorial can be found [here](http://bit.ly/
+41hC8uI).
 ### Knowledge Distillation Training Knowledge Distillation is a training
 technique that uses a large model, teacher model, to improve the performance of
 a smaller model, the student model. Learn more about SuperGradients knowledge
 distillation training with our pre-trained BEiT base teacher model and Resnet18
 student model on CIFAR10 example notebook on Google Colab for an easy to use
 tutorial using free GPU hardware
  ### Recipes To train a model, it is necessary to configure 4 main components.
@@ -259,15 +263,15 @@
 CuDNN >= 8.1.x - Nvidia Driver with CUDA >= 11.2 support (â¥460.x)  ### Quick
 Installation  Install stable version using PyPi See in [PyPi](https://pypi.org/
 project/super-gradients/) ```bash pip install super-gradients ``` That's it !
 Install using GitHub ```bash pip install git+https://github.com/Deci-AI/super-
 gradients.git@stable ```  ## Implemented Model Architectures
 __________________________________________________________________________________________________________
 All Computer Vision Models - Pretrained Checkpoints can be found in the [Model
-Zoo](http://bit.ly/3EGfKD4) Detailed list can be found [here](http://bit.ly/
+Zoo](http://bit.ly/41dkt89) Detailed list can be found [here](http://bit.ly/
 3GnJwgZ) ### Image Classification - [DensNet (Densely Connected Convolutional
 Networks)](https://github.com/Deci-AI/super-gradients/blob/master/src/
 super_gradients/training/models/classification_models/densenet.py) - [DPN]
 (https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/
 training/models/classification_models/dpn.py) - [EfficientNet](https://
 github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/
 models/classification_models/efficientnet.py) - [LeNet](https://github.com/
@@ -332,20 +336,22 @@
 super_gradients/training/datasets/segmentation_datasets/
 cityscape_segmentation.py) - [Coco](https://github.com/Deci-AI/super-gradients/
 blob/master/src/super_gradients/training/datasets/segmentation_datasets/
 coco_segmentation.py) - [PascalVOC 2012 / PascalAUG 2012](https://github.com/
 Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/
 segmentation_datasets/pascal_voc_segmentation.py) - [SuperviselyPersons](https:
 //github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/
-datasets/segmentation_datasets/supervisely_persons_segmentation.py) ### Object
-Detection - [Coco](https://github.com/Deci-AI/super-gradients/blob/master/src/
-super_gradients/training/datasets/detection_datasets/coco_detection.py) -
-[PascalVOC 2007 & 2012](https://github.com/Deci-AI/super-gradients/blob/master/
-src/super_gradients/training/datasets/detection_datasets/
-pascal_voc_detection.py)
+datasets/segmentation_datasets/supervisely_persons_segmentation.py) -
+[Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/blob/
+master/src/super_gradients/training/datasets/segmentation_datasets/
+mapillary_dataset.py) ### Object Detection - [Coco](https://github.com/Deci-AI/
+super-gradients/blob/master/src/super_gradients/training/datasets/
+detection_datasets/coco_detection.py) - [PascalVOC 2007 & 2012](https://
+github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/
+datasets/detection_datasets/pascal_voc_detection.py)
 __________________________________________________________________________________________________________
 ## Documentation Check SuperGradients [Docs](https://deci-ai.github.io/super-
 gradients/welcome.html) for full documentation, user guide, and examples. ##
 Contributing To learn about making a contribution to SuperGradients, please see
 our [Contribution page](CONTRIBUTING.md). Our awesome contributors: [https://
 contrib.rocks/image?repo=Deci-AI/super-gradients]
 Made with [contrib.rocks](https://contrib.rocks). ## Citation If you are using
@@ -358,19 +364,27 @@
 Slack]( https://join.slack.com/t/supergradients-comm52/shared_invite/zt-
 10vz6o1ia-b_0W5jEPEnuHXm087K~t8Q) * To report a bug, [file an issue](https://
 github.com/Deci-AI/super-gradients/issues) on GitHub. * Join the [SG
 Newsletter](https://www.supergradients.com/#Newsletter) for staying up to date
 with new features and models, important announcements, and upcoming events. *
 For a short meeting with us, use this [link](https://calendly.com/ofer-baratz-
 deci/15min) and choose your preferred time. ## License This project is released
-under the [Apache 2.0 license](LICENSE).
+under the [Apache 2.0 license](LICENSE). ## Citing ### BibTeX ```bibtex @misc
+{supergradients, doi = {10.5281/ZENODO.7789328}, url = {https://zenodo.org/
+record/7789328}, author = {Aharon, Shay and {Louis-Dupont} and {Ofri Masad} and
+Yurkova, Kate and {Lotem Fridman} and {Lkdci} and Khvedchenya, Eugene and
+Rubin, Ran and Bagrov, Natan and Tymchenko, Borys and Keren, Tomer and Zhilko,
+Alexander and {Eran-Deci}}, title = {Super-Gradients}, publisher = {GitHub},
+journal = {GitHub repository}, year = {2021}, } ``` ### Latest DOI [![DOI]
+(https://zenodo.org/badge/DOI/10.5281/zenodo.7789328.svg)](https://doi.org/
+10.5281/zenodo.7789328)
 __________________________________________________________________________________________________________
 ## Deci Platform Deci Platform is our end to end platform for building,
 optimizing and deploying deep learning models to production. [Request free
 trial](https://bit.ly/3qO3icq) to enjoy immediate improvement in throughput,
-latency, memory footprint and model size. Features: - Automatically compile and
+latency, memory footprint and model size. Features - Automatically compile and
 quantize your models with just a few clicks (TensorRT, OpenVINO). - Gain up to
 10X improvement in throughput, latency, memory and model size. - Easily
 benchmark your modelsâ performance on different hardware and batch sizes. -
 Invite co-workers to collaborate on models and communicate your progress. -
 Deci supports all common frameworks and Hardware, from Intel CPUs to Nvidia's
 GPUs and Jetsons. Ö¿ Request free trial [here](https://bit.ly/3qO3icq)
```

## Comparing `super_gradients-3.0.8.dist-info/RECORD` & `super_gradients-3.0.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-super_gradients/__init__.py,sha256=cmI1LVgXkRW2WRp4rPHTdgZK0bs-qxnMvey1jiTGpXI,932
+super_gradients/__init__.py,sha256=e1PEJK3EaBHt27KXTY-kVQSBCVhq6e41ifYtuDk2SeE,932
 super_gradients/requirements.pro.txt,sha256=N4SNm12LMYBhOwA5ShEQlihV_6nJoveWkbEo1037idI,44
 super_gradients/requirements.txt,sha256=-hJEsVtZGOENWHmv4jiAUp-doNLwlJ_Ld4uhVULJf-U,729
 super_gradients/train_from_recipe.py,sha256=597R7Zw0-cyQA5fcuTr6r6HynEiEQnoe3ZLVXxQOkfI,654
 super_gradients/common/__init__.py,sha256=1F7pRDWoGs7wMWpbBw3iaTPWpeegxOroNPqUO3nzEMw,1098
-super_gradients/common/object_names.py,sha256=sB2BAdg4I0PBJly9yGImISBodDwZv-vYXogNMafscsI,14327
+super_gradients/common/object_names.py,sha256=Upy33h3UfnvHsfdPStzcd_txUnCmymhGziN3vcFXZSc,15140
 super_gradients/common/abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/abstractions/abstract_logger.py,sha256=MpEjg7PihMZb_qLBKC-R58wWFqNJdPJMlOkxEU25hCU,879
 super_gradients/common/abstractions/mute_processes.py,sha256=JxC3ofVySoiL7U7x9QYhzWLVYArkgqKQB2Kp3HyPOyE,3129
 super_gradients/common/auto_logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/auto_logging/auto_logger.py,sha256=qH84FkmTe50L7Mg8kDjTKVHVxCsCi4DQTMV2V53jARU,4687
 super_gradients/common/auto_logging/console_logging.py,sha256=PEPSfHQ8incS13dkM9gzlWBeRdwbodo9qVqRSk32s_E,6625
 super_gradients/common/aws_connection/__init__.py,sha256=cZCFSeQHk8E6TTZHTjnAhezGATF5iSKiFR2dBof8vqg,142
@@ -42,15 +42,15 @@
 super_gradients/common/environment/__init__.py,sha256=ljbYwQPDh8G0dCHjA6EGPSX5guFcsj-tUB6Ks0mHR-A,202
 super_gradients/common/environment/argparse_utils.py,sha256=c-XT11eDEZ42bWu2eKr4e6i30SF-OlM0a8xxgD08ob4,993
 super_gradients/common/environment/cfg_utils.py,sha256=_jUmcZ6HG7NK2R0H7edjNM62rDNzCTeRXBdAH2FFbq4,9170
 super_gradients/common/environment/checkpoints_dir_utils.py,sha256=UMQbSQ8tuZzYfTmwrqNef3KHElbZ3DC69B2L_hbGqNw,4218
 super_gradients/common/environment/ddp_utils.py,sha256=JMEzTKSrQ5pG9MGLd0xaIGIlg4Rlexh4soXhi0r6nzY,2682
 super_gradients/common/environment/device_utils.py,sha256=wV1pK5rjB4IShktrVdo9vx5mg_tF4XHIrRFssl2ftZA,752
 super_gradients/common/environment/env_variables.py,sha256=OxUpZ6aDt16d3rHPfw9u6wn-cmvdV4Zp67FIVc6n01c,1147
-super_gradients/common/environment/omegaconf_utils.py,sha256=iEdJ0dygWdbSwcMs4vyg_tBrOgbfivQ3-GsTxspw9eo,1550
+super_gradients/common/environment/omegaconf_utils.py,sha256=4Pb6xm4LAqwiqyX_VhfIsnvCVtjI8ThLY5MhfyQzvu0,1768
 super_gradients/common/environment/path_utils.py,sha256=p6fBTLBdxdpsALaD0lanM2jEtZcbSdthuEXSoOmgT5Q,459
 super_gradients/common/environment/monitoring/__init__.py,sha256=QmJWRpVWwHOK0qjNPV6PlA5ZzKjgumxNbSoYDnhUzzo,112
 super_gradients/common/environment/monitoring/cpu.py,sha256=eGHnEDbci_jku-RTzgROxt_kPy9bUdydk_bUMin3Kxc,153
 super_gradients/common/environment/monitoring/data_models.py,sha256=t3Hky9Iu-qLKATdzyqb76j_6QxEVxamC7gnjh7Te5xk,2517
 super_gradients/common/environment/monitoring/disk.py,sha256=2XI7426eWGk_z3O_Fy_LWoVwUkLdK7ee7D8rqE6lmWE,1025
 super_gradients/common/environment/monitoring/monitoring.py,sha256=7c2anfycW-cHauTphi-ZaRH6CYVuEPLsGCbLz7BjHSQ,5427
 super_gradients/common/environment/monitoring/network.py,sha256=kfse7NZsOErzvkYmHKRbCP4g5hVW0ZNyZ0GbRTjtrw4,948
@@ -72,23 +72,24 @@
 super_gradients/common/factories/datasets_factory.py,sha256=x9kvJ072Pv-Bq-6ELhuE64KvpGpoQqKOG_0c_ammKto,237
 super_gradients/common/factories/detection_modules_factory.py,sha256=50m8-hqKMxmJW8FiMT0kPunAgPjHJA2AyNtD1SJ2B84,1014
 super_gradients/common/factories/list_factory.py,sha256=n6THqmLOuHTEkpFTCEfUHmG1VyKZ5xibDCLhpYsmvos,572
 super_gradients/common/factories/losses_factory.py,sha256=X0wM4QzKOszDVSUGLOgC01MALnREZFy12EKh3Jqc_yw,223
 super_gradients/common/factories/metrics_factory.py,sha256=yV5D5iHgcj2Q-a632zymQF7NnCwvOiYMVJnlbPQBslo,226
 super_gradients/common/factories/optimizers_type_factory.py,sha256=tIad1d-uYmT1glByXT-JXTkZpEygyk2zdb4ihiP7qVk,467
 super_gradients/common/factories/pre_launch_callbacks_factory.py,sha256=qjd2jvcn95jRNcmJRBa0IWnGSkxNPJf-Xn66j-4H6MY,271
+super_gradients/common/factories/processing_factory.py,sha256=t-IEuzn6SxR7gDLQQ_WMp8-zPiq7UCjlDuONTnplWpk,623
 super_gradients/common/factories/samplers_factory.py,sha256=pdsa9My_0aF63vBgHLQtzobw8-ykz-dFbDemMizJrdI,229
 super_gradients/common/factories/target_generator_factory.py,sha256=LZXQUxMI-jz_QPj0Bfi9FccLgX3Ky2MjU1llqxHFvOE,263
 super_gradients/common/factories/transforms_factory.py,sha256=TrwGexN9y33eAw0wQRFDgM5a26FKhCOzQvyC-fp2kfM,1873
 super_gradients/common/factories/type_factory.py,sha256=HwIiWskEfoHZiEkN8batqIxATs_20TJqq8qR9W0_Has,2377
 super_gradients/common/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/plugins/deci_client.py,sha256=CP0H4tvynauOmLOWmPLjTvu3ho-Cugu8gLhofFY08HA,10974
 super_gradients/common/registry/__init__.py,sha256=gYkyLBFQN2kIgt0YFzGJl7lXKyOHBHE67B-1_C_JS8I,271
 super_gradients/common/registry/albumentation.py,sha256=MU7ZkXX-qSM5A_2l2apl6njJECwuUn4U1bo22yovOIY,1231
-super_gradients/common/registry/registry.py,sha256=51E0lUjiR5oNQfNgGpoXVQLwUCDQ2uBSGY8YuJmAnTg,5918
+super_gradients/common/registry/registry.py,sha256=XNgmvUY3kV3oF7i-yz4aZqyoM42EG4cV_mwS1EIyNFw,6006
 super_gradients/common/registry/registry_utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/sg_loggers/__init__.py,sha256=yMh5um_t_0FsWFMDF3Gi2ncf-s-g8HcicBMw-VSTxY4,409
 super_gradients/common/sg_loggers/abstract_sg_logger.py,sha256=OoGxOvQXwDfycg4A9wt_jgxI1zTS5XIS8GPFBQmY5rM,7355
 super_gradients/common/sg_loggers/base_sg_logger.py,sha256=W5IBmftH8M9b85t-F-mWsnRIo34_6CQ_vQd9owslUN8,14980
 super_gradients/common/sg_loggers/clearml_sg_logger.py,sha256=BWAJzubNT974xgcsOVckRsU8KLsYW2NLJ5x65tCeQ6w,10055
 super_gradients/common/sg_loggers/deci_platform_sg_logger.py,sha256=XLanzH_CwW4Nw6Mx-m4tS6rFkDH3xZ9P8rCIyYIxoGs,6618
 super_gradients/common/sg_loggers/wandb_sg_logger.py,sha256=DnGC3OmBcMSpK_wQ00KW0e7SLsgZ9vhDbhNhJYHRAtE,13073
@@ -133,14 +134,16 @@
 super_gradients/examples/train_from_recipe_example/train_from_recipe.py,sha256=l-PwJ3GKaKcnYIbTVdVL811-diMyYdcoY4HxoO9jb60,627
 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py,sha256=wRiGIkRqoD3HRTQt4hBxWMp97EQrF50aqT1Jct_Wtrk,1334
 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py,sha256=fJscmGOW90V-4x3MshgVcfrez7_XThZnOoec6W2J-QM,1643
 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/train_from_recipe_with_user_objects/train.py,sha256=MX3SCfca8NLmiiHv7iO1GUKA8fgy5fCLk6tN93kH8vY,1326
 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py,sha256=vX_3SS6ZVmUVbBA62L7tx6FamPnPN66PRoh8NNeXw-Y,2548
+super_gradients/module_interfaces/__init__.py,sha256=T2XfJNfNnFl5cuqk3picDTlOevEErG_6fUKyrjoTRFE,118
+super_gradients/module_interfaces/module_interfaces.py,sha256=VV-G11F_mcG29TzjUcpbuMUDq6yv-XVjn6ClClap_W4,958
 super_gradients/modules/__init__.py,sha256=TsT-xloLimGBxiwiVkqeX5YVesJq2zCacDxGl_RghwU,2589
 super_gradients/modules/all_detection_modules.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/modules/anti_alias.py,sha256=Qi4RW9_TuuJMtNV2sHfHfp0BLMMA0BgeTZcn9k6pXz4,617
 super_gradients/modules/conv_bn_act_block.py,sha256=jsV1AV-HcdErb8PV4ZG63CtumfJrpI7Xjw4DhY7KnOU,2073
 super_gradients/modules/conv_bn_relu_block.py,sha256=pZ0OazMsoP7PxjV6-ltgR8IytjsF6tsC71GH4kRgEgE,1976
 super_gradients/modules/detection_modules.py,sha256=F8qgnSt-yAEk2i1xFimdCNc6PpvSo47AWczPyGlQEso,15129
 super_gradients/modules/multi_output_modules.py,sha256=YLofR05Z56k4iHM460KRO-GQ4jMcP1MrrrgT-aOcew4,4362
@@ -158,14 +161,15 @@
 super_gradients/recipes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/recipes/cifar10_resnet.yaml,sha256=M4RO1pDcd27U2NbPvJCWXQJiIbaUTAJGoh7RBSZYBbc,1516
 super_gradients/recipes/cityscapes_ddrnet.yaml,sha256=aacRQxOIDMUJl97XtBFutzGz1r-8qI78BXB2wlMionI,3856
 super_gradients/recipes/cityscapes_kd_base.yaml,sha256=6Py8Oc2VnxzIvDyZJWA7nRugMmgrBQ_xvB9C2rEyXvQ,4072
 super_gradients/recipes/cityscapes_pplite_seg50.yaml,sha256=Nfx-C6nJYcLVm7TLDPk1C2nPljY0lseW1yLWIyliXOI,3615
 super_gradients/recipes/cityscapes_pplite_seg75.yaml,sha256=l0Oyy3qSLPSutlwyjlwJtWGSBxSVt1R8-OG0fPCEYVA,3514
 super_gradients/recipes/cityscapes_regseg48.yaml,sha256=rbcNThYt8YqWbnjT69H0g-JfU-MYVyswny7McAMIh0c,2771
+super_gradients/recipes/cityscapes_segformer.yaml,sha256=7G29cYeKoIOFP0mUDmyV5XR8-gYul9Br8vNqAL-UWF4,4293
 super_gradients/recipes/cityscapes_stdc_base.yaml,sha256=4HtapSi082EfOsufJTToCFu-dPLoE3UGeN6j1UeUWcI,852
 super_gradients/recipes/cityscapes_stdc_seg50.yaml,sha256=DyLzvIRUwemcq2e1ZrVDEcRTILZ2X-PwgOaXgjXLk2E,3175
 super_gradients/recipes/cityscapes_stdc_seg75.yaml,sha256=i1IREG_2l_PQHWs_HgoG4ylSLV6mzHgY2BxdMlGbbLs,3369
 super_gradients/recipes/coco2017_pose_ddrnet39.yaml,sha256=HmQhrTODv7zMI_9qbmL42UBskAGKUQFQGheI0QGse5Q,2063
 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml,sha256=wn1oRekmwMfclrg3wtqFbUPD28iah_GeS1SsupiKaTU,3821
 super_gradients/recipes/coco2017_pose_pppose_l.yaml,sha256=8cmmkZ-t-P8Tgv3-ZlbnvSCcy3mEcfDEm8AoEBycDsQ,2231
 super_gradients/recipes/coco2017_ppyoloe_l.yaml,sha256=-syEeGFn4GZS9h78I8-uBvHA_ryC9dhtrQt3qdgwnfU,2388
@@ -182,14 +186,16 @@
 super_gradients/recipes/imagenet_mobilenetv3_small.yaml,sha256=d5MyAZJHe_EOcHDfIH25MOzsL163Sfqhj_XUEoP6BJI,992
 super_gradients/recipes/imagenet_regnetY.yaml,sha256=RXCCk8__OR891tRH2UdeZ9qCLTCPLG7nNM6W7zXPZYI,2387
 super_gradients/recipes/imagenet_repvgg.yaml,sha256=ghGo2YoP5VzmW7fw9ouLKK1VkYmM4KcOD0EfWpcd-iU,1519
 super_gradients/recipes/imagenet_resnet50.yaml,sha256=xB7uBvqcLujZ5j4ZNbgEgSM7I5LjM7ahaE1jz_I7hh8,1442
 super_gradients/recipes/imagenet_resnet50_kd.yaml,sha256=-Hz22cJysjIJmOjyOB6dK5rklXQXFoKxlfS4V4qmiUY,2998
 super_gradients/recipes/imagenet_vit_base.yaml,sha256=V4xwcPI_1uDQDqIraN5TQZMMSQB5q_VeoVaXrHGLCqU,1409
 super_gradients/recipes/imagenet_vit_large.yaml,sha256=l_MkDxYYWmjN6a1Rs6LwYMAWfUj2yxfPYlOjGrbtP9w,1283
+super_gradients/recipes/roboflow_ppyoloe.yaml,sha256=gJMGuCgFU7UeARh8iE5YSadZmmO2Hh0_I90ZvXSRbh0,2226
+super_gradients/recipes/roboflow_yolox.yaml,sha256=igSc1HUa6plUIRTQg46mz4nfr0mFxHfzQ3B6415MvdA,2134
 super_gradients/recipes/supervisely_unet.yaml,sha256=GwBvE2vvOmdgpLr1bka3_83jQCi2ug8rzyjINKhYUr0,1520
 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml,sha256=0qDPTZn_TfM5uFBpw5HawJ947223y8oBqH6wU96XRRc,1906
 super_gradients/recipes/user_recipe_mnist_example.yaml,sha256=RZ_Ja8ZKACL1xgoredVAd3LG33KJDJhTVfJyfELY_E4,2367
 super_gradients/recipes/anchors/ssd_anchors.yaml,sha256=iRsfDXt3bWyCvmZtOQK-Y2maAJEgfgXVWF5sos6r7RU,2222
 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml,sha256=dEn_jgEn_NA80xaugB6lY1mdRRjVcOTwnckMlVmdbXE,563
 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml,sha256=jQfnMGb1kcprnr6UnUbmYaNwslEn728j-8Ci5NpX63E,104
 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml,sha256=An9tm3_3uLY6veIA23sp9SoZDapgVZ-q2hH9XgdUThw,103
@@ -229,33 +235,34 @@
 super_gradients/recipes/arch_params/unet_arch_params.yaml,sha256=U-7HSXzOXXr2-d6xQjNJF-8oD1KLhD1WqqaThI0atUk,1369
 super_gradients/recipes/arch_params/unet_default_arch_params.yaml,sha256=w8lhI0_oNU4wpBs3qcKf79yW2G1i8XLeFl9MT7Qrkno,3014
 super_gradients/recipes/arch_params/vit_base_arch_params.yaml,sha256=Y6skbVr98NRSf5Ts4c47JPwsDMudqygFu5W4ZQiXkLo,63
 super_gradients/recipes/arch_params/yolo_arch_params.yaml,sha256=GroGr-T0l_puiM3nPIT3Y_RzuwhNrv3U5s4g5y1Pijo,2393
 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml,sha256=lmtcOUvHlhQf9anw1ybaks25GETvHu2QpH2D9jJqEUg,235
 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml,sha256=atByNWwQqnpaZ7SXEW2Q5cKo0T99V447xLhh1NoShFs,237
 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml,sha256=1yJcwDkZwKlL_6MeWjyypFtsPyyC9CdNWquRG7gQoXI,237
-super_gradients/recipes/arch_params/yolox_s_arch_params.yaml,sha256=6O9HaTbY4U1DHRMoJmmwjR7MltYT1bDBYW9-vS6CstU,236
+super_gradients/recipes/arch_params/yolox_s_arch_params.yaml,sha256=J2qgjwp6VxRcNsRomCyZtdV5Ht3RruMZmYJagtlzttU,237
 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml,sha256=rxYvMOUeT5jnGhZ9-OTZ4ohHgheLDdHyNJ4_-m6JSQU,229
 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml,sha256=Wsg5AnPiqHZTnbTLFGUr90eS5a45F9ko0dfT8XTZbPQ,228
 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml,sha256=XpQsqckADGZgsZHxW6bc0vF971bRz0kpyuP_1dH6aRI,611
 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml,sha256=VYKzkX1jD8sB9NH9rLHc2KFCPx83Zn9c8SptLYSDjpM,72
 super_gradients/recipes/conversion_params/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml,sha256=GEM_wvMaJqERXYOkKgz2G0vUUpzo3NV_DuARpkBYkww,1807
 super_gradients/recipes/conversion_params/default_conversion_params.yaml,sha256=u2CB5clR_aud10_nDsoqGinb2W1dJK-_8w46BbMFkhg,2040
 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml,sha256=fg_lvX7KrY8XEuUwfC2PP2vcfXLmX2YTdu7twh4fzjI,869
 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml,sha256=t3w9oe7aIUSBNhQWnPClAtFs77m8QCijbO4qKGpnr08,1530
 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml,sha256=Uz3J9LB42eM6n08Dz7m9BG5VIWM2lnPrXy2eOySa6gs,1056
 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml,sha256=1NjXHAMg_znj2v-UHR57daxXpzLPvN3ZIMLKwsH5Zso,615
 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml,sha256=HUr8IaV0IIfuxK-fibY42yKUHe04kUCBFnYAE5E3rGI,525
 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml,sha256=CKSennwvRG1a-swVvL1he18vdtNRnCStH3LFhruGSnQ,706
 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml,sha256=dtbvoxt9IR9cBaslNOWCcsX7s_gjHRnWK5Ayl1ElzmI,644
+super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml,sha256=i7l9LXea216Y2RB8e3FxhlGNBR_a1tLJKCg2Ix8JsTI,721
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml,sha256=WK7UH73r-nuHMKepBVyykR0tf306s-P5NgQNGI-dZWk,709
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml,sha256=wBHhYk6Q6kdmLDk9tTi0vpREr0fhTz4r1Zh0ybrRPGw,708
 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml,sha256=x8wk7EC6eKGlxSyaBTxKGJidss5BbgX1MTG9KLCnU0M,3946
-super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml,sha256=8HvRub3MwZ1mer247KALAQ5musvSdn7ansLWzvA7Pt8,3662
+super_gradients/recipes/dataset_params/coco_detection_deci_yolo_dataset_params.yaml,sha256=S7uKClewyJSp-NJn7oOWfM583KpfpRwSNYod_pz2Fcs,3661
 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml,sha256=GeCdBxnGf5WqQ165WIVCg4jz4vmjqT2LzofdvXB6bAs,4202
 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml,sha256=PqQ6fBINO3sHHAAGx4rHKz4PAURkd67qPrVLWu1WM5Y,3590
 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml,sha256=qHBh-kCmrXr5ICR0Ww_C1B2RywSEOz4nVSZSt96K-aU,2461
 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml,sha256=q8s65W76DEu9XWRY_gR9fyr5Xp5HH1vLh8eG9ZvR7fA,405
 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml,sha256=SC_nc2CyZqQ7R-z4pcqoTyZlBZB7JlmT_5hzgMjHCRc,1466
 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml,sha256=9JnbyZjCkZ3ZdMHj0CwVkQdzi7QBevwmoK1KQlxlymU,931
 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml,sha256=CILfhTGk4ne0wk0L7gbD95EjBTKGGTR8UjCaTW79Joc,732
@@ -265,16 +272,17 @@
 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml,sha256=SiPRDxzkwoOMDtKqzM7p0c5M658dQNEMQRvFH24K3aA,1059
 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml,sha256=C5-HGDjjDbnDWy43zM5byBmZicVqey-YQdoTkqKA7nw,1093
 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml,sha256=YvXeTTMlK8hEOu6HoedazdFtkk81icNHBg81yNGKmSw,845
 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml,sha256=mgexC2b4s-uabJsT2v51GdifhDg67WZfnexTMo-_NTY,1762
 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml,sha256=KzOrZe-NRkZ3XGkixGkUTA6Pd9aO2fTtnIhpaQOdIvU,149
 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml,sha256=exEzH6LsS7KdvC975vG7TiA5byADG4YSfLUpCss58uI,1571
 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml,sha256=eIHwt4ZsVYKtpQbNSk1ZbsdneEZ6twlZkpxVG9LLt84,1414
+super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml,sha256=M6x8EzF8yDIKZ8ifPX11OmA_DAtbIQLimKxaRZRZ8R0,3398
 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml,sha256=GshRG6Jqdb1S9uoBjWbckkSajIPo6Avuf46WXFMcC5w,961
-super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml,sha256=saGXz2S1dSTqhdYzN7B_KalMO8JT9qp54FeretqtytY,558
+super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml,sha256=4_4HkNjzZDKFHpgSV1-S0s9rRrZJUj5S-7zUk1wOFaY,559
 super_gradients/recipes/quantization_params/default_quantization_params.yaml,sha256=OVewy7FMpSUpheoL7_eAzbJVpcfy5O2eIwpEri0tUc8,1155
 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml,sha256=jZV1VVe3Lda96Mq-hb8zHfR3EATHt0kSGLOpcdxssFg,591
 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml,sha256=NUOLRusDJ9H6Nxp-NGVsie7tPuRXKE493jwzI_U8rqE,700
 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml,sha256=vh7Ej8ViU6qH7B87femqWgoxkE2WYxYhTFNsR-8JzK0,877
 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml,sha256=Ah9iuCKngV2Bri_R0PPB-p5SB0oPpVYGs38yG83X-kU,1302
 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml,sha256=vuTXdVTzwM52w1n44mGBB-kJKluXtmxymgmbdLg85Jw,723
 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml,sha256=hMDTZejrlTXQxuSJPXyW6jdxTrd5De5IoilzpP-Fmis,956
@@ -291,47 +299,52 @@
 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml,sha256=NoLNnoAVy7-P7IJAymyPY7sjhiNuy973WHttv_Hh8eI,519
 super_gradients/sanity_check/__init__.py,sha256=IrTB1Lxw15cKFjxV8bGraUxj5d_pmEqYk7FHa01nuvk,107
 super_gradients/sanity_check/env_sanity_check.py,sha256=2_55JKDSsL1krMuXrWbF_qpz3Ob5SHP8lTYvSO5Ie-Q,5262
 super_gradients/training/__init__.py,sha256=LaqXsoTNBBFvGcV14K7tjt0iMbQdEy5NINJEycpcrPw,666
 super_gradients/training/params.py,sha256=I62jGc85o5YZeQDfvv9uUDyDKFeUnwXpR_i5rSZ2aZs,4155
 super_gradients/training/pretrained_models.py,sha256=fbXHJRWmx_7azXkOUXNgDEORdsaVQ6jjp0jYfkO_dbU,5696
 super_gradients/training/dataloaders/__init__.py,sha256=tlQw2GmkFPEMK3FA-_eODb1LHhDVKbl12BL6G1GEMak,3228
-super_gradients/training/dataloaders/dataloaders.py,sha256=HqNKgNT5z_H4oCLyI5MoJ8B9coS0lWZqn0wt8mPJC9g,29718
-super_gradients/training/datasets/__init__.py,sha256=MTX9-ZQ2zAJasXpqXF5_UfzY8Di1CC8f9PrdGAJTRY0,1714
+super_gradients/training/dataloaders/dataloaders.py,sha256=uMi6Ld8nVj-sxPFsWeJuAIzqnhNGW9gpPFvhmmtQR5M,31443
+super_gradients/training/datasets/__init__.py,sha256=nptSnL6f7srktNihvAqw5polrwp4K-IrhTWPQ9vFLEM,1811
 super_gradients/training/datasets/auto_augment.py,sha256=VHw-Wq4ecHSKcqe9l63RUGpNa6JygUP3N7B6hbnTPxg,14162
 super_gradients/training/datasets/data_augmentation.py,sha256=TJOIT7j6ZWaNW6E4VvkJ-ARIWBY7Y4210NqrZbzKJJ8,3705
 super_gradients/training/datasets/datasets_conf.py,sha256=U2FTTYwCFp3cFZkzliWSGCHuCUUrns57AX7uS5Wn5NY,3484
 super_gradients/training/datasets/datasets_utils.py,sha256=oZnyLGBkfibkczYP2t69xf2OtqPU8ixyWDlc3iXQJh0,30279
 super_gradients/training/datasets/mixup.py,sha256=WDHoqTFbq-PGemKxE0eZ10Q03mpH8GIj-vFBNIZEg1U,14663
 super_gradients/training/datasets/sg_dataset.py,sha256=xVqf-7vvGk96TkshGHIcqiQfIVXdOCs12U1fcJjWrX0,11746
 super_gradients/training/datasets/classification_datasets/__init__.py,sha256=LcdaPeIQxwDM_qRb-sEwVswsjSveuZcdndpZKusGGsQ,252
 super_gradients/training/datasets/classification_datasets/cifar.py,sha256=lH_iBhC2igE_KQEJb_Lc1FpKvs4QsnuCxzOTIE0qNUw,3096
 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py,sha256=idY9fSwXxrgqJt9lJOaLFsQS0hz5qX6BIbXHBW_TIrU,1706
-super_gradients/training/datasets/data_formats/__init__.py,sha256=x4QXVQX7qZ6IVwPHr9QIuxnPdex53mSEVIRZ9iFOfhk,363
+super_gradients/training/datasets/data_formats/__init__.py,sha256=V2Sioujv6egladjkcsgceQ-goRUpja2Ey0ma-DDihWc,862
 super_gradients/training/datasets/data_formats/default_formats.py,sha256=GbP2UWXISbkfKtP7rjV2Qag3Q5BrlwU_RDzdM8DJuDk,3927
 super_gradients/training/datasets/data_formats/format_converter.py,sha256=yMJj-9REVJ_T-JkPB34IJsQzpxWOhhnlxxRNRhMUSqU,3071
 super_gradients/training/datasets/data_formats/formats.py,sha256=Aa3odNETBnS5_ZC3TcKOevqr89gw_qWZKZpS9Gb_wPo,7928
 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py,sha256=p9pa3hZA3tzVf7xCWqnTRlKr03i4NjxIbUic_IHt7U8,1044
 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py,sha256=ID3k0HeqcWUWBqyFMvyKkiAtY44u-3q5lSe6m0EprZE,2674
 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py,sha256=V1-2q4ULIIyc2XO1e3MENu0XbOcR9riVh2L9t0XvdMo,5094
 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py,sha256=OzZJc6ZUMcJXiVeEulmAAVYt67yznNRPik0NE6bMESM,2089
 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py,sha256=NaVEMg1EEC71ZK509wyts-rHND6DYnSlqxc2wRk6t7E,2043
 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py,sha256=a8BhAyUPCLuFbLTkE1uU0rOwQxRzOUaRVSU0GzAwSL8,5043
 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py,sha256=VhtZmqnW1cxeo1azP-zPNcMYMPCzc4ZBBokkFWioqPw,2948
 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py,sha256=nCCohobPvCOtQ_SF2BAyyVyuSV68ZjjxrUurGfwNXMs,575
 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py,sha256=LChhVCXQ9-d9Zp3sa_PzAOrUBa15f_QKtxHdW51ocwg,1792
 super_gradients/training/datasets/data_formats/output_adapters/__init__.py,sha256=n7aH5WQzk_awjpei_GY-yOktBTw7LtzekY-gHJ8_AKE,92
-super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py,sha256=q9kCSFV0sbbhLBeUUhCnFSan7rGcVYaKk4isjZIAQx4,8384
-super_gradients/training/datasets/detection_datasets/__init__.py,sha256=a7CrY5YAoh7tOR1lEPngk6dUyXHwoJG0-Y5xFhHqqPc,399
-super_gradients/training/datasets/detection_datasets/coco_detection.py,sha256=_PzaJIa7KPRD88dvqIFb8ecut85rmfOOC89WEmwtXEY,2511
-super_gradients/training/datasets/detection_datasets/coco_format_detection.py,sha256=qXdOyW3kPfE7UPJpXRmfNmgkYvVb8P791ucU2xBhIoU,8762
-super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=X4PqiWaDo1mUeSROXROsgZfhNRirhFsodx6ScpTopvk,24762
+super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py,sha256=qH0LPewt8hvKE5jVaZl0HunzONd7UHErbBcCuK_rjZk,8373
+super_gradients/training/datasets/detection_datasets/__init__.py,sha256=g86eRhqJoDs-9snO7QR6zejTmqhF2Amq71O-ZZQLPZc,683
+super_gradients/training/datasets/detection_datasets/coco_detection.py,sha256=EUTVRS0igoBFeUDhXg_tqxJSDhGUEU45jdL8YYko2ng,2505
+super_gradients/training/datasets/detection_datasets/coco_format_detection.py,sha256=OJ0JEQLClxRgdMZlUpuVEH0jxRqwfTbhOZnHK4rzjuY,9258
+super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=7J4vM6N5MIsmWf9gFx3G0Kn1rHWCdbwAlYA_HsBilD8,25694
 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py,sha256=pAtuVBRVO_Y0Q-diaHQz3tWyjW7U3xR04ohzPx-vkbo,11353
+super_gradients/training/datasets/detection_datasets/yolo_format_detection.py,sha256=Z96cYyHxzpYO3m5OQNNehU3iixtm60Wc11cZWkkpQs4,10390
+super_gradients/training/datasets/detection_datasets/roboflow/__init__.py,sha256=Kw_KF41iHBr9tHrg6I6T6gdy8fgKLlG0NLCtXOyNpEs,328
+super_gradients/training/datasets/detection_datasets/roboflow/metadata.py,sha256=PTwZuphA1HyeYtxDnio6kmbcV6aM8VPD0AM4gk3_JCU,18882
+super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py,sha256=9UEctKh8WxBLxdRP8wqfg3KDFq_KDYTr5AX4qD2Om7I,3504
+super_gradients/training/datasets/detection_datasets/roboflow/utils.py,sha256=_7mtuGnTHUVqfUqWlC9zpKGutBdaYJCGGj9pSbItfxI,1997
 super_gradients/training/datasets/pose_estimation_datasets/__init__.py,sha256=BeCVpXLn0FV9Oo_8iWtHz9n1GxdhXqTzymGT97_bdCA,502
-super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=gV-KX0OfzbC4ARg6XHo0Y26ZIWbdDic98cLiYgVSviY,4899
+super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=6xNszBrqqOOdIKgM2ZFOZ4Crwssfh096_AcLZL5R1q4,4910
 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=aADh3OLNLBLCk-3_nxLHjrrHniqr-tfbIHjKzJf-REA,9066
 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py,sha256=uMq0vV22npZqz21L_preyhbyKSHiBqS14Mp2UuEb-_4,5929
 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py,sha256=McVUG3sWR9Lxgk_ca8ECqvYieQwZApsFRfLNABES51Q,10167
 super_gradients/training/datasets/samplers/__init__.py,sha256=bsLNxxZ61qQx2DbmGzsfd_6jDo4UYPkYNswoTOQtjrE,385
 super_gradients/training/datasets/samplers/infinite_sampler.py,sha256=VPqUXdOAsPAwuozPQ19rweHkT-RYlq9BMLlNWt8Zofw,2516
 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py,sha256=dnYh_2wWCFPlWVwnEhUEwhAaRpJGIGtoIbNiXSRAfq4,4809
 super_gradients/training/datasets/segmentation_datasets/__init__.py,sha256=5zkvFQ4Av5Ceydrnkq9jS19xp9axFBF7M-41K6DXBFU,1037
@@ -353,15 +366,15 @@
 super_gradients/training/losses/__init__.py,sha256=FQs7jZgVyXfS26m4P__S47ybTUAfJuQq3ep0CdEJBlk,1476
 super_gradients/training/losses/all_losses.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/losses/bce_dice_loss.py,sha256=uBqTiQDgBCzd62lcZN_fLEmPOyuCbh9r6BYLlFiCPns,1219
 super_gradients/training/losses/bce_loss.py,sha256=F7oXzO08RJVjVfglKszaJ3j3CaqO2T6tVaSBdCgUFpw,419
 super_gradients/training/losses/cwd_loss.py,sha256=1jO8qdoGd9NKdZbWvc-2hAuN5Cn9U8Vk-3rIQt2bGj4,2374
 super_gradients/training/losses/ddrnet_loss.py,sha256=tfSfllVAW9HoPq0W3vbFEH3taznQR1WCpwaXKo33XLg,2525
 super_gradients/training/losses/dekr_loss.py,sha256=SBDKparvpTGysGkWUY0346aN-IJAag_EiVgIlrF2GBQ,3377
-super_gradients/training/losses/dice_ce_edge_loss.py,sha256=lFSR09dLRlovVYT3FSkjzmjFccXDeP3_lKnaxWEhKXE,5646
+super_gradients/training/losses/dice_ce_edge_loss.py,sha256=1TM7s822Ik4IkKT27U4VCd8lVwoy3ClemCFpktxgx04,5618
 super_gradients/training/losses/dice_loss.py,sha256=hcVfl6Jrf0SKTDUf8dEWD15np99XU_I9yv9rR7G142I,5208
 super_gradients/training/losses/focal_loss.py,sha256=-mrmypTdwa5XcSCas-4Hk2wsc_oIaJjvhqY6FHyJ0Go,1214
 super_gradients/training/losses/iou_loss.py,sha256=ON_fJAatqVH4_XVNCrSd9gLNkYlPLEhizUPaJ9jwvT8,5051
 super_gradients/training/losses/kd_losses.py,sha256=-CGP7dWa1B-Ni2MnCQQLARRWxg5ajIUay81xQag-ZUI,2176
 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py,sha256=74uR2HNtiC7h59ywLCjb1NL_3DPtLuNHx3fcxHXGLcs,4177
 super_gradients/training/losses/loss_utils.py,sha256=E23MWbrXOsyF-DexK-tnCB2XyMajI0LHhtPXX9t1FT0,550
 super_gradients/training/losses/mask_loss.py,sha256=Co9_ugt0A3422AJX8PgYdVgcbt-BRAFFhN_tDkenPnE,3854
@@ -379,24 +392,26 @@
 super_gradients/training/metrics/all_metrics.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/metrics/classification_metrics.py,sha256=Zopby8WBumdoJxZLJv5YgL7W_ZQODN4hKs55UJKO_H0,3262
 super_gradients/training/metrics/detection_metrics.py,sha256=XXneeuIzFCMwQfiGQcZZCN9cWhD6v3Cj_25HJTZ93nE,10741
 super_gradients/training/metrics/metric_utils.py,sha256=WT1TmuARbVKDLhw4Z1rJt38JM6jnSLAqO6gJa8rKWWY,3973
 super_gradients/training/metrics/pose_estimation_metrics.py,sha256=rw2gFnRSe1tET_TD4rdvt-8DWAvfSoAZwTaT5FZY_og,15346
 super_gradients/training/metrics/pose_estimation_utils.py,sha256=aOv42gu29NiWLihv6kmDBoFBXf0heVUsICF75dmM0l4,11454
 super_gradients/training/metrics/segmentation_metrics.py,sha256=B24ivTj53cF2COHeyDutxGohDLYcFT_eiKEqXpjDMXk,11935
-super_gradients/training/models/__init__.py,sha256=1JQTy52TidlNkPgoB6Grhi6k79pYlfh5D4pKNKIT87s,8103
+super_gradients/training/models/__init__.py,sha256=XZlJndgVtaqOjpv_3Gns6ixTdvmCn-FwhibEra8RICE,8368
 super_gradients/training/models/arch_params_factory.py,sha256=ufy6mCMPUm1b9s3wm-AVMIbX2irytPoZpeXELgtCROs,1226
 super_gradients/training/models/conversion.py,sha256=kucMPr5HGUVn_xL06BaQU7vXzcgvUaqjZF5jiGgupqE,7060
-super_gradients/training/models/model_factory.py,sha256=Q8XZeU25hQGA13qXx4IbCpgaCZcwFYQmLxmWWXMX7ew,11273
+super_gradients/training/models/model_factory.py,sha256=z2vsf1_zjK2wgWYimHxRxA-bpOHG3ZQx2bC1o0Nhz6s,11875
+super_gradients/training/models/prediction_results.py,sha256=KB0vc3zhL_-is3LN4eeMqwoEtyvjlwFJ4msvv-OM6-8,10850
+super_gradients/training/models/predictions.py,sha256=-i4fUfLThPPTpSPiyFj-3TS_MRQWwXwQm5QZG1GD754,2054
 super_gradients/training/models/sg_module.py,sha256=JalNA0oIrW5IqV6Fl-SkAaq1qmcdLcAS8jx9QC84zMk,2998
 super_gradients/training/models/classification_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/classification_models/beit.py,sha256=kAq50cBeBteSF3uE3SW4TwYqfVn6edxPNXQEvOXc1Xg,20025
 super_gradients/training/models/classification_models/densenet.py,sha256=kDFzSB95Zk9OES501IiAyZmUlOnT03M3BEDaxlFONjM,7472
-super_gradients/training/models/classification_models/dpn.py,sha256=gKqXPQi5-GbqSmGrLUTCmHRK9teBpkXY4zFI99D7nO8,3678
-super_gradients/training/models/classification_models/efficientnet.py,sha256=J7wjsHVwZqFKFHNluR048O8PSrjgm9C7Q0FYi5twTfk,29281
+super_gradients/training/models/classification_models/dpn.py,sha256=B5wPjPhPGp2PhTRxbC3w4VheCqVVs_8s9swqtwWnNKQ,3707
+super_gradients/training/models/classification_models/efficientnet.py,sha256=t9Rc9DveDC99iin-Xsv6UQ_Oy43SMOx3WjykTziqRgA,36745
 super_gradients/training/models/classification_models/googlenet.py,sha256=H57hvNMY7fqOV4v7Ezre-QVvawD1U9wuyAKUmpC1A4o,8862
 super_gradients/training/models/classification_models/lenet.py,sha256=uCaZPPVyfwyLfmD1KfoXiw05PvH-Ue4oa9Zczb_dHmg,798
 super_gradients/training/models/classification_models/mobilenet.py,sha256=JuABaCD_b6_Sh1EzigrBKqOniTTnI9RQ-a1V_YGaS6g,2407
 super_gradients/training/models/classification_models/mobilenetv2.py,sha256=V8FF_9Ibrn9LCf_4ybvQVKr5wVs1LEhpbXOff_XE0pY,9472
 super_gradients/training/models/classification_models/mobilenetv3.py,sha256=2aVzTJOufcdqthtSbjVHE7ViT3iaZcvvwTE9l-GiiKA,8696
 super_gradients/training/models/classification_models/pnasnet.py,sha256=DAo76uXefiCtOUTJ8uiuwAKSDN0nasSSOsCHg-sCkP0,4339
 super_gradients/training/models/classification_models/preact_resnet.py,sha256=24X4Zz00jj3Tj_l3BlLZOl-Z-dLJQ17mf7WKcpYcMtw,4209
@@ -408,96 +423,107 @@
 super_gradients/training/models/classification_models/shufflenet.py,sha256=-57ZOa75ul4eEUMi3fnNbEff2AJGCXJaXQ9npLzETa4,3660
 super_gradients/training/models/classification_models/shufflenetv2.py,sha256=hHMYew6ET-QV8bYhwyCfCoXwIGn1uAJjSyQ9F6EJ9Kw,9768
 super_gradients/training/models/classification_models/vgg.py,sha256=byU29VjwL79efNtIC_ETLXhBLSe8qn_4Wm2RJ4BQYlo,1538
 super_gradients/training/models/classification_models/vit.py,sha256=NwtBiuhcO8dFTXwRb7h66phGDyrQuztdAM_nO5--1UA,9210
 super_gradients/training/models/detection_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/detection_models/csp_darknet53.py,sha256=mn3ndQ4JDVsMM_N1q6wI8fnEYu3JnaX1RWDNJqm-GaM,9502
 super_gradients/training/models/detection_models/csp_resnet.py,sha256=OVL-DXEWj7e5B873jujeKxYvhs7Nhy6ViXOcLDHr49E,9814
-super_gradients/training/models/detection_models/customizable_detector.py,sha256=-1HzS5RifoU-rvw6xLRAnSsf9myXzMUQxQwGMvyA1xo,3782
+super_gradients/training/models/detection_models/customizable_detector.py,sha256=E02Mx-8ehqZwV6GTnJ-uBgWMQGNBN_lW1gC6b-no0k4,8784
 super_gradients/training/models/detection_models/darknet53.py,sha256=FBFqJjU01A1l94HW7u7gCBmnRhSUvRVjlXZCsqyR4X8,4746
-super_gradients/training/models/detection_models/ssd.py,sha256=7pPGW2AftzfrH6YHdeThzHVWA0KV_FD0Y1LHcTWdvTs,1438
-super_gradients/training/models/detection_models/yolo_base.py,sha256=s-v_6QfzkCQboU9qXD-m1p1IWiAQvAykCTCDeBMEgLw,24897
+super_gradients/training/models/detection_models/ssd.py,sha256=wvl6t3ltL6y5tjwqiFzBl8KmkwBOyUh07VS_7yVDfjs,2315
+super_gradients/training/models/detection_models/yolo_base.py,sha256=gLF2ohfGLVA6x_a5b2CI8GPZNgcp-SHk7I1XUb-khBI,29459
 super_gradients/training/models/detection_models/yolox.py,sha256=Wjz2H7NwX3j_YkUzLWMSmcDbnEqee59dCXLrd4jRJ-Q,2459
 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py,sha256=kKdYZ8QRFvcXymQyiO30nRuf--sHEt1uncYowhNT6Kg,155
 super_gradients/training/models/detection_models/pp_yolo_e/pan.py,sha256=WJmWjmTzqNBlf0kmznhduaAGmNaTrxns6-1qro0KKaY,6984
 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py,sha256=D4V9FAX5_VoxoPcwbuvYDtxaTfPRxFfvM5Ds0frO6js,3487
-super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=eXR6icU69NEVytxOdfkh2SMSyIVkuuOnmT6lHNqXoUk,3725
+super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=bZkjWOiKH3MXtEW3bnVFPa68LzX2LOZHQEQRGPyGBhw,8240
 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py,sha256=dMdGGlREeqFBOB5J3FmOnHad7cs6N5zKhOt-Hz15NV0,12334
 super_gradients/training/models/kd_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/models/kd_modules/kd_module.py,sha256=VRkHiGg-fkD3vB1JQkonjIXH338h2aqBr75kHe2jfhg,3170
+super_gradients/training/models/kd_modules/kd_module.py,sha256=urOyHbsubq615UiGJo4-CAFpKvdKxHLrTFMzp1TlM5c,3553
 super_gradients/training/models/pose_estimation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py,sha256=1WeqAspQseBaECT42iGbKnVfFJ2hHPx-63eublI_dgQ,21231
-super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py,sha256=SXPgL4GcP4lgi7qCsneVbElCTOZrCI4ieB3dR7upih0,892
-super_gradients/training/models/pose_estimation_models/pose_ppyolo.py,sha256=Or1tXbidF59tBcQDYCeKDXN90RrSfl0S4BM4774IQH0,891
+super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py,sha256=vQUuvQO6JDdW4tNKYL7k_iDfRf1h28j7aj-n_Xr0UPo,1294
+super_gradients/training/models/pose_estimation_models/pose_ppyolo.py,sha256=pLLHoTF_V2rJKmJ0gLQmcQC0wt7TSfb9RrFA4VoYSaU,1335
 super_gradients/training/models/segmentation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/segmentation_models/common.py,sha256=58mVuAE3Hds_5f_5hr3a-ovHzYoGMslKBlwQRhl_5dY,964
 super_gradients/training/models/segmentation_models/context_modules.py,sha256=CcUiqpDPW2iyBuzzcpFGEYu50slxXenRrKdPVJ-zhTo,5139
 super_gradients/training/models/segmentation_models/ddrnet.py,sha256=ta4b4urUI0zazPNYUKk3p6Rf1sb61H87XSveJPccAa0,27896
 super_gradients/training/models/segmentation_models/ddrnet_backbones.py,sha256=tLHTnh590-QIg_Jyw87uLgGPt_yM2djx9pqilaAG7hk,2439
 super_gradients/training/models/segmentation_models/laddernet.py,sha256=aQAwG7h_AinfT6r-LvYqdzkWDzcKV0YqzQMNbRcOMmU,21760
 super_gradients/training/models/segmentation_models/ppliteseg.py,sha256=tuwPCaE8CyDU4OX0SqZyJ4B8JD377rOBC7Tgr8F20Qk,15648
 super_gradients/training/models/segmentation_models/regseg.py,sha256=V-Vc4zZcoigUlFD8-p4K9_p-BLuhYWmrPyZX8di8_QI,14424
+super_gradients/training/models/segmentation_models/segformer.py,sha256=hNSunP6CtOcwxczuwQRQxY1sZdc0R1OnxatCW2aHBPA,20334
 super_gradients/training/models/segmentation_models/segmentation_module.py,sha256=ypc_zQRfeuP6YEoY3Kc-tcRRVLLuOaY0uJuWpQRTzKo,2256
 super_gradients/training/models/segmentation_models/shelfnet.py,sha256=bcSLs0d1ulhjWUbgAtdmG6hR_vN4IXMXCkwK0r2Dp98,24833
 super_gradients/training/models/segmentation_models/stdc.py,sha256=m2oXqSvRV-lM8Rl_51ebP_6xcQt0pX8imkL59nzJp6A,29005
 super_gradients/training/models/segmentation_models/unet/__init__.py,sha256=WZp8BByl8QZpdPlnLwvW7QF5qfODj_-yo4UbtoScPng,260
 super_gradients/training/models/segmentation_models/unet/unet.py,sha256=x5Zu2Z7rw6i4LXyxcyxfL2uOzt3DuofWo7uKX_utTCw,12324
 super_gradients/training/models/segmentation_models/unet/unet_decoder.py,sha256=PdmnBOjv8MrreWEEphMJsMqS3MuxeNDqvRf0ls-uqvY,8305
 super_gradients/training/models/segmentation_models/unet/unet_encoder.py,sha256=auTtUn6jkKWUOdW_wKvOyKC9DpVSi7Y-LjoZY1POA3g,13292
 super_gradients/training/models/user_models/__init__.py,sha256=WNfXGheDVebPB3XmC9ce-wkyh0qXHRlINW43JIdnY6E,119
+super_gradients/training/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/training/pipelines/pipelines.py,sha256=ML0ylHisBvP9wwhg33NoEw8U8N4ZADDQZ_bYZF5E3Lo,14399
 super_gradients/training/pre_launch_callbacks/__init__.py,sha256=SZtn0Kq5PJ_GIMfFT5bBb0Pck6r5mAnBAfgpDaX5Cdk,393
 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=E3UsNalAFR0-7pwga-OjFCTp4m7SuO9BEy04Lwt18kk,13955
+super_gradients/training/processing/__init__.py,sha256=L_S3KapcujiBTXjHcMZxQz5aCwJM9Xxurbhs08oy0_o,517
+super_gradients/training/processing/processing.py,sha256=Z-CvRtbGgEYtvT9N6S3-8NfOwSetFTZkCk1DzrdIRZc,13178
 super_gradients/training/qat_trainer/__init__.py,sha256=GZRdCf6P1Ximp-eoVw8kHv5Zb4AjBqxV0E2NwO1OmNo,98
 super_gradients/training/qat_trainer/qat_trainer.py,sha256=PY3-7_vEJN8mgVIsD17K1qZ-DT6PETe7KuvoN2tFnls,9896
 super_gradients/training/sg_trainer/__init__.py,sha256=dug-p1erLN2SzYFQytJzPWDLOCmfvE94kFtcFLOTqj0,184
-super_gradients/training/sg_trainer/sg_trainer.py,sha256=-5EPB9yHks3BFlXRPNkZ2Eo8MEf01pDCTDurVGVtpQQ,95882
+super_gradients/training/sg_trainer/sg_trainer.py,sha256=9Nk2wyMgrEAMGEcgkjONQms3_WHcEN8Hudbf54I9Ro8,97370
 super_gradients/training/training_hyperparams/__init__.py,sha256=R5pvZNSQgDNxRp23qAlAAhGdPT7u_e78QiztqQDqosc,1685
 super_gradients/training/training_hyperparams/training_hyperparams.py,sha256=pZIOz9L6vf-tgCMUbvf2WLch1zCCfDevhfYPnL3QR7A,3774
 super_gradients/training/transforms/__init__.py,sha256=SMLfPEp8zqooiV6mB4byOzk5SprUUo77LIUNgTTB7A8,1024
 super_gradients/training/transforms/all_transforms.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/transforms/keypoint_transforms.py,sha256=-lTR8tHtWGmK6THZvyI52OpH5yhWXDGJeUJM_FwcZhE,16193
 super_gradients/training/transforms/pipeline_adaptors.py,sha256=ukVHjcx-XaCEGZ3I_afIb9Uj73vwYtkmgrLJw9jr7oU,1134
-super_gradients/training/transforms/transforms.py,sha256=wSXiEnKjfYeYs0HmAuo7xVsGppGxYkyV1LAwluaWKxc,57465
+super_gradients/training/transforms/transforms.py,sha256=OcqekeLDMA7_TUrtuo_wJG6XrUCwaEJ9qty2Ouxu0bk,55085
+super_gradients/training/transforms/utils.py,sha256=WkgT9-2hZm7IBS_HZzy1kOE0EOb-k0t8gypuPhpC5Z4,6048
 super_gradients/training/utils/__init__.py,sha256=hveHoDSb03rQ0jXc0SLWD7Pvwd9gCnaISEgc_oikTOE,1104
 super_gradients/training/utils/activations_utils.py,sha256=LNgR7SUWOehjBbvtHvU8PtgazsbxX9ztvIUNAQ4nB64,1673
 super_gradients/training/utils/bbox_utils.py,sha256=tvDIJ5TkShshteJAzXVtQZaZFMtIHrYS98U5bpcc0sU,1111
-super_gradients/training/utils/checkpoint_utils.py,sha256=e9Bj3euX8dgi0uwKPa1v4Pd8VdnOEe5FZ7Znqt_DK-s,13875
+super_gradients/training/utils/checkpoint_utils.py,sha256=jqphMTl_izp2nW41Fu9gj7iMVxVBZwyvgLxfnEju4vg,14834
 super_gradients/training/utils/config_utils.py,sha256=jDS_SaRfIEvAXzPB5ZerzVtKaDxD8mgKesUI4M2ERdo,9794
 super_gradients/training/utils/deprecated_utils.py,sha256=YtKScFu62sn2IDBtzC2cPmdSFQ_UfeQZ3CrPDuOZpO4,1132
-super_gradients/training/utils/detection_utils.py,sha256=MY___279AIpnmfolIkBPg4Sk7A-eAEqiUoS6Egz1C70,53513
-super_gradients/training/utils/distributed_training_utils.py,sha256=p5Ch2wEsQo1Ke98CCtQpLs2N5aokYtoe_mb8hfau9B8,16153
+super_gradients/training/utils/detection_utils.py,sha256=EzzS372c8jPTOcOY50R5b7giRKkypXNFXcU9cBCbeTk,53611
+super_gradients/training/utils/distributed_training_utils.py,sha256=1hUkc_OE3CCvBtcWlUsGbB8kmgjAUWtgXFJs9QORX-I,16195
 super_gradients/training/utils/early_stopping.py,sha256=FGv-bFT6N1WrtEmZ2Q0xmmijmOI_IKoTvxQcua0LK9g,6352
 super_gradients/training/utils/ema.py,sha256=xPjihYYtpKqrOth0KoRyTeFarCTEH-AVnh0J9M767PM,9322
 super_gradients/training/utils/ema_decay_schedules.py,sha256=lV9zLoVvfPPWJajPpNBnkn8d5ahLJIAjHtv3rZsDU1E,2610
 super_gradients/training/utils/export_utils.py,sha256=Ci9yz8OiK0oVEBHaG74-YuPqBANciWpFf17w-IVYvRc,1072
 super_gradients/training/utils/get_model_stats.py,sha256=nMKVdVxsLPSKDXD7qnTWk60f0B3F1-Ct-XdZchFbsJM,7508
 super_gradients/training/utils/kd_trainer_utils.py,sha256=j-RWPU7_0rKX-4Cf9RiyGk3GuH6j7_cGeBLKYhuXYOk,771
+super_gradients/training/utils/load_image.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/optimizer_utils.py,sha256=tB-M7Iv9SqRMyzTpk_5tL1gNTk7tpeVPRyEhI_5tqY0,5827
 super_gradients/training/utils/regularization_utils.py,sha256=apNkV4g-9-mA0m6aSGVz6M5Y6MisplfmcdkYwDnFIyA,839
 super_gradients/training/utils/segmentation_utils.py,sha256=otlxMRGq63cNsSj39lTQtNLyDvM9UrU7LVPlHHYxbRI,10388
-super_gradients/training/utils/sg_trainer_utils.py,sha256=mBufIcveWskIYA1ITH__SdFMIma_zkg2jin8qeqmWME,19633
+super_gradients/training/utils/sg_trainer_utils.py,sha256=wnH6njXa_0eENF9QpznsYi81lfUrOLzbBqaOVAbSd50,19625
 super_gradients/training/utils/ssd_utils.py,sha256=n31g0sdpHM96PWJGrJlXK5EGMb0t1nRgAE5sI17XXM4,6272
-super_gradients/training/utils/utils.py,sha256=dw4hmxAGX2PipS_W5SfjKDkfkMQ_OyWiKtP6Vsvlsy8,17925
+super_gradients/training/utils/utils.py,sha256=EWcR6vxmbKJNAVLrO4hpJhhaZHvquDdEX7gEHKCepcw,18273
 super_gradients/training/utils/version_utils.py,sha256=lzIg-vB-ok6tF2HfzFNkIEpq1XB3_cVqoaaNikGR1PE,303
 super_gradients/training/utils/weight_averaging_utils.py,sha256=a9rw30CWTfp-QCDysObSC-yd-W_XQYJeX12SfvyH8TQ,6209
 super_gradients/training/utils/callbacks/__init__.py,sha256=IW4hEmiLvmSqcvYMQn6D0e8qcI-avUnHUcMI8Mv9gvg,2030
 super_gradients/training/utils/callbacks/all_callbacks.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/callbacks/base_callbacks.py,sha256=pCMNK9iUQm8jqSAm5elZrG9Oy3AYD62L-_qj8e9du8U,20126
-super_gradients/training/utils/callbacks/callbacks.py,sha256=nw2B3FXAm7j--W2UBfkEb-Sd_OqA8Z9KHmNkWIViVIM,31285
+super_gradients/training/utils/callbacks/callbacks.py,sha256=UCHS-mkHzEqqoORL2OiVa23Zab1inMLfytJnnioOkkE,32630
 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py,sha256=7-EaXO3ipczQw9H6NIGqZ-3cR3n-ZN6oAEcnCsv-VtE,1169
+super_gradients/training/utils/media/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+super_gradients/training/utils/media/image.py,sha256=F47OIx3s23gJDxujpHOd0Vw_YpN_aJj-abUeraFyA9M,5775
+super_gradients/training/utils/media/stream.py,sha256=wgVafnzRXnZvSxaiquNXUC6PqSMlLI4A6YS6_b4A04Y,4046
+super_gradients/training/utils/media/video.py,sha256=XnoV6dnd6--iNT4JhT0e671DlQIfnN03nO7TrBBfkgQ,5360
 super_gradients/training/utils/optimizers/__init__.py,sha256=Z-kZTiqwHe-KFYP0BTFsX0TNms8-CfRrc6iKEfewopM,396
 super_gradients/training/utils/optimizers/lamb.py,sha256=zdvmfKHGen7_rwMohoEs6DOSDEH95ELFCKezD1fN1v0,9760
 super_gradients/training/utils/optimizers/lion.py,sha256=ivMkwLg0vpOyfD4h226wScYXYDwTdCh0o_zkOeyrdcs,3008
 super_gradients/training/utils/optimizers/rmsprop_tf.py,sha256=5gzx0uy3x4c8G8UgfDnOTLjASwT1enBAcfUkgzrOOJU,6834
 super_gradients/training/utils/pose_estimation/__init__.py,sha256=V0xjHNxc1OeJUE2QOTlAV298wmQwgRWwXLx5Pq6p5Gw,213
 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py,sha256=1y-85e33A9mKokm4ER_HpwuRqWpbY2pjm6gAjjy4WXc,11167
 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py,sha256=HEdNaksgnzoXh1RWRvB5rd_tniZWkk6Ro-6D2-Abv1Q,7140
 super_gradients/training/utils/quantization/__init__.py,sha256=FsLDGZR4MT_1tTIcnyOhIqUTfCf178tU7Y72och-Fws,387
 super_gradients/training/utils/quantization/calibrator.py,sha256=vfXnyPxLdHjk5e5CF3-lBwofRDjX-ZCyDaRreuu6_h4,6271
 super_gradients/training/utils/quantization/core.py,sha256=CYykLasziH9YT0h_utxWj6WZ6tXi4KUSKaiBf1N2YZM,8417
 super_gradients/training/utils/quantization/export.py,sha256=GW22x2GMQJMEp1iZcJ63qcxev6Etay_FI6taKbJpmv8,2196
 super_gradients/training/utils/quantization/selective_quantization_utils.py,sha256=hQ8uZliyAK21pguj0aSybxINffXrj0R2YCHCWIRV7Z4,17062
-super_gradients-3.0.8.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
-super_gradients-3.0.8.dist-info/METADATA,sha256=RJeABHhHQMlGNMmjTBmC-8WsMPSH-uag_iaNr3y2oDI,32749
-super_gradients-3.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-super_gradients-3.0.8.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
-super_gradients-3.0.8.dist-info/RECORD,,
+super_gradients-3.0.9.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
+super_gradients-3.0.9.dist-info/METADATA,sha256=qEEElq7wG2GUcVgeJE1foQ9XbaK5E-F9j4AzZimz3ug,34221
+super_gradients-3.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+super_gradients-3.0.9.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
+super_gradients-3.0.9.dist-info/RECORD,,
```

