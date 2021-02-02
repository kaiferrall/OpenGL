cmake_minimum_required(VERSION 3.17)
project(OpenGL)

set(CMAKE_CXX_STANDARD 14)

add_executable(OpenGL main.cpp)

add_subdirectory(dependencies/glfw-3.3.2)

include_directories(dependencies/glfw-3.3.2/include)

target_link_libraries(OpenGL glfw ${GLFW_LIBRARIES})