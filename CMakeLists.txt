cmake_minimum_required(VERSION 3.23)
project(StaticLibTest)

set(CMAKE_CXX_STANDARD 20)
set(LIBS d3d9 d3d11 d3dcompiler_43)

add_library(StaticLibTest library.cpp)
target_link_libraries(StaticLibTest ${LIBS})
