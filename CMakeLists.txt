cmake_minimum_required(VERSION 3.16)

set(CMAKE_TOOLCHAIN_FILE ${CMAKE_CURRENT_LIST_DIR}/SDK/toolchain-avr-gcc.cmake)

project(AVR_GCC_BAREBONES_PROJECT C CXX)

add_subdirectory(lib/CayenneLPP_MemOptimized)

add_executable(barebones_app src/main.cpp)

