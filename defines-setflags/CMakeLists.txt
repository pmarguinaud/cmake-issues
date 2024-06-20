cmake_minimum_required (VERSION 3.22)

project (cmkpack LANGUAGES Fortran)

set (CMAKE_Fortran_FLAGS "-DDEF")

add_library (
  AB
  OBJECT
  a.F90
  b.F90
)

