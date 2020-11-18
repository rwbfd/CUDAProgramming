cmake_minimum_required(VERSION 3.15)
project(simple-kernel LANGUAGES CXX CUDA)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(simple-kernel
        simple-kernel.cu)
set_target_properties(simple-kernel PROPERTIES CUDA_SEPARABLE_COMPILATION ON)