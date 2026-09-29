cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(HexaMesher)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/DomenicoRiggio/SlicerHexaMesher")
set(EXTENSION_CATEGORY "Utilities")
set(EXTENSION_CONTRIBUTORS "Domenico Riggio (Institute of Biomedical Engineering, KIT), Kimia Ghodousipour (Institute of Biomedical Engineering, KIT), Laura Lichtlein (Institute of Biomedical Engineering, KIT), Ciro Benito Raggio (Institute of Biomedical Engineering, KIT), Maria Francesca Spadea (Karlsruhe Institute of Technology, Germany)")
set(EXTENSION_DESCRIPTION "This extensions aims to transform models into hexahedron volumetric meshes.")
set(EXTENSION_ICONURL "https://raw.githubusercontent.com/DomenicoRiggio/SlicerHexaMesher/main/HexaMesher/Resources/Icons/HexaMesher.png")
set(EXTENSION_SCREENSHOTURLS "https://raw.githubusercontent.com/DomenicoRiggio/SlicerHexaMesher/main/HexaMesher/Resources/Icons/Examples.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(HexaMesher)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
