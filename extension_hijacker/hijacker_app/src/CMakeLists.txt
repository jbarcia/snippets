cmake_minimum_required (VERSION 2.8)
project (ExtensionHijacker)

set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} /MT")

set (srcs
    main.cpp
    res_dropper.cpp
    ext_hijacker.cpp
)
set (hdrs
	resource.h
    res_dropper.h
    ext_hijacker.h
)

set (rsrc
    resource.rc
)

add_executable (ExtensionHijacker ${rsrc} ${hdrs} ${srcs})