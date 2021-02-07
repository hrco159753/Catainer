cmake_minimum_required(VERSION 3.17.3)

add_executable(hello_world_test_exe main.cpp)
target_link_libraries(hello_world_test_exe PRIVATE ${CATAINER_LIBRARY_NAMESPACE}::${CATAINER_LIBRARY_NAME})
add_test(hello_world_test hello_world_test_exe)