# STL tool

A little C++ programm that reads and writes ASCII or Binary STL ("STereoLithography" or "Standard Triangle Language").

## What's in

* `triangle.hpp` provides a basic Triangle class
* `STL_tool.hpp` provides the read and write routines for .stl files

If you want to create a .stl file you need to fill a `std::vector<Triangle>` with the surface traingulation and pass it to a `Write*` routine of the STL_tool class.

Reading a .stl file returns a `std::vector<Triangle>`.

* `surface_creation.hpp` is a sample collection to create `std::vector<Triangle>` which can then be written to .stl on viewed in e.g. [Paraview](https://www.paraview.org).