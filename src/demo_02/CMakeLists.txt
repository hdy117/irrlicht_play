cmake_minimum_required(VERSION 3.17)

aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} src_files)

add_executable(demo_02 ${src_files})
target_link_libraries(demo_02 ${lib_sys} ${lib_log})
install(TARGETS demo_02 RUNTIME DESTINATION ${output_dir})