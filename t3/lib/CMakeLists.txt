set(LIBHELLO_SRC hello.c)
add_library(hello SHARED ${LIBHELLO_SRC})
set(LIBRARY_OUTPUT_PATH /home/kiki/github/qt/cmake-demo/t3/cbuild/depends)