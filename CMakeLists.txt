cmake_minimum_required(VERSION 3.13.4)

project(MyFirstSlicerExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/MyFirstSlicerExtension")
set(EXTENSION_CATEGORY "Learning")
set(EXTENSION_CONTRIBUTORS "Vinith Kugathasan (UoM)")
set(EXTENSION_DESCRIPTION "This is for Medical Image Processing assignment")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/MyFirstSlicerExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstSlicerExtension/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
