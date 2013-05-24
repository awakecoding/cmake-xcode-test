
cmake_minimum_required(VERSION 2.8)

project(X C)

set(CMAKE_COLOR_MAKEFILE ON)

include(CheckIncludeFiles)
include(CheckLibraryExists)
include(CheckStructHasMember)
include(CMakeDetermineSystem)
include(FindPkgConfig)
include(TestBigEndian)
include(FeatureSummary)
include(CheckCCompilerFlag)
include(GNUInstallDirs)

add_subdirectory(C)
add_subdirectory(App)
