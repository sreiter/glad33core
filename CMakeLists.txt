cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project (glad)

set (headers
     include/glad/glad.h
     include/KHR/khrplatform.h)

set (sources
     src/glad.c)

add_library (glad ${sources} ${headers})
target_include_directories (glad PUBLIC include)
