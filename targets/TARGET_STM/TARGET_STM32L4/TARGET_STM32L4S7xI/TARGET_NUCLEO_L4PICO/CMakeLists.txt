# Copyright (c) 2022 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-nucleo-l4pico INTERFACE)

target_sources(mbed-nucleo-l4pico
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-nucleo-l4pico
    INTERFACE
        .
)

target_link_libraries(mbed-nucleo-l4pico INTERFACE mbed-stm32l4s7xi)
