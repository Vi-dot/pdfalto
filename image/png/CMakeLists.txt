cmake_minimum_required(VERSION 3.5+)
project(png)

set(CMAKE_CXX_STANDARD 98)

set(PNG_SOURCE_FILES
        png.c
        png.h
        pngconf.h
        pngerror.c
        pnggccrd.c
        pngget.c
        pngmem.c
        pngpread.c
        pngread.c
        pngrio.c
        pngrtran.c
        pngrutil.c
        pngset.c
        pngtrans.c
        pngvcrd.c
        pngwio.c
        pngwrite.c
        pngwtran.c
        pngwutil.c
        )

add_library(${PROJECT_NAME} SHARED ${PNG_SOURCE_FILES})
target_link_libraries(png zlib)