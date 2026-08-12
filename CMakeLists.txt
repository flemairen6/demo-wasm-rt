project(DemoWasmRt LANGUAGES CXX)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(demo-wasm-rt SHARED
    src/functions.cpp
    include/functions.hpp
)
target_include_directories(demo-wasm-rt PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/include)
