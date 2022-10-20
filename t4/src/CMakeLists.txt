add_executable(main main.c) # NOTE: put this line behind link_directories
find_path(helloHeader hello.h)
if(helloHeader)
include_directories(${helloHeader})
endif(helloHeader)
find_library(libhello hello /tmp/lib)
target_link_libraries(main ${libhello})