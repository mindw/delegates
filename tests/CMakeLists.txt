
include_directories(${CMAKE_SOURCE_DIR}/include)

# make project/target
add_executable(DelegateTest DelegateTests.cpp)
add_test(NAME DelegateTest COMMAND $<TARGET_FILE:DelegateTest>)

add_executable(ClosureTest ClosureTests.cpp)
add_test(NAME ClosureTest COMMAND $<TARGET_FILE:ClosureTest>)

add_executable(sample01 sample01.cpp)
add_test(NAME sample01 COMMAND $<TARGET_FILE:sample01>)
