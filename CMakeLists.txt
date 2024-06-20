cmake_minimum_required (VERSION 3.22)

project (cmkpack LANGUAGES Fortran)

set_source_files_properties (
  src_mse_module_mode_read_surf_lfi.F90
  PROPERTIES
  COMPILE_DEFINITIONS
  SFX_LFI
)

add_library (
  IAL
  OBJECT
  src_mse_module_mode_read_surf_lfi.F90
  src_surfex_OFFLIN_modi_fmread.F90
)

