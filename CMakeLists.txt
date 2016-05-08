cmake_minimum_required(VERSION 3.0)

project(http-parser)

add_library(${PROJECT_NAME} STATIC
  http_parser.c
  http_parser.h
)

target_include_directories(${PROJECT_NAME}
  PUBLIC
  ${CMAKE_CURRENT_SOURCE_DIR}
)
