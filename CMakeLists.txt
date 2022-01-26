cmake_minimum_required(VERSION 3.16)
project(eigen_example)

list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake )

# external dependencies
include(CPM)
CPMAddPackage(
  NAME Eigen
  GIT_REPOSITORY https://gitlab.com/libeigen/eigen
  GIT_TAG 3.4
)

add_subdirectory(hello_world)