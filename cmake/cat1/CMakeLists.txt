cmake_minimum_required(VERSION 3.10)
project(SimpleCppProject)

file(GLOB SOURCES "src/*.cpp")
file(GLOB HEADERS "include/*.h")

add_executable(MyApp ${SOURCES} ${HEADERS})

target_include_directories(MyApp PUBLIC ${PROJECT_SOURCE_DIR}/include)
