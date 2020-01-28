# Static Library Linking Example

This example is my attempt to demonstrate how to link a statically 
built C++ library to a separate project.

There are generally two approaches to linking C++ library:

1. Shared library
2. Static library

The Shared library approach requires installing the library into the
system which may not always be desireable, and updating linker 
definitions (LD... more on this later). This is OK if working in a 
docker or vitrual environment, however, sometimes it may not be
benefivial to install a library into the system.
