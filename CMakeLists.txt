# Copyright (c) 2021 Nordic Semiconductor ASA
# SPDX-License-Identifier: Apache-2.0
#
# This CMake file is picked by the Zephyr build system because it is defined
# as the module CMake entry point (see zephyr/module.yml).

zephyr_library()
set(MY_MODULE_DIR ${ZEPHYR_CURRENT_MODULE_DIR})
zephyr_include_directories(
  .
  ${MY_MODULE_DIR}/include
  )
zephyr_library_sources(
  ${MY_MODULE_DIR}/src/my-source.c
  )
