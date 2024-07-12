cmake_minimum_required(VERSION 3.14)

project(pdfium_library VERSION 2.0.1 LANGUAGES CXX)

add_library(pdfium SHARED
  "pdfium_interop.cpp"
)

set_target_properties(pdfium PROPERTIES
  OUTPUT_NAME "pdfium"
)

target_compile_definitions(pdfium PUBLIC DART_SHARED_LIB)