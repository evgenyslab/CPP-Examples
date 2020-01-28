cmake_minimum_required(VERSION 3.0.0)
project(myproj)
add_compile_options(-std=c++11)

include_directories(
        include
        # include the inc folder of the external library:
        ../mylib/include
)

# create variable for full path to static library:
SET(MYLIB_SOURCE /Users/en/Git/cpplinking/mylib/cmake-build-debug)

# create executible linked to source: (can add .h files)
add_executable(test src/main.cpp)

# add linker to static library:
target_link_libraries(test ${MYLIB_SOURCE}/libmylib.a)