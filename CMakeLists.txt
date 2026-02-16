cmake_minimum_required (VERSION 3.5) 
project (ORDERBOOK)

# Initialize CXXFLAGS.
set(CMAKE_CXX_FLAGS "-Wall -Wno-missing-braces -std=c++11")
set(CMAKE_BUILD_TYPE Release)

set(TEST_SRCS engine.cpp test.cpp)
set(SCORE_SRCS engine.cpp score.cpp)

add_executable(test ${TEST_SRCS})
add_executable(score ${SCORE_SRCS})