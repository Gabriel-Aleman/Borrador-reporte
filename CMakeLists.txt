cmake_minimum_required(VERSION 3.10)
project(examen VERSION 1.0
              DESCRIPTION "Proyecto"
              LANGUAGES C)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ./bin)

set(sources
  src/main.c
  src/menu.c
  src/display_data.c
  src/dynamic_memory.c
  src/file_management.c
  src/sort.c)

include_directories("${PROJECT_SOURCE_DIR}/include")

add_executable(proyecto ${sources})

install (TARGETS proyecto DESTINATION bin)