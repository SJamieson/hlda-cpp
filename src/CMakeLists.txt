find_package(GSL)
include_directories(${GSL_INCLUDE_DIRS})

file(GLOB SRC_FILES "*.cc")
add_executable(${PROJECT_NAME} "${SRC_FILES}")
target_link_libraries(${PROJECT_NAME} ${GSL_LIBRARIES})
