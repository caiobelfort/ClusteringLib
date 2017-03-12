file(GLOB_RECURSE SOURCES *.h *.hxx *.hpp)
add_library(Eigen ${SOURCES})
set_target_properties(Eigen PROPERTIES LINKER_LANGUAGE CXX)