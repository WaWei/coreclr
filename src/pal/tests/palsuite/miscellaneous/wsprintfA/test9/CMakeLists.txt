cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test.cpp
)

add_executable(paltest_wsprintfa_test9
  ${SOURCES}
)

add_dependencies(paltest_wsprintfa_test9 coreclrpal)

target_link_libraries(paltest_wsprintfa_test9
  pthread
  m
  coreclrpal
)
