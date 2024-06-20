cmake_minimum_required (VERSION 3.22)

project (cmkpack LANGUAGES Fortran)

set_source_files_properties (
  a.F90
  PROPERTIES
  COMPILE_DEFINITIONS
  SFX_LFI
)

add_library (
  IAL
  OBJECT
  a.F90
  b.F90
)

