cmake_minimum_required(VERSION 3.8)

project(Lab2)

set(SOURCE_EXE main.cpp)

set(SOURCE_LIB hello_lib.cpp)

add_library(hello_lib SHARED ${SOURCE_LIB})

add_executable(sayHello ${SOURCE_EXE})

target_link_libraries(sayHello hello_lib)
