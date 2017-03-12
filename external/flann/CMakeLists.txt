
file(GLOB_RECURSE SOURCES flann_cpp.cpp lz4.c lz4hc.c)
add_library(flann STATIC ${SOURCES})









