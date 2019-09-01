cmake_minimum_required(VERSION 3.0.0)
project(sdl2test VERSION 0.1.0)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(sdl2test main.cpp)

target_link_libraries(sdl2test ${SDL2_LIBRARIES})
