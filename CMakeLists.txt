cmake_minimum_required(VERSION 3.4)

project(ClusteringLib)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

# Options
option(BUILD_TESTS "Build library tests")
option(BUILD_EXAMPLES "Build library usage examples")



include(DownloadProject.cmake)

# External projects 
add_subdirectory(external)

if(BUILD_EXAMPLES)
	add_subdirectory(examples)
endif()


if(BUILD_TESTS)
	include(CTest)
	add_subdirectory(tests)
endif()