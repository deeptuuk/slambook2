cmake_minimum_required( VERSION 2.8)

project( useEigen3 )

include_directories( "/usr/include/eigen3" )

add_executable( useEigen3 eigenMatrix.cpp )
