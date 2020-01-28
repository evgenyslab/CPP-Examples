cmake_minimum_required(VERSION 3.0.0)
project(mylib)
add_compile_options(-std=c++11)

include_directories(
        include
)

add_library(mylib STATIC src/myClass.cpp)