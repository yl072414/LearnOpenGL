cmake_minimum_required(VERSION 3.5)

project(LearnOpenGL LANGUAGES CXX)

set(SRC_LIST main.cpp glad.c)

include_directories(${LearnOpenGL_SOURCE_DIR}/include)
link_directories(${LearnOpenGL_SOURCE_DIR}/lib)

add_executable(LearnOpenGL ${SRC_LIST})

target_link_libraries(LearnOpenGL opengl32.lib glfw3.lib)