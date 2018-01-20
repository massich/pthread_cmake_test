cmake_minimum_required (VERSION 3.2)
project (test_pthread)


find_package (Threads REQUIRED)
add_executable(xx pthread_create_cmake_test.c)

target_link_libraries(xx Threads::Threads)
