cmake_minimum_required(VERSION 2.8)
project(delegates CXX)

include(CTest)

if(BUILD_TESTING)
    add_subdirectory(tests)
endif()

# includes
install(
    FILES include/Closure.h  include/Delegate.h  include/Delegate01.h
    DESTINATION include/delegates
    )
