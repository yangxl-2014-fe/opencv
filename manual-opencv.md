<!--

@created at 2020-06-22

#
#
#

-->

# Contents

- [Contents](#contents)
- [Algorithms](#algorithms)
  - [bilateral filter](#bilateral-filter)
  - [Images stitching](#images-stitching)

<!--

- <div align="left"><img src="xxx" height="" width="640" /></div>

#
#
#

<details>
<summary>
</summary>
<br/>
</details>

-->

# Algorithms

## bilateral filter

- ref: /home/ftx/Documents/yangxl-2014-fe/[fork]-Robot/pcl/manual-pcl.md

```bash
opencv$ tree -f -a | grep -i bilateral
│   │   │   ├── ./doc/js_tutorials/js_assets/js_filtering_bilateralFilter.html
│   │   │   │   │   ├── ./doc/py_tutorials/py_imgproc/py_filtering/images/bilateral.jpg
│   │   │   ├── ./doc/tutorials/imgproc/gausian_median_blur_bilateral_filter
│   │   │   │   ├── ./doc/tutorials/imgproc/gausian_median_blur_bilateral_filter/gausian_median_blur_bilateral_filter.markdown
│   │   │   │   └── ./doc/tutorials/imgproc/gausian_median_blur_bilateral_filter/images
│   │   │   │       ├── ./doc/tutorials/imgproc/gausian_median_blur_bilateral_filter/images/Smoothing_Tutorial_Result_Median_Filter.jpg
│   │   │   │       └── ./doc/tutorials/imgproc/gausian_median_blur_bilateral_filter/images/Smoothing_Tutorial_theory_gaussian_0.jpg
│   │   │   ├── ./modules/imgproc/perf/perf_bilateral.cpp
│   │   │   ├── ./modules/imgproc/src/bilateral_filter.dispatch.cpp
│   │   │   ├── ./modules/imgproc/src/bilateral_filter.simd.hpp
│   │   │   │   ├── ./modules/imgproc/src/opencl/bilateral.cl
│   │       ├── ./modules/imgproc/test/test_bilateral_filter.cpp
```

<!--

#
#
#

-->

## Images stitching

- [Images stitching - 3.4.11-pre](https://docs.opencv.org/3.4/d1/d46/group__stitching.html)

```bash
ftx@ftxD:~/Documents/yangxl-2014-fe/[fork]-Robot/opencv$ tree -f -a | grep -i stitching
│   │   │   │       ├── ./doc/tutorials/features2d/homography/images/homography_panorama_stitching.jpg
│   │   ├── ./doc/tutorials/stitching
│   │   │   ├── ./doc/tutorials/stitching/stitcher
│   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images
│   │   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images/affinepano.jpg
│   │   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images/boat.jpg
│   │   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images/budapest.jpg
│   │   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images/compressedPlaneA2B1.jpg
│   │   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images/fisheye.jpg
│   │   │   │   │   ├── ./doc/tutorials/stitching/stitcher/images/gvedit.jpg
│   │   │   │   │   └── ./doc/tutorials/stitching/stitcher/images/newspaper.jpg
│   │   │   │   └── ./doc/tutorials/stitching/stitcher/stitcher.markdown
│   │   │   └── ./doc/tutorials/stitching/table_of_content_stitching.markdown
│   ├── ./modules/stitching
│   │   ├── ./modules/stitching/CMakeLists.txt
│   │   ├── ./modules/stitching/doc
│   │   │   └── ./modules/stitching/doc/StitchingPipeline.jpg
│   │   ├── ./modules/stitching/include
│   │   │   └── ./modules/stitching/include/opencv2
│   │   │       ├── ./modules/stitching/include/opencv2/stitching
│   │   │       │   ├── ./modules/stitching/include/opencv2/stitching/detail
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/autocalib.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/blenders.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/camera.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/exposure_compensate.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/matchers.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/motion_estimators.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/seam_finders.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/timelapsers.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/util.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/util_inl.hpp
│   │   │       │   │   ├── ./modules/stitching/include/opencv2/stitching/detail/warpers.hpp
│   │   │       │   │   └── ./modules/stitching/include/opencv2/stitching/detail/warpers_inl.hpp
│   │   │       │   └── ./modules/stitching/include/opencv2/stitching/warpers.hpp
│   │   │       └── ./modules/stitching/include/opencv2/stitching.hpp
│   │   ├── ./modules/stitching/misc
│   │   │   └── ./modules/stitching/misc/python
│   │   │       ├── ./modules/stitching/misc/python/pyopencv_stitching.hpp
│   │   │       └── ./modules/stitching/misc/python/test
│   │   │           └── ./modules/stitching/misc/python/test/test_stitching.py
│   │   ├── ./modules/stitching/perf
│   │   │   ├── ./modules/stitching/perf/opencl
│   │   │   │   ├── ./modules/stitching/perf/opencl/perf_stitch.cpp
│   │   │   │   └── ./modules/stitching/perf/opencl/perf_warpers.cpp
│   │   │   ├── ./modules/stitching/perf/perf_estimators.cpp
│   │   │   ├── ./modules/stitching/perf/perf_main.cpp
│   │   │   ├── ./modules/stitching/perf/perf_matchers.cpp
│   │   │   ├── ./modules/stitching/perf/perf_precomp.hpp
│   │   │   └── ./modules/stitching/perf/perf_stich.cpp
│   │   ├── ./modules/stitching/src
│   │   │   ├── ./modules/stitching/src/autocalib.cpp
│   │   │   ├── ./modules/stitching/src/blenders.cpp
│   │   │   ├── ./modules/stitching/src/camera.cpp
│   │   │   ├── ./modules/stitching/src/cuda
│   │   │   │   ├── ./modules/stitching/src/cuda/build_warp_maps.cu
│   │   │   │   └── ./modules/stitching/src/cuda/multiband_blend.cu
│   │   │   ├── ./modules/stitching/src/exposure_compensate.cpp
│   │   │   ├── ./modules/stitching/src/matchers.cpp
│   │   │   ├── ./modules/stitching/src/motion_estimators.cpp
│   │   │   ├── ./modules/stitching/src/opencl
│   │   │   │   ├── ./modules/stitching/src/opencl/multibandblend.cl
│   │   │   │   └── ./modules/stitching/src/opencl/warpers.cl
│   │   │   ├── ./modules/stitching/src/precomp.hpp
│   │   │   ├── ./modules/stitching/src/seam_finders.cpp
│   │   │   ├── ./modules/stitching/src/stitcher.cpp
│   │   │   ├── ./modules/stitching/src/timelapsers.cpp
│   │   │   ├── ./modules/stitching/src/util.cpp
│   │   │   ├── ./modules/stitching/src/util_log.hpp
│   │   │   ├── ./modules/stitching/src/warpers.cpp
│   │   │   └── ./modules/stitching/src/warpers_cuda.cpp
│   │   └── ./modules/stitching/test
│   │       ├── ./modules/stitching/test/ocl
│   │       │   └── ./modules/stitching/test/ocl/test_warpers.cpp
│   │       ├── ./modules/stitching/test/test_blenders.cpp
│   │       ├── ./modules/stitching/test/test_blenders.cuda.cpp
│   │       ├── ./modules/stitching/test/test_main.cpp
│   │       ├── ./modules/stitching/test/test_matchers.cpp
│   │       └── ./modules/stitching/test/test_precomp.hpp
│   │   ├── ./samples/cpp/stitching.cpp
│   │   ├── ./samples/cpp/stitching_detailed.cpp
│   │   │   │       ├── ./samples/cpp/tutorial_code/features2D/Homography/panorama_stitching_rotating_camera.cpp
│   │       │       ├── ./samples/java/tutorial_code/features2D/Homography/PanoramaStitchingRotatingCamera.java
│   │   ├── ./samples/python/stitching_detailed.py
│   │   ├── ./samples/python/stitching.py
│   │   │   │       ├── ./samples/python/tutorial_code/features2D/Homography/panorama_stitching_rotating_camera.py

```

<!--

- <div align="left"><img src="xxx" height="" width="640" /></div>

#
#
#

<details>
<summary>
</summary>
<br/>
</details>

-->
