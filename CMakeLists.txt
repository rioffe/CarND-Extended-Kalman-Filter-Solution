project(ExtendedKF)

cmake_minimum_required (VERSION 3.5)

add_definitions(-std=c++0x)

set(sources
    src/FusionEKF.cpp
    src/kalman_filter.cpp
    src/main.cpp
    src/tools.cpp)

set(headers
    src/FusionEKF.h  
	src/ground_truth_package.h  
	src/kalman_filter.h  
	src/measurement_package.h  
	src/tools.h)

add_executable(ExtendedKF ${sources} ${headers})
