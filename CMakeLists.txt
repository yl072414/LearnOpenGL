cmake_minimum_required(VERSION 3.5)

project(LearnOpenGL LANGUAGES CXX)

set(SRC
    src/glad.c
    src/main.cpp
)

link_directories(${LearnOpenGL_SOURCE_DIR}/lib)

add_executable(LearnOpenGL ${SRC})

target_include_directories(LearnOpenGL
    PRIVATE 
        ${PROJECT_SOURCE_DIR}/include
)

target_link_libraries(LearnOpenGL 
	PRIVATE 
		opengl32.lib glfw3.lib)