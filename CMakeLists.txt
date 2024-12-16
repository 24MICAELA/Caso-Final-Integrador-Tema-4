cmake_minimum_required(VERSION 3.29)
project(Caso_Final_Integrador_Tema_4)

set(CMAKE_CXX_STANDARD 14)

add_executable(Caso_Final_Integrador_Tema_4
    main.cpp
        tests/tests.cpp
        tests/tests.h
        tiny-lisp/tinylisp.cpp
)
