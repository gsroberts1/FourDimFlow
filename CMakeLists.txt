cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(Angiogram)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/FourDimFlow")
set(EXTENSION_CATEGORY "FourDimFlow")
set(EXTENSION_CONTRIBUTORS "Grant Roberts (NeoSoft, LLC)")
set(EXTENSION_DESCRIPTION "This is an example of a simple extension")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/FourDimFlow.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/FourDimFlow/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(Angiogram)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
