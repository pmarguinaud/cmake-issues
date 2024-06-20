cmake_minimum_required (VERSION 3.22)

project (cmkpack LANGUAGES Fortran)

set_source_files_properties (
  a.F90
  PROPERTIES
  COMPILE_DEFINITIONS
  DEF
)

add_library (
  AB
  OBJECT
  a.F90
  b.F90
)

