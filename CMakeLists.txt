cmake_minimum_required(VERSION 2.8.9)

project(MultiResolutionAffineRegistration)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://wiki.slicer.org/slicerWiki/index.php/Documentation/Nightly/Modules/MultiResolutionAffineRegistration")
set(EXTENSION_CATEGORY "Legacy.Registration")
set(EXTENSION_CONTRIBUTORS "Casey B Goodlett (Utah)")
set(EXTENSION_DESCRIPTION "Provides affine registration using multiple resolution levels and decomposed affine transforms.")
set(EXTENSION_ICONURL "")
set(EXTENSION_SCREENSHOTURLS "")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(MultiResolutionAffineRegistration)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
