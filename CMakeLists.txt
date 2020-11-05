cmake_minimum_required(VERSION 3.5)

project(HelloWindow LANGUAGES CXX)

include_directories(Include)
link_directories(Library)
LINK_LIBRARIES(glfw3.lib)

add_executable(HelloWindow main.cpp)