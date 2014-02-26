project(xxhash)

add_library(xxhash xxhash.h xxhash.c)

add_executable(xxhash-bench bench.c)
target_link_libraries(xxhash-bench xxhash)

install(TARGETS xxhash LIBRARY DESTINATION lib ARCHIVE DESTINATION lib)
install(FILES xxhash.h DESTINATION include)
