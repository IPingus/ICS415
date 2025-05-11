cmake_minimum_required(VERSION 3.10)
project(MinecraftClone)

set(CMAKE_CXX_STANDARD 11)

# Add GLFW, GLEW, and GLM to your project
find_package(GLFW3 REQUIRED)
find_package(GLEW REQUIRED)

# You need to set the GLM directory for the header-only library
include_directories(path_to_glm)

# Add your source files
add_executable(MinecraftClone main.cpp)

# Link your libraries
target_link_libraries(MinecraftClone glfw GLEW)
