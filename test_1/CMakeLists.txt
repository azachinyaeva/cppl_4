cmake_minimum_required (VERSION 3.8)
project ("test_1")
add_executable (test_1 "test_1.cpp" )


add_subdirectory(Catch2 Catch2-build)
target_link_libraries(test_1 PRIVATE Catch2::Catch2)