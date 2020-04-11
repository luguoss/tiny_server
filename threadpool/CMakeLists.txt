# 声明要求的cmake最低版本
cmake_minimum_required( VERSION 2.8 )
 
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -pthread -Wl,--no-as-needed")




# 声明一个cmake工程
project( threadpool_test )

# 头文件
include_directories(
    ${CMAKE_CURRENT_LIST_DIR}/inc/
)

link_libraries(

)


add_executable(threadpool_test ${CMAKE_CURRENT_LIST_DIR}/src/ThreadPool.cpp)    