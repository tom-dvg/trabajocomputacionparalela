cmake_minimum_required(VERSION 3.10)

# Nombre del proyecto
project(Trabajo)

# Especificar la version de C++
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Encontrar la biblioteca OpenMP
find_package(OpenMP REQUIRED)

# Agregar el ejecutable
add_executable(mi_programa main.cpp)

# Enlazar OpenMP
target_link_libraries(mi_programa PUBLIC OpenMP::OpenMP_CXX)

