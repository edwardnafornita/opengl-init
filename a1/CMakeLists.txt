cmake_minimum_required(VERSION 3.10)
project(a1)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)
find_package(GLFW3 REQUIRED)

add_executable(a1 main.cpp)

target_link_libraries(a1 PRIVATE
    OpenGL::GL
    GLEW::GLEW
    glfw
)
