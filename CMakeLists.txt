cmake_minimum_required(VERSION 2.6)

#include(log.cmake)

set(CMAKE_DEFS "-std=c++11 -fno-rtti -fno-threadsafe-statics -fvisibility-inlines-hidden")
#set(EXTRA_DEFS "-g -O2 -Wall -Wextra")
#set(EXTRA_DEFS "-Wall -Wextra -Wno-write-strings -Wno-unused-variable")
set(EXTRA_DEFS "-Wno-write-strings -Wno-unused-variable")

include_directories(${CMAKE_SOURCE_DIR}/include)


add_definitions(${CMAKE_DEFS})
add_definitions(${EXTRA_DEFS})

add_subdirectory(apps)
