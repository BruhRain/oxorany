cmake_minimum_required(VERSION 3.20)
project(oxorany)
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(SOURCES
  ${PROJECT_SOURCE_DIR}/source/oxorany.cpp
  ${PROJECT_SOURCE_DIR}/source/oxorany.h
  ${PROJECT_SOURCE_DIR}/source/oxorany_include.h)

add_library(${PROJECT_NAME} STATIC ${SOURCES})
target_include_directories(${PROJECT_NAME} PRIVATE
  ${PROJECT_SOURCE_DIR}/source)
