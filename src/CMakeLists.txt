# set SRC_SOURCES to all .h and .cpp files in tst folder
file(GLOB_RECURSE
	 SRC_SOURCES
	 LIST_DIRECTORIES false
	 *.h *.cpp)

add_executable(${CMAKE_PROJECT_NAME}_run ${SRC_SOURCES})

add_library(${CMAKE_PROJECT_NAME}_lib SHARED ${SRC_SOURCES})

