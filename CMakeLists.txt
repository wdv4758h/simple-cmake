cmake_minimum_required(VERSION 3.6)

project(func)
set(func_srcs func.c)
set(prog_srcs prog.c)
add_library(func SHARED ${func_srcs})
add_executable(prog ${prog_srcs})
install(TARGETS func DESTINATION .)
install(TARGETS prog DESTINATION .)
