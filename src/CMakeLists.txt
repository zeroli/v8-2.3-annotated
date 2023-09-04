cmake_minimum_required(VERSION 3.8)

aux_source_directory(. SRCS)
aux_source_directory(x64 SRCS)
add_library(v8 STATIC ${SRCS})
target_include_directories(v8 PUBLIC ../src)
