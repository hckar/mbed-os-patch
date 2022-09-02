# Copyright (c) 2022 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-disco-f407vg INTERFACE)

target_sources(mbed-disco-f407vg
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-disco-f407vg
    INTERFACE
        .
)

target_link_libraries(mbed-disco-f407vg INTERFACE mbed-stm32f407xg)
