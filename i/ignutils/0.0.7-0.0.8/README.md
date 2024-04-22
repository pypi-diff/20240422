# Comparing `tmp/ignutils-0.0.7.tar.gz` & `tmp/ignutils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignutils-0.0.7.tar", last modified: Wed Apr 17 13:31:37 2024, max compression
+gzip compressed data, was "ignutils-0.0.8.tar", last modified: Mon Apr 22 09:27:58 2024, max compression
```

## Comparing `ignutils-0.0.7.tar` & `ignutils-0.0.8.tar`

### file list

```diff
@@ -1,124 +1,132 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.374993 ignutils-0.0.7/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-12 14:41:07.000000 ignutils-0.0.7/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1291 2024-04-17 13:31:37.374993 ignutils-0.0.7/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3893 2024-04-17 13:31:28.000000 ignutils-0.0.7/README.md
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      753 2024-04-17 13:31:28.000000 ignutils-0.0.7/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      303 2024-04-17 12:21:27.000000 ignutils-0.0.7/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-17 13:31:37.374993 ignutils-0.0.7/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.306993 ignutils-0.0.7/src/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.334993 ignutils-0.0.7/src/ignutils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3649 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    45289 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/active_augmentation.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4159 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/algo_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.342993 ignutils-0.0.7/src/ignutils/autoui_utils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3885 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/autogui_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    20681 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/autotest_recplayback.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2484 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/autoui_utils/calculator_demo.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.346993 ignutils-0.0.7/src/ignutils/calib_utils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1412 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/angle_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6380 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/charuco_mono_calib.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16504 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/charuco_stereo_calib.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14815 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/infer_depth.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5981 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_calib.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3770 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_dump.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6312 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_error_calc.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3647 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/mono_undistort.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    44010 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/optimize_depth.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7902 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/point_depth_demo.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10569 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/pose_estimate.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7728 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/rs_crop_dump.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10662 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_3d_error_calc.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14560 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_calib.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4941 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_dump.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10057 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_error_calc.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5667 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/calib_utils/stereo_record.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.346993 ignutils-0.0.7/src/ignutils/cam_utils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      871 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5755 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/camera_reader.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1676 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/gopro_reader.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6950 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/cam_utils/realsense_reader.py
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    12744 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/clone_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5347 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/config_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37875 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/contour_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4201 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/docker_utils.py
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)     9782 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/draw_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14237 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/file_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1094 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/filter_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8726 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/fisheye_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4775 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/geom_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5746 2024-04-17 13:31:28.000000 ignutils-0.0.7/src/ignutils/gpu_utils.py
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    24667 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/img_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3061 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/json_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1663 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/keyboard_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5654 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/labelme_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10540 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/license_check.py
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    20812 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/mouse_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2094 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/multi_process_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.350993 ignutils-0.0.7/src/ignutils/o3d_utils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1196 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/plot_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3372 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/read_rosbag.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8528 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/o3d_utils/registration_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.350993 ignutils-0.0.7/src/ignutils/registration/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      916 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4521 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/ecc_register.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    18564 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/keypoint_register.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1825 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/register_abstract.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1257 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/register_wrapper.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8253 2024-04-17 06:11:12.000000 ignutils-0.0.7/src/ignutils/registration/superglue_register.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.366993 ignutils-0.0.7/src/ignutils/selenium/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1254 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/selenium/selenium_test.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12894 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/show_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5265 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/ssh_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/stitch_det_track/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      812 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6126 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/extract_gps_data.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8250 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/register_seq.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5518 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/stitch.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    45952 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/stitch_det_track_seq.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2891 2024-04-17 12:21:27.000000 ignutils-0.0.7/src/ignutils/stitch_det_track/unique_identifier.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3232 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/system_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      993 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/timer_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19564 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/transform_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5449 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/transfrom_crops.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1756 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/typehint_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/video_utils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      826 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2887 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/dump_frames.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2596 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/exif_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3740 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/folder_reader.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3275 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/play_video.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12810 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/video_reader.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8329 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/video_sync.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4369 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/video_utils/video_writer.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.306993 ignutils-0.0.7/src/ignutils/vo/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/vo/mono_vo/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3882 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/Visualization.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1964 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/feature_det.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2983 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/feature_track.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6374 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/find_match.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6074 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/main.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22917 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/mono_VO.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2181 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/optimizer.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      684 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/mono_vo/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.370993 ignutils-0.0.7/src/ignutils/vo/stereo_vo/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5071 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/stereo_vo/data_handler.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    23487 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/vo/stereo_vo/stereo_vo.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.374993 ignutils-0.0.7/src/ignutils/workflow/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      107 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      812 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/__main__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8004 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/filter_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6494 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/keras_seg_mlnode.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    17255 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/mlnode.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    25301 2024-04-17 11:53:25.000000 ignutils-0.0.7/src/ignutils/workflow/node_config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4818 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/node_utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5086 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/seg_mlnode.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12781 2024-04-17 09:28:21.000000 ignutils-0.0.7/src/ignutils/workflow/workflow_main.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3435 2024-04-16 12:04:09.000000 ignutils-0.0.7/src/ignutils/yaml_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-17 13:31:37.374993 ignutils-0.0.7/src/ignutils.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1291 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3868 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      304 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-17 13:31:37.000000 ignutils-0.0.7/src/ignutils.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.070937 ignutils-0.0.8/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-12 14:41:07.000000 ignutils-0.0.8/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1356 2024-04-22 09:27:58.070937 ignutils-0.0.8/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6016 2024-04-22 09:26:52.000000 ignutils-0.0.8/README.md
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      753 2024-04-22 09:26:52.000000 ignutils-0.0.8/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2024-04-22 09:26:52.000000 ignutils-0.0.8/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-22 09:27:58.070937 ignutils-0.0.8/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:57.906938 ignutils-0.0.8/src/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:57.978937 ignutils-0.0.8/src/ignutils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3694 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    45289 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/active_augmentation.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4159 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/algo_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:57.982937 ignutils-0.0.8/src/ignutils/autoui_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/autoui_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3885 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/autoui_utils/autogui_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    20681 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/autoui_utils/autotest_recplayback.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2484 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/autoui_utils/calculator_demo.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.002937 ignutils-0.0.8/src/ignutils/calib_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1412 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/angle_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6380 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/charuco_mono_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16504 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/charuco_stereo_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14815 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/infer_depth.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5981 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/mono_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3770 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/mono_dump.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6312 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/mono_error_calc.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3647 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/mono_undistort.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    44010 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/optimize_depth.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7902 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/point_depth_demo.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10569 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/pose_estimate.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7728 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/rs_crop_dump.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10662 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/stereo_3d_error_calc.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14560 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/stereo_calib.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4941 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/stereo_dump.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10057 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/stereo_error_calc.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5667 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/calib_utils/stereo_record.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.002937 ignutils-0.0.8/src/ignutils/cam_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      871 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/cam_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5755 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/cam_utils/camera_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1676 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/cam_utils/gopro_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6950 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/cam_utils/realsense_reader.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    12744 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/clone_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5347 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/config_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37875 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/contour_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4201 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/docker_utils.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    10467 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/draw_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14237 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/file_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1094 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/filter_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8726 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/fisheye_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4775 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/geom_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5746 2024-04-17 13:31:28.000000 ignutils-0.0.8/src/ignutils/gpu_utils.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    24667 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/img_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3061 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/json_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1663 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/keyboard_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5654 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/labelme_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10540 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/license_check.py
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)    20812 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/mouse_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2094 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/multi_process_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.006937 ignutils-0.0.8/src/ignutils/o3d_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/o3d_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1196 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/o3d_utils/plot_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3372 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/o3d_utils/read_rosbag.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8528 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/o3d_utils/registration_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.018937 ignutils-0.0.8/src/ignutils/registration/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      916 2024-04-17 06:11:12.000000 ignutils-0.0.8/src/ignutils/registration/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4521 2024-04-17 06:11:12.000000 ignutils-0.0.8/src/ignutils/registration/ecc_register.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    18564 2024-04-17 06:11:12.000000 ignutils-0.0.8/src/ignutils/registration/keypoint_register.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1825 2024-04-17 06:11:12.000000 ignutils-0.0.8/src/ignutils/registration/register_abstract.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1257 2024-04-17 06:11:12.000000 ignutils-0.0.8/src/ignutils/registration/register_wrapper.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8253 2024-04-17 06:11:12.000000 ignutils-0.0.8/src/ignutils/registration/superglue_register.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.018937 ignutils-0.0.8/src/ignutils/segmentation/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      983 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/segmentation/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.018937 ignutils-0.0.8/src/ignutils/segmentation/sam/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      941 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/segmentation/sam/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8652 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/segmentation/sam/fine_tune.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7671 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/segmentation/sam/sam_finetuned_infer.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10390 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/segmentation/sam/sam_infer.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4012 2024-04-22 09:26:52.000000 ignutils-0.0.8/src/ignutils/segmentation/segment.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.022937 ignutils-0.0.8/src/ignutils/selenium/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1254 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/selenium/selenium_test.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12894 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/show_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5265 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/ssh_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.042937 ignutils-0.0.8/src/ignutils/stitch_det_track/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      812 2024-04-17 12:21:27.000000 ignutils-0.0.8/src/ignutils/stitch_det_track/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6126 2024-04-17 12:21:27.000000 ignutils-0.0.8/src/ignutils/stitch_det_track/extract_gps_data.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8250 2024-04-17 12:21:27.000000 ignutils-0.0.8/src/ignutils/stitch_det_track/register_seq.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5518 2024-04-17 12:21:27.000000 ignutils-0.0.8/src/ignutils/stitch_det_track/stitch.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    45952 2024-04-17 12:21:27.000000 ignutils-0.0.8/src/ignutils/stitch_det_track/stitch_det_track_seq.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2891 2024-04-17 12:21:27.000000 ignutils-0.0.8/src/ignutils/stitch_det_track/unique_identifier.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3232 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/system_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      993 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/timer_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19564 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/transform_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5449 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/transfrom_crops.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1756 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/typehint_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.042937 ignutils-0.0.8/src/ignutils/video_utils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      826 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2887 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/dump_frames.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2596 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/exif_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3740 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/folder_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3275 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/play_video.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12810 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/video_reader.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8329 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/video_sync.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4369 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/video_utils/video_writer.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:57.906938 ignutils-0.0.8/src/ignutils/vo/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.050937 ignutils-0.0.8/src/ignutils/vo/mono_vo/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3882 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/Visualization.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1964 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/feature_det.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2983 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/feature_track.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6374 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/find_match.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6074 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/main.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22917 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/mono_VO.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2181 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/optimizer.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      684 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/mono_vo/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.050937 ignutils-0.0.8/src/ignutils/vo/stereo_vo/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5071 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/stereo_vo/data_handler.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    23487 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/vo/stereo_vo/stereo_vo.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.070937 ignutils-0.0.8/src/ignutils/workflow/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      107 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      812 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/__main__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8004 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/filter_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6494 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/keras_seg_mlnode.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    17255 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/mlnode.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    25301 2024-04-17 11:53:25.000000 ignutils-0.0.8/src/ignutils/workflow/node_config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4818 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/node_utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5086 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/seg_mlnode.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12781 2024-04-17 09:28:21.000000 ignutils-0.0.8/src/ignutils/workflow/workflow_main.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3435 2024-04-16 12:04:09.000000 ignutils-0.0.8/src/ignutils/yaml_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-22 09:27:58.070937 ignutils-0.0.8/src/ignutils.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1356 2024-04-22 09:27:57.000000 ignutils-0.0.8/src/ignutils.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4124 2024-04-22 09:27:57.000000 ignutils-0.0.8/src/ignutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-22 09:27:57.000000 ignutils-0.0.8/src/ignutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2024-04-22 09:27:57.000000 ignutils-0.0.8/src/ignutils.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-22 09:27:57.000000 ignutils-0.0.8/src/ignutils.egg-info/top_level.txt
```

### Comparing `ignutils-0.0.7/LICENSE` & `ignutils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/PKG-INFO` & `ignutils-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignutils
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small CV test package
 Author-email: Ignitarium <jerin.antony@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ignutils
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ignutils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,7 +39,9 @@
 Requires-Dist: scikit-image
 Requires-Dist: selenium
 Requires-Dist: shapely
 Requires-Dist: sympy
 Requires-Dist: termcolor
 Requires-Dist: bs4
 Requires-Dist: scipy
