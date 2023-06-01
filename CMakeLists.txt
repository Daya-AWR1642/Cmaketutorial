cmake_minimum_required(VERSION 3.15)
project(SimpleCmakeExample)

add_subdirectory(include)
add_subdirectory(src)

option(BUILD_EXAPLES "Whether or not to build examples"
ON)

if (BUILD_EXAPLES)
    message(STATUS "Building examples..")
    add_subdirectory(examples)

endif()