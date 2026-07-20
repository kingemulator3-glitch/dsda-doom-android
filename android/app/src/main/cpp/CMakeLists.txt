cmake_minimum_required(VERSION 3.22.1)

project(dsda-doom)

add_library(
    dsda-doom
    SHARED
    dummy.cpp
)

find_library(
    log-lib
    log
)

target_link_libraries(
    dsda-doom
    ${log-lib}
)
