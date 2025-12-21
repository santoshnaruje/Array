cmake_minimum_required(VERSION 3.16)
project(Array)

set(CMAKE_CXX_STANDARD 14)

file(GLOB SOURCES "*.cpp")

foreach(src ${SOURCES})
    get_filename_component(exec_name ${src} NAME_WE)
    add_executable(${exec_name} ${src}
            remove_duplicates_from_sorted_array.cpp
            move_all_the_zeros_to_the_end_of_the_array.cpp
            find_the_union.cpp
            merge2sortedarrays.cpp
            find_missing_number_in_array.cpp
            maximum_consecutive_ones.cpp
    )
endforeach()
