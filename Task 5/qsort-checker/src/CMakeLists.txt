project(qsort-checker CXX)

set(CMAKE_CXX_FLAGS "-Wall -std=c++17")
set(CMAKE_CXX_FLAGS_DEBUG "-g")
set(CMAKE_CXX_FLAGS_RELEASE "-O2")

set(CMAKE_CXX_STANDARD_REQUIRED ON)

file(GLOB SRC "*.cc" "**/*.cc")
add_executable(qsort-checker ${SRC})

target_link_libraries(qsort-checker dl argument-parser)
