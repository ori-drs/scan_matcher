cmake_minimum_required(VERSION 2.8.12)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wno-deprecated-declarations")

# pull in the pods macros. See cmake/pods.cmake for documentation
set(POD_NAME scan_matcher)
include(cmake/pods.cmake)

add_subdirectory(src/scan_matcher)

