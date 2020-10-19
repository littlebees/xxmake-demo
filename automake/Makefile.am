AUTOMAKE_OPTIONS=foreign  
# autoreconf complain, so add this line
ACLOCAL_AMFLAGS = -I m4
bin_PROGRAMS=main 
main_SOURCES=main.cpp sta.cpp 
include_HEADERS = sta.h dyn.h
lib_LTLIBRARIES = libdyn.la
libdyn_la_SOURCES = dyn.cpp
LDADD = libdyn.la