+Requires-Dist: segment-anything==1.0
+Requires-Dist: transformers
```

### Comparing `ignutils-0.0.7/pyproject.toml` & `ignutils-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ignutils"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Ignitarium", email="jerin.antony@ignitarium.com" },
 ]
 description = "A small CV test package"
 # readme = "pypi/README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

### Comparing `ignutils-0.0.7/src/ignutils/__init__.py` & `ignutils-0.0.8/src/ignutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,8 +88,9 @@
 from ignutils.workflow.seg_mlnode import *
 from ignutils.workflow.workflow_main import *
 
 from ignutils.stitch_det_track.extract_gps_data import *
 from ignutils.stitch_det_track.register_seq import *
 from ignutils.stitch_det_track.stitch import *
 from ignutils.stitch_det_track.stitch_det_track_seq import *
-from ignutils.stitch_det_track.unique_identifier import *
+from ignutils.stitch_det_track.unique_identifier import *
+#from ignutils.segmentation.segment import *
```

### Comparing `ignutils-0.0.7/src/ignutils/active_augmentation.py` & `ignutils-0.0.8/src/ignutils/active_augmentation.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/algo_utils.py` & `ignutils-0.0.8/src/ignutils/algo_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/autoui_utils/__init__.py` & `ignutils-0.0.8/src/ignutils/autoui_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/autoui_utils/autogui_utils.py` & `ignutils-0.0.8/src/ignutils/autoui_utils/autogui_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/autoui_utils/autotest_recplayback.py` & `ignutils-0.0.8/src/ignutils/autoui_utils/autotest_recplayback.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/autoui_utils/calculator_demo.py` & `ignutils-0.0.8/src/ignutils/autoui_utils/calculator_demo.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/angle_utils.py` & `ignutils-0.0.8/src/ignutils/calib_utils/angle_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/charuco_mono_calib.py` & `ignutils-0.0.8/src/ignutils/calib_utils/charuco_mono_calib.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/charuco_stereo_calib.py` & `ignutils-0.0.8/src/ignutils/calib_utils/charuco_stereo_calib.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/infer_depth.py` & `ignutils-0.0.8/src/ignutils/calib_utils/infer_depth.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/mono_calib.py` & `ignutils-0.0.8/src/ignutils/calib_utils/mono_calib.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/mono_dump.py` & `ignutils-0.0.8/src/ignutils/calib_utils/mono_dump.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/mono_error_calc.py` & `ignutils-0.0.8/src/ignutils/calib_utils/mono_error_calc.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/mono_undistort.py` & `ignutils-0.0.8/src/ignutils/calib_utils/mono_undistort.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/optimize_depth.py` & `ignutils-0.0.8/src/ignutils/calib_utils/optimize_depth.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/point_depth_demo.py` & `ignutils-0.0.8/src/ignutils/calib_utils/point_depth_demo.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/pose_estimate.py` & `ignutils-0.0.8/src/ignutils/calib_utils/pose_estimate.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/rs_crop_dump.py` & `ignutils-0.0.8/src/ignutils/calib_utils/rs_crop_dump.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/stereo_3d_error_calc.py` & `ignutils-0.0.8/src/ignutils/calib_utils/stereo_3d_error_calc.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/stereo_calib.py` & `ignutils-0.0.8/src/ignutils/calib_utils/stereo_calib.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/stereo_dump.py` & `ignutils-0.0.8/src/ignutils/calib_utils/stereo_dump.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/stereo_error_calc.py` & `ignutils-0.0.8/src/ignutils/calib_utils/stereo_error_calc.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/calib_utils/stereo_record.py` & `ignutils-0.0.8/src/ignutils/calib_utils/stereo_record.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/cam_utils/__init__.py` & `ignutils-0.0.8/src/ignutils/cam_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/cam_utils/camera_reader.py` & `ignutils-0.0.8/src/ignutils/cam_utils/camera_reader.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/cam_utils/gopro_reader.py` & `ignutils-0.0.8/src/ignutils/cam_utils/gopro_reader.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/cam_utils/realsense_reader.py` & `ignutils-0.0.8/src/ignutils/cam_utils/realsense_reader.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/clone_utils.py` & `ignutils-0.0.8/src/ignutils/clone_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/config_utils.py` & `ignutils-0.0.8/src/ignutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/contour_utils.py` & `ignutils-0.0.8/src/ignutils/contour_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/docker_utils.py` & `ignutils-0.0.8/src/ignutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/draw_utils.py` & `ignutils-0.0.8/src/ignutils/draw_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -266,14 +266,39 @@
     if copy_flag:
         img = img.copy()
     contours = np.array(contours).reshape((len(contours), -1, 1, 2)).astype(np.int32)  # type: ignore
     img = cv2.drawContours(img, contours, -1, color, thickness)
     return img
 
 
