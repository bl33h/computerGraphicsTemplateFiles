# computerGraphicsTemplateFiles
This project contains the source code for a framebuffer implementation in C++. It allows you to manipulate and display colors on a virtual screen. It also provides functionality to clear the screen, set the current color, and store color values in a vector. This repository was made to use as a template for the different activities in the Computer Graphics course.

<p align="center">
  <br>
  <img src="https://res.cloudinary.com/practicaldev/image/fetch/s--K18o3cwe--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/r01ddc56dxmcjqpr7p1d.png" alt="pic" width="500">
  <br>
</p>
<p align="center" >
  <a href="#Files">Files</a> •
  <a href="#Features">Features</a> •
  <a href="#how-to-use">How To Use</a> 
</p>

## Files

- src: the file that implements de solution.
- CMakeLists.txt: the CMake configuration.

## Features
The main features of the application include:
- Framebuffer: The framebuffer.h file provides a framebuffer vector that represents the virtual screen. It is a 1-dimensional vector of Color objects, with dimensions defined by the SCREEN_WIDTH and SCREEN_HEIGHT constants.
- Color Manipulation: The colors.h file defines the Color struct, which represents an RGB color. It provides functionality to create colors, perform arithmetic operations (addition and multiplication), and clamp color values within a specified range.
- Clearing the Screen: The clear() function in framebuffer.h clears the framebuffer by filling it with the clearColor value. It utilizes the std::fill algorithm to efficiently set all elements of the vector.


## How To Use
To clone and run this application, you'll need [Git](https://git-scm.com), [CMake](https://cmake.org/download/) and a [C++ compiler](https://www.fdi.ucm.es/profesor/luis/fp/devtools/mingw.html) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/bl33h/computerGraphicsTemplateFiles

# Open the folder
$ cd src

# Run the app
$ g++ main.cpp -o framebuffer
$ ./framebuffer

# Build the app using CMake
$ cmake -G "Unix Makefiles" -S . -B build
$ cd build/
$ make
$ GAME.exe
```
