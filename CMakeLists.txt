cmake_minimum_required(VERSION 3.17)

project(irrlicht_play)

set(output_dir ${CMAKE_CURRENT_SOURCE_DIR}/bin)

set(CMAKE_CXX_STANDARD 17)
add_compile_options(-fPIC)

set(lib_sys pthread)
set(lib_log glog gflags)

include_directories(/usr/include 
    /user/include/irrlicht 
    /usr/include/eigen3
    ${CMAKE_SOURCE_DIR})

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/demo_01)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/demo_02)

