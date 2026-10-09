cmake_minimum_required(VERSION 3.10)

project(hello LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(hello main.cpp src/hello.cpp)

target_include_directories(hello PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)
