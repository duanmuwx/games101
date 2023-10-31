cmake_minimum_required(VERSION 3.10)
project(EigenExample)

# 设置C++标准
set(CMAKE_CXX_STANDARD 11)

# 查找Eigen3库
find_package(Eigen3 REQUIRED)

# 添加可执行文件
add_executable(EigenExample main.cpp)

# 包含Eigen3的头文件目录
target_include_directories(EigenExample PRIVATE ${EIGEN3_INCLUDE_DIRS})
