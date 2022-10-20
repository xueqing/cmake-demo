include_directories(BEFORE /tmp/include/hello)
link_directories(/tmp/lib)
add_executable(main main.c) # NOTE: put this line behind link_directories
target_link_libraries(main hello)