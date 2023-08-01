cmake_minimum_required(VERSION 3.12)

project(Transcode)

set(FFMPEG_DIR "E:/EBmgProjects/bmg/3rdMisc/FFmpegBuild/ffmpeg6/WIN64")

# 确定 FFmpeg 的各个组件的路径
set(FFMPEG_INCLUDE_DIR ${FFMPEG_DIR}/include)
set(FFMPEG_LIBRARY_DIR ${FFMPEG_DIR}/lib)

# 链接 FFmpeg 的库文件
link_directories(${FFMPEG_LIBRARY_DIR})

# 添加包含的头文件目录
include_directories(${FFMPEG_INCLUDE_DIR})

add_executable(Transcode vaapi_transcode.c)






