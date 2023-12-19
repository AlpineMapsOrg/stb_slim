cmake_minimum_required(VERSION 3.24)
project(stb_slim_src LANGUAGES CXX)

add_library(stb_slim 
    stb_slim/stb_truetype.h
)

target_include_directories(stb_slim PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_compile_features(stb_slim PUBLIC cxx_std_20)
