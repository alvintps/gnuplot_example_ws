cmake_minimum_required(VERSION 3.10)
project(gnuplot_example C CXX)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/bin)

add_library(gnuplot external/gnuplot_i.c)
include_directories(external)

add_executable(example src/example.c)
target_link_libraries(example gnuplot)

add_executable(anim src/anim.c)
target_link_libraries(anim gnuplot)

add_executable(sinepng src/sinepng.c)
target_link_libraries(sinepng gnuplot)
