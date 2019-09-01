cmake_minimum_required(VERSION 3.0.0)
project(sdl2test VERSION 0.1.0)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${PROJECT_SOURCE_DIR}/cmake")

find_package(SDL2 REQUIRED)

include_directories(${SDL2_INCLUDE_DIR})

add_executable(sdl2test main.cpp)

target_link_libraries(sdl2test ${SDL2_LIBRARY})
