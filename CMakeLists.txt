cmake_minimum_required(VERSION 3.6)

project(func)
set(func_srcs func.c)
add_library(func SHARED ${func_srcs})
install(TARGETS func DESTINATION .)
