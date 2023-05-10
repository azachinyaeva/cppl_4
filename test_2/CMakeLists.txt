cmake_minimum_required (VERSION 3.8)
project ("test_2")
add_executable (test_2 "test_2.cpp" )

add_subdirectory(Catch2 Catch2-build)
target_link_libraries(test_2 PRIVATE Catch2::Catch2)
