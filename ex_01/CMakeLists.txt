cmake_minimum_required(VERSION 3.15)

project(ex_01 LANGUAGES CXX)

add_executable(${PROJECT_NAME}
  main.cpp
  README.md
)

target_link_libraries(${PROJECT_NAME}
  PRIVATE
    Vulkan::Headers
    Vulkan::Vulkan
    glfw
    glm
)