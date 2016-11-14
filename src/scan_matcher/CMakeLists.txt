cmake_minimum_required(VERSION 2.8.12 FATAL_ERROR)
project(scan_matcher)

add_executable(rpg-scan-matcher scan_matcher.cpp)
pods_use_pkg_config_packages(rpg-scan-matcher
 frsm
 path-util
 bot2-frames bot2-frames_cpp
 eigen3)
pods_install_executables(rpg-scan-matcher)
