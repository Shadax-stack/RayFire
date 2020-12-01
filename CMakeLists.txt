cmake_minimum_required(VERSION 2.8)
cmake_policy(SET CMP0048 NEW)

project(RayFirePathTracer)

add_subdirectory(submodules)
add_subdirectory(src)
add_subdirectory(examples)

set(RAY_FIRE_SUBMODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}")