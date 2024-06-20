cmake_minimum_required (VERSION 3.22)

project (cmkpack LANGUAGES Fortran)

add_library (
  AB
  OBJECT
  a.F90
  b.F90
)

set_target_properties (
  AB
  PROPERTIES
  COMPILE_DEFINITIONS
  DEF
)
