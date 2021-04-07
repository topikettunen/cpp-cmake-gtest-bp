set(BINARY ${CMAKE_PROJECT_NAME})

set(HEADERS base.h)
set(SOURCES main.cpp base.cpp)

# set(SUBPROJECT subproject)
# 
# add_subdirectory(${SUBPROJECT})

add_executable(${BINARY}_run ${SOURCES} ${HEADERS})
add_library(${BINARY}_lib STATIC ${SOURCES} ${HEADERS})

# target_link_libraries(${BINARY}_run ${BINARY}_${SUBPROJECT}_lib)
# target_link_libraries(${BINARY}_lib ${BINARY}_${SUBPROJECT}_lib)

# GoogleTest

# include(FetchContent)
# FetchContent_Declare(
#   googletest
#   GIT_REPOSITORY https://github.com/google/googletest.git
#   GIT_TAG        release-1.10.0)
# 
# set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
# set(BUILD_GMOCK OFF CACHE BOOL "" FORCE)
# set(BUILD_GTEST ON CACHE BOOL "" FORCE)
# 
# FetchContent_MakeAvailable(googletest)

# set(BINARY_TEST ${CMAKE_PROJECT_NAME}_test)
# 
# set(
#   SOURCES)
# 
# add_executable(${BINARY_TEST} ${SOURCES})
# 
# target_link_libraries(
#   ${BINARY_TEST}
#   PUBLIC
#   gtest_main
#   ${CMAKE_PROJECT_NAME}_lib)
# 
# add_test(
#   NAME ${BINARY_TEST}
#   COMMAND ${BINARY_TEST})
