cmake_minimum_required(VERSION 3.10)
project(ComplexCppProject)

file(GLOB SOURCES "src/*.cpp")
file(GLOB HEADERS "include/*.h")

find_package(Boost REQUIRED COMPONENTS filesystem system)

add_executable(MyApp ${SOURCES} ${HEADERS})

target_link_libraries(MyApp PRIVATE Boost::filesystem Boost::system)

target_include_directories(MyApp 
    PUBLIC 
        ${PROJECT_SOURCE_DIR}/include
    PRIVATE
        ${Boost_INCLUDE_DIRS}
)
