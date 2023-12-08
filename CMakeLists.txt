cmake_minimum_required(VERSION 3.10)

set(CMAKE_EXPORT_COMPILE_COMMANDS on)

project(vc_fmt_test CXX)

find_package(fmt CONFIG REQUIRED)

add_executable(fmt_test src/main.cxx)

target_link_libraries(fmt_test PRIVATE fmt::fmt)
