# Copyright (c) 2022 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-xxx INTERFACE)

target_sources(mbed-xxx
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-xxx
    INTERFACE
        .
)

target_link_libraries(mbed-xxx INTERFACE mbed-stm32l4s7xi)
