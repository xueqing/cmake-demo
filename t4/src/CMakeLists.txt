add_executable(main main.c) # NOTE: put this line behind link_directories
include_directories(BEFORE /tmp/include/hello)
find_library(libhello hello /tmp/lib)
target_link_libraries(main ${libhello})