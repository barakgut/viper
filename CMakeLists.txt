cmake_minimum_required(VERSION 3.13.1)

set(BOARD_ROOT ${CMAKE_CURRENT_LIST_DIR})
set(BOARD rookieboard)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(viper)

target_sources(app PRIVATE src/main.c)