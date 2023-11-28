cmake_minimum_required(VERSION 3.26)
project(CFI_2)

include(FetchContent)

FetchContent_Declare(
        googletest
        GIT_REPOSITORY https://github.com/dropbox/json11.git
        GIT_TAG v3.7.3
)

set(CMAKE_CXX_STANDARD 14)

add_executable(CFI_2
        main.cpp)


target_link_libraries(CFI_2 PUBLIC json11)