+def ansi_colors():
+    """
+    Generate ANSI codes for different colors used in print statements.
+
+    Returns:
+        dict: A dictionary containing color names as keys and their corresponding
+              ANSI escape codes as values.
+
+    Example:
+        color_codes = ansi_colors()
+        print(f"{color_codes['GREEN']}This text is in green color.{color_codes['RESET']}")
+    """
+    colors = {
+        "BLACK": "\033[30m",
+        "RED": "\033[31m",
+        "GREEN": "\033[32m",
+        "YELLOW": "\033[33m",
+        "BLUE": "\033[34m",
+        "MAGENTA": "\033[35m",
+        "CYAN": "\033[36m",
+        "WHITE": "\033[37m",
+        "RESET": "\033[0m",
+    }
+    return colors
+
 class TestDrawUtils(unittest.TestCase):
     """test draw utils"""
 
     @classmethod
     def setUpClass(cls):
         cls.image_ = cv2.imread("samples/Scopito_1.JPG")
         cls.json_dict_ = read_json("samples/Scopito_1.json")
```

### Comparing `ignutils-0.0.7/src/ignutils/file_utils.py` & `ignutils-0.0.8/src/ignutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/filter_utils.py` & `ignutils-0.0.8/src/ignutils/filter_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/fisheye_utils.py` & `ignutils-0.0.8/src/ignutils/fisheye_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/geom_utils.py` & `ignutils-0.0.8/src/ignutils/geom_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/gpu_utils.py` & `ignutils-0.0.8/src/ignutils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/img_utils.py` & `ignutils-0.0.8/src/ignutils/img_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/json_utils.py` & `ignutils-0.0.8/src/ignutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/keyboard_utils.py` & `ignutils-0.0.8/src/ignutils/keyboard_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/labelme_utils.py` & `ignutils-0.0.8/src/ignutils/labelme_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/license_check.py` & `ignutils-0.0.8/src/ignutils/license_check.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/mouse_utils.py` & `ignutils-0.0.8/src/ignutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/multi_process_utils.py` & `ignutils-0.0.8/src/ignutils/multi_process_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/o3d_utils/plot_utils.py` & `ignutils-0.0.8/src/ignutils/o3d_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/o3d_utils/read_rosbag.py` & `ignutils-0.0.8/src/ignutils/o3d_utils/read_rosbag.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/o3d_utils/registration_utils.py` & `ignutils-0.0.8/src/ignutils/o3d_utils/registration_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/registration/__init__.py` & `ignutils-0.0.8/src/ignutils/registration/__init__.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/registration/ecc_register.py` & `ignutils-0.0.8/src/ignutils/registration/ecc_register.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/registration/keypoint_register.py` & `ignutils-0.0.8/src/ignutils/registration/keypoint_register.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/registration/register_abstract.py` & `ignutils-0.0.8/src/ignutils/registration/register_abstract.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/registration/register_wrapper.py` & `ignutils-0.0.8/src/ignutils/registration/register_wrapper.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/registration/superglue_register.py` & `ignutils-0.0.8/src/ignutils/registration/superglue_register.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/selenium/selenium_test.py` & `ignutils-0.0.8/src/ignutils/selenium/selenium_test.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/show_utils.py` & `ignutils-0.0.8/src/ignutils/show_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/ssh_utils.py` & `ignutils-0.0.8/src/ignutils/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/stitch_det_track/__init__.py` & `ignutils-0.0.8/src/ignutils/stitch_det_track/__init__.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/stitch_det_track/extract_gps_data.py` & `ignutils-0.0.8/src/ignutils/stitch_det_track/extract_gps_data.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/stitch_det_track/register_seq.py` & `ignutils-0.0.8/src/ignutils/stitch_det_track/register_seq.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/stitch_det_track/stitch.py` & `ignutils-0.0.8/src/ignutils/stitch_det_track/stitch.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/stitch_det_track/stitch_det_track_seq.py` & `ignutils-0.0.8/src/ignutils/stitch_det_track/stitch_det_track_seq.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/stitch_det_track/unique_identifier.py` & `ignutils-0.0.8/src/ignutils/stitch_det_track/unique_identifier.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/system_utils.py` & `ignutils-0.0.8/src/ignutils/system_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/timer_utils.py` & `ignutils-0.0.8/src/ignutils/timer_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/transform_utils.py` & `ignutils-0.0.8/src/ignutils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/transfrom_crops.py` & `ignutils-0.0.8/src/ignutils/transfrom_crops.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/typehint_utils.py` & `ignutils-0.0.8/src/ignutils/typehint_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/__init__.py` & `ignutils-0.0.8/src/ignutils/video_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/dump_frames.py` & `ignutils-0.0.8/src/ignutils/video_utils/dump_frames.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/exif_utils.py` & `ignutils-0.0.8/src/ignutils/video_utils/exif_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/folder_reader.py` & `ignutils-0.0.8/src/ignutils/video_utils/folder_reader.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/play_video.py` & `ignutils-0.0.8/src/ignutils/video_utils/play_video.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/video_reader.py` & `ignutils-0.0.8/src/ignutils/video_utils/video_reader.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/video_sync.py` & `ignutils-0.0.8/src/ignutils/video_utils/video_sync.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/video_utils/video_writer.py` & `ignutils-0.0.8/src/ignutils/video_utils/video_writer.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/Visualization.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/Visualization.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/feature_det.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/feature_det.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/feature_track.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/feature_track.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/find_match.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/find_match.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/main.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/main.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/mono_VO.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/mono_VO.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/optimizer.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/optimizer.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/mono_vo/utils.py` & `ignutils-0.0.8/src/ignutils/vo/mono_vo/utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/stereo_vo/data_handler.py` & `ignutils-0.0.8/src/ignutils/vo/stereo_vo/data_handler.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/vo/stereo_vo/stereo_vo.py` & `ignutils-0.0.8/src/ignutils/vo/stereo_vo/stereo_vo.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/__main__.py` & `ignutils-0.0.8/src/ignutils/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/filter_utils.py` & `ignutils-0.0.8/src/ignutils/workflow/filter_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/keras_seg_mlnode.py` & `ignutils-0.0.8/src/ignutils/workflow/keras_seg_mlnode.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/mlnode.py` & `ignutils-0.0.8/src/ignutils/workflow/mlnode.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/node_config.py` & `ignutils-0.0.8/src/ignutils/workflow/node_config.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/node_utils.py` & `ignutils-0.0.8/src/ignutils/workflow/node_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/seg_mlnode.py` & `ignutils-0.0.8/src/ignutils/workflow/seg_mlnode.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/workflow/workflow_main.py` & `ignutils-0.0.8/src/ignutils/workflow/workflow_main.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils/yaml_utils.py` & `ignutils-0.0.8/src/ignutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.7/src/ignutils.egg-info/PKG-INFO` & `ignutils-0.0.8/src/ignutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignutils
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small CV test package
 Author-email: Ignitarium <jerin.antony@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ignutils
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ignutils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,7 +39,9 @@
 Requires-Dist: scikit-image
 Requires-Dist: selenium
 Requires-Dist: shapely
 Requires-Dist: sympy
 Requires-Dist: termcolor
 Requires-Dist: bs4
 Requires-Dist: scipy
