cmake_minimum_required(VERSION 3.22)
project(mycraft)

set(CMAKE_CXX_STANDARD 17)

include_directories(
    src
    ./include
)

link_directories(
    ./lib
)

add_executable(mycraft
    src/main.cpp
    src/deps/glad.c
)

target_link_libraries(mycraft glfw.3.3)
