cmake_minimum_required(VERSION 3.16)

include(lib/framework64/cmake/configure_platform.cmake REQUIRED)

if (FW64_PLATFORM_N64)
    project(spooky C)
else()
    project(spooky)
endif()

add_subdirectory(lib/framework64)
add_subdirectory(src)