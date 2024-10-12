cmake_minimum_required(VERSION 3.10)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

project(HelloWindow)

find_package(glad CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)

add_executable(HelloWindow src/hello_window.cpp)

target_link_libraries(HelloWindow PRIVATE glad::glad glfw)
