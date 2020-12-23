cmake_minimum_required(VERSION 3.5)

project(LearnOpenGL)

set(SRC
	src/glad.c
    src/main.cpp
)

add_executable(LearnOpenGL ${SRC})

target_include_directories(LearnOpenGL
    PRIVATE 
        ${PROJECT_SOURCE_DIR}/include
)

target_link_directories(LearnOpenGL
	PRIVATE
		${PROJECT_SOURCE_DIR}/lib
)

target_link_libraries(LearnOpenGL 
	PRIVATE 
		opengl32.lib glfw3.lib)