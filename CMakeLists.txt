
cmake_minimum_required (VERSION 3.10)

project (CJSON)

include (../cmake/cmake-flags.cmake)

aux_source_directory(. SOURCE_CJSON)

add_library(cjson STATIC ${SOURCE_CJSON})

target_include_directories(cjson INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

