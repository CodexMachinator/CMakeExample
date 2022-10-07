cmake_minimum_required(VERSION 3.15)
project(example)

find_package(Git REQUIRED)
set(CMAKE_CXX_STANDARD 14)

include_directories(src)

add_subdirectory(lib)
add_subdirectory(src)
add_subdirectory(tst)

