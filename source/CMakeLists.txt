set( CMAKE_CXX_STANDARD 17 )
set( CMAKE_CXX_STANDARD_REQUIRED ON )
set( CMAKE_CXX_EXTENSIONS OFF )

add_executable( ${SON8PROJ} )
target_sources( ${SON8PROJ} PRIVATE
    main.cxx
)
