project(xxhash)

add_library(xxhash xxhash.h xxhash.c)

add_executable(xxhash-bench bench.c)
target_link_libraries(xxhash-bench xxhash)
