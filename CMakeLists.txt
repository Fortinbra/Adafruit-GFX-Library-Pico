# Adafruit GFX Library
# https://github.com/adafruit/Adafruit-GFX-Library
# BSD License

cmake_minimum_required(VERSION 3.13)

add_library(Adafruit_GFX 
Adafruit_GFX.cpp
Adafruit_SPITFT.cpp
glcdfont.c
)
target_include_directories(Adafruit_GFX INTERFACE .)
target_link_libraries(Adafruit_GFX
					  Adafruit_BusIO
					  pico_stdlib
					  hardware_gpio
					  hardware_spi
					  hardware_i2c)
