# SPDX-License-Identifier: Apache-2.0
#
# Copyright (c) 2022 Nuvoton Technology Corporation.

zephyr_include_directories(StdDriver/inc)
zephyr_include_directories(Devices/M2354/Include)
zephyr_include_directories(dt-bindings/pinctrl)

zephyr_sources_ifdef(CONFIG_SOC_SERIES_M2354 Devices/M2354/Source/system_M2354.c)

add_subdirectory(StdDriver)
