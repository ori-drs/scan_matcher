add_definitions( -ggdb3 -std=gnu99 )

cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(control)


add_executable(rpg-scan-matcher scan_matcher.cpp  )
target_link_libraries(rpg-scan-matcher boost_system)
pods_use_pkg_config_packages(rpg-scan-matcher
 bot2-core frsm
 path-util
 bot2-frames bot2-frames_cpp
 eigen3)
pods_install_executables(rpg-scan-matcher )