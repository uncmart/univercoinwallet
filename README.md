**1. Clone wallet sources**

```
git clone https://github.com/uncmart/univercoinwallet
```

**2. Build**
### On ubuntu 14.04

```
mkdir build && cd build && cmake .. && make
```


### On Windows
Dependencies: MSVC 2017, CMake 3.10.2 or later, Boost 1.59, and Qt 5.9 or later. You may download them from:

MSVC 2017: http://www.microsoft.com/
CMake: http://www.cmake.org/
Boost: https://nchc.dl.sourceforge.net/project/boost/boost-binaries/1.59.0/boost_1_59_0-msvc-14.0-64.exe
Qt: https://www.qt.io/

To build, change to a directory where this file is located, set Qt PATH in CMakeLists.txt:
set (CMAKE_PREFIX_PATH "C:\\Qt\\5.9\\msvc2017_64")

and run theas commands: 
```
mkdir build
cd build
cmake -G "Visual Studio 15 Win64" ..
```

And then use MSVC 2017 open "karbowanec.sln", do Build.
Good luck!

fix encode problem On Windows:https://msdn.microsoft.com/en-us/library/mt708821.aspx
To set this compiler option in the Visual Studio development environment
Open the project Property Pages dialog box. For more information, see How to: Open Project Property Pages.

Expand the Configuration Properties, C/C++, Command Line folder.

In Advanced Options, add the /utf-8 option, and specify your preferred encoding.

Choose OK to save your changes.

