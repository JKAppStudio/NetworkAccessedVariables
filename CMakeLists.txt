#
#Athor: Evgeny Krivoshein
#
########################################################################
# Project setup
########################################################################
cmake_minimum_required(VERSION 3.10)
project(NAV CXX)

########################################################################
# Add required cmake modules paths
########################################################################
list(INSERT CMAKE_MODULE_PATH 0 ${CMAKE_SOURCE_DIR}/ClientServerNetwork)
set(CSNET_SOURCE_DIR ${CMAKE_SOURCE_DIR}/ClientServerNetwork)

########################################################################
# Set C++ standatd
########################################################################
set(CMAKE_CXX_STANDARD 17)

########################################################################
# Include cmake modules
########################################################################
include(csNet)

########################################################################
# Local Include Dir
########################################################################
include_directories(${CMAKE_BINARY_DIR}/include)
include_directories(${CMAKE_SOURCE_DIR}/include)

