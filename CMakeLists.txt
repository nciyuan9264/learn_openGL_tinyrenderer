cmake_minimum_required(VERSION 3.20)
project(tinyrenderer_win)
add_definitions(-std=c++11)

# 设置代码文件
set(SRC_DIR ${PROJECT_SOURCE_DIR}/src/)

# 添加头文件
set(HEADER_DIR ${PROJECT_SOURCE_DIR}/include/)
include_directories(${HEADER_DIR})

# 设置可执行文件输出路径
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/output)

file(GLOB SOURCES ${SRC_DIR}/*.cpp)
add_executable(${PROJECT_NAME} ${SOURCES})