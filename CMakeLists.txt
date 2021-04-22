# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.13.1)

# Depended on your own environment variable
set(GNUARMEMB_TOOLCHAIN_PATH "$ENV{GCC_ARM_HOME}")
set(ZEPHYR_TOOLCHAIN_VARIANT gnuarmemb)

list(APPEND BOARD_ROOT ${CMAKE_CURRENT_SOURCE_DIR})

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(zephyr_stm32f407_lvgl_demo)


FILE(GLOB app_sources src/*.c)
target_sources(app PRIVATE ${app_sources})