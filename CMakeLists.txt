cmake_minimum_required(VERSION 3.20)

set (PostgreSQL_ADDITIONAL_VERSIONS "16")

project (PqxxProject2)

add_subdirectory("C:\\Users\\Kir17\\source\\repos\\libpqxx-7.9.1" pqxx-build)


add_executable( PqxxProject2 main.cpp)

target_compile_features (PqxxProject2 PRIVATE cxx_std_17)

target_link_libraries (PqxxProject2 pqxx) 