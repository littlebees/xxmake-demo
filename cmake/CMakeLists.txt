cmake_minimum_required (VERSION 3.16)
project(main CXX)
include_directories( ${CMAKE_CURRENT_SOURCE_DIR} )
link_directories( ${CMAKE_CURRENT_SOURCE_DIR} )
set(main_SOURCES
    main.cpp
    sta.cpp
)
add_library(dyn
	    SHARED
	    dyn.cpp
)
set(main_LIBS
    dyn
)
add_executable( ${PROJECT_NAME} ${main_SOURCES} )
target_link_libraries( ${PROJECT_NAME} ${main_LIBS} )
