cmake_minimum_required(VERSION 3.12)
project(MPAGSCipher VERSION 0.1.0)



set(CMAKE_VERBOSE_MAKEFILE ON)



set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_EXTENSIONS "-Wall -Wextra -Werror -Wfatal-error -Wshadow -pedantic")



add_executable(mpags-cipher mpags-cipher.cpp
 MPAGSCipher/TransformChar.cpp
 MPAGSCipher/TransformChar.hpp
)


target_include_directories(mpags-cipher PRIVATE MPAGSCipher)
target_compile_features(mpags-cipher PRIVATE cxx_std_20)



