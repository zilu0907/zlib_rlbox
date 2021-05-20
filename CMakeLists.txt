cmake_minimum_required(VERSION 3.10)

# set the project name
project(zpipe_rlbox VERSION 2.0)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

SET_SOURCE_FILES_PROPERTIES( zpipe_verify.c PROPERTIES LANGUAGE CXX )

# link to zlib
find_package(ZLIB)

# add the executable
add_executable(zpipe_rlbox zpipe_verify.c)

target_link_libraries(zpipe_rlbox ZLIB::ZLIB)