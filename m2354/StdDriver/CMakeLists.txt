# SPDX-License-Identifier: Apache-2.0
#
# Copyright (c) 2022 Nuvoton Technology Corporation.

zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_HAL src/sys.c)

zephyr_library_sources(src/clk.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_GPIO src/gpio.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_UART src/uart.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_FMC src/fmc.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_I2C src/i2c.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_SPI src/spi.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_SPI src/qspi.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_PWM src/epwm.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_USBD src/usbd.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_HSUSBD src/hsusbd.c)
zephyr_library_sources_ifdef(CONFIG_HAS_NUMAKER_CANFD src/canfd.c)