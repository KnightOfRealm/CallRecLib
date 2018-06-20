cmake_minimum_required(VERSION 3.4.1)

add_library(callrecfix SHARED
            audio.h
            Audio.cpp
            CallRecFix.cpp
            fake_dlfcn.c
            main.h
            )

# Include libraries needed for callrecfix lib
target_link_libraries(callrecfix
                      android
                      log)
