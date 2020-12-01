set(RAY_FIRE_SOURCE_DIR "${CMAKE_CURRENT_SOURCE_DIR}")
set(RAY_FIRE_HEADER_DIR "${CMAKE_CURRENT_SOURCE_DIR}")

file(GLOB_RECURSE RAY_FIRE_FILES "RayFire/*.h" "RayFire/*.cpp")

# TODO: Add support for shared linking
add_library(RayFire STATIC "${RAY_FIRE_FILES}")
