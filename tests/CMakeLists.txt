cmake_minimum_required(VERSION 2.8)

# set source/lib variables
set(delegates_sources DelegateTests.cpp)
set(closure_sources ClosureTests.cpp)
set(sample01_sources sample01.cpp)

include_directories( ../include)

# make project/target
project(delegates-tests CXX)
add_executable(DelegateTest ${delegates_sources})
add_executable(ClosureTest ${closure_sources})
add_executable(sample01 ${sample01_sources})
