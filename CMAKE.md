## 官方Tutorial
[CMake Tutorial - CMake 3.19.2 Documentation](https://cmake.org/cmake/help/latest/guide/tutorial/index.html#a-basic-starting-point-step-1)

## Easy Version
```CMake
# cmake version
cmake_minimum_required (VERSION 2.6)
# set the project name, name -> usually executable in the test
project(Tutorial)
# specify the C++ standard
set(CMAKE_CXX_STANDARD 14)/ADD_DEFINITIONS(-std=c++14)
set(CMAKE_CXX_STANDARD_REQUIRED True)
# add the executable
add_executable(Tutorial tutorial.cxx)
```

## Build and Test
```bash
mkdir -p build
cd build
cmake -DCMAKE_INSTALL_PREFIX=$INSTALL_DIR -DCMAKE_BUILD_TYPE=$CMAKE_BUILD_TYPE ..
make install
Tutorial xxx -> 用来测试
```

## Add Library
Library的名字一般都是已经帮你设好的，有${xxx_src}/也有xxxx::xxxx

```CMake
target_link_library()
add_dependencies()
link_directories()
include_directories()
```

## Tips
- 加入这个文件夹，一起编译/或者跑cmake
    ```CMake 
    ADD_SUBDIRECTORY(src)
    ```
- Include all the includes files
    ```CMake 
    INCLUDE_DIRECTORIES(include)
    ```
- if 判断
    ```CMake 
    if()
    endif()
    ```
- 表示一个变量的
    ```CMake 
    ${}
    ```
- 设置变量alias，变量属性
    ```CMAKE 
    SET(VARIABLE_NAME 值/ON/String)
    ```
- 加入list
    ```CMake 
    list(APPEND list_name append_value)
    ```
- print message
    ```CMake 
    MESSAGE(STATUS “A_B_C is : ${A_B_C}”)
    ```
- 看到variable的值（一定要现有cmake的文件在）
    ```CMake 
    ccmake .. ，才可以看到这次cmake的一些variable的值
    ```
