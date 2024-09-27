# Adafruit GFX Library
# https://github.com/adafruit/Adafruit-GFX-Library
# BSD License

cmake_minimum_required(VERSION 3.5)

add_library(Adafruit_GFX 
Adafruit_GFX.cpp
Adafruit_GrayOLED.cpp
Adafruit_SPITFT.cpp
glcdfont.c
)
target_include_directories(Adafruit_GFX INTERFACE .)
