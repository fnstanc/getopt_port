project (getopt)
cmake_minimum_required (VERSION 2.8)

add_library(getopt STATIC getopt.h getopt.c)

add_executable(getopt_tests main.cpp testfx.h testfx.cpp getopt_tests.cpp getopt_long_tests.cpp)
target_link_libraries(getopt_tests getopt)
