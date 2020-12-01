# We do not want to build the shared library
set(glew-cmake_BUILD_SHARED OFF CACHE BOOL "" FORCE)
set(GLFW_INSTALL OFF CACHE BOOL "" FORCE)

add_subdirectory(GLFW)
add_subdirectory(GLEW)

set_target_properties(libglew_static PROPERTIES FOLDER submodules)
set_target_properties(glfw PROPERTIES FOLDER submodules)