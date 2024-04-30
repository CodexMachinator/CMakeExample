set(BINARY_NAME ${CMAKE_PROJECT_NAME}_tst)

# set TST_SOURCES to all .h and .cpp files in tst folder
file(GLOB_RECURSE
	 TST_SOURCES
	 LIST_DIRECTORIES false
	 *.h *.cpp)

add_executable(${BINARY_NAME} ${TST_SOURCES})
target_link_libraries(${BINARY_NAME} PUBLIC ${CMAKE_PROJECT_NAME}_lib gtest)

add_test(NAME ${BINARY_NAME} COMMAND ${BINARY_NAME})

