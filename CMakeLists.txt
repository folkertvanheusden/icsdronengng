project(Dog)
cmake_minimum_required(VERSION 3.6)

add_definitions("-Wall")

#set(CMAKE_BUILD_TYPE Release)
set(CMAKE_BUILD_TYPE RelWithDebInfo)
#set(CMAKE_BUILD_TYPE Debug)

cmake_policy(SET CMP0069 NEW)
set(CMAKE_POLICY_DEFAULT_CMP0069 NEW)
set(CMAKE_INTERPROCEDURAL_OPTIMIZATION TRUE)

add_executable(
  icsdroneng
  argparser.c
  board.c
  computer.c
  fics.c
  main.c
  marker.c
  net.c
  polyglot.c
  proxy.c
  sched.c
  utils.c
)
