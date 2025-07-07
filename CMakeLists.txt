cmake_minimum_required(VERSION 3.10)
project(nrlmsise-00 VERSION 2.0)

set(CMAKE_C_STANDARD 99)

add_compile_options(
    -O2
    -fPIC
)

include_directories(
    ${PROJECT_SOURCE_DIR}/include
)

add_library(nrlmsise-00 SHARED
    src/nrlmsise-00.c
    src/nrlmsise-00_data.c
)

target_link_libraries(nrlmsise-00 m)

add_executable(nrlmsise-00_test
    test/nrlmsise-00_test.c
)

target_link_libraries(nrlmsise-00_test nrlmsise-00)


