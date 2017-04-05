cmake_minimum_required(VERSION 3.6)
project(host)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    apdu_split.c
    apdu_split.h
    main.c
    Makefile
    simtrace.h
        libusb.h
    simtrace_usb.h
        )

add_executable(host ${SOURCE_FILES})