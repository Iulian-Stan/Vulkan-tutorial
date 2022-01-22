cmake_minimum_required(VERSION 3.15)

project(Vulkan_Exercise)

SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/${CMAKE_BUILD_TYPE}/bin)
SET(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/${CMAKE_BUILD_TYPE}/lib)
SET(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/${CMAKE_BUILD_TYPE}/lib)

find_package(Vulkan REQUIRED)

# Adding dependencies
add_subdirectory(deps)

# Adding tutorials
add_subdirectory(ex_01)    # Creating OpenGL Window using FreeGLUT
