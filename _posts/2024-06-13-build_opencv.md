---
layout: post
title: "编译opencv"
date:   2024-06-13
tags: [opencv]
comments: true
author: weogen
---

编译opencv...

<!-- more -->


# 安装依赖  
[参考网址](https://dev.to/swervin/how-to-install-opencv-4-2-0-on-ubuntu-18-04-3i7l)  

# cmake 指令  
cmake -D CMAKE_BUILD_TYPE=Release \
-D CMAKE_INSTALL_PREFIX=/usr/local \
-D OPENCV_EXTRA_MODULES_PATH=../../opencv_contrib-4.5.4/modules \
-D WITH_TBB=ON \
-D WITH_IPP=OFF \
-D WITH_1394=OFF \
-D BUILD_WITH_DEBUG_INFO=OFF \
-D BUILD_DOCS=OFF \
-D INSTALL_C_EXAMPLES=OFF \
-D INSTALL_PYTHON_EXAMPLES=OFF \
-D BUILD_EXAMPLES=OFF \
-D BUILD_TESTS=OFF \
-D BUILD_PERF_TESTS=OFF \
-D WITH_QT=OFF \
-D WITH_GTK=ON \
-D WITH_OPENGL=OFF \
-D WITH_V4L=ON  \
-D WITH_FFMPEG=ON \
-D WITH_XINE=ON \
-D BUILD_NEW_PYTHON_SUPPORT=OFF \
-D BUILD_JAVA=OFF \
-D BUILD_opencv_python2=OFF \
-D BUILD_opencv_python3=OFF \
-D WITH_OPENCL=ON \
-D WITH_ONNX=ON \
-D OPENCV_GENERATE_PKGCONFIG=ON ../

sudo make -j8

sudo make install