+Requires-Dist: segment-anything==1.0
+Requires-Dist: transformers
```

### Comparing `ignutils-0.0.7/src/ignutils.egg-info/SOURCES.txt` & `ignutils-0.0.8/src/ignutils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -66,14 +66,20 @@
 src/ignutils/o3d_utils/registration_utils.py
 src/ignutils/registration/__init__.py
 src/ignutils/registration/ecc_register.py
 src/ignutils/registration/keypoint_register.py
 src/ignutils/registration/register_abstract.py
 src/ignutils/registration/register_wrapper.py
 src/ignutils/registration/superglue_register.py
+src/ignutils/segmentation/__init__.py
+src/ignutils/segmentation/segment.py
+src/ignutils/segmentation/sam/__init__.py
+src/ignutils/segmentation/sam/fine_tune.py
+src/ignutils/segmentation/sam/sam_finetuned_infer.py
+src/ignutils/segmentation/sam/sam_infer.py
 src/ignutils/selenium/selenium_test.py
 src/ignutils/stitch_det_track/__init__.py
 src/ignutils/stitch_det_track/extract_gps_data.py
 src/ignutils/stitch_det_track/register_seq.py
 src/ignutils/stitch_det_track/stitch.py
 src/ignutils/stitch_det_track/stitch_det_track_seq.py
 src/ignutils/stitch_det_track/unique_identifier.py
```

