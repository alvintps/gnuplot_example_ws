# Gnuplot Example Workspace

Gnuplot interface in ANSI C by Nicolas Devillard.

## Setup on Linux/Ubuntu

#### Install gnuplot
```
$ sudo apt-get update
$ sudo apt-get install gnuplot
```

#### Make
```
$ mkdir build
$ cd build
$ cmake ..
$ make
```

## Setup on Windows

#### Setup build environment
1. Configure Visual Studio Code to use the GCC C++ compiler (g++) and GDB debugger from mingw-w64: https://code.visualstudio.com/docs/cpp/config-mingw
2. Install [CMake Tools extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools&ssr=false#overview).

#### Install gnuplot
Download and install the appropriate Windows 64bit binary self-installer from: https://sourceforge.net/projects/gnuplot/files/gnuplot/

#### Make
1. Create an empty directory in the workspace and rename it as `build`.
2. Open the Command Palette (`Ctrl+Shift+P`) and run the <b>CMake: Configure</b> command.
3. Open the Command Palette (`Ctrl+Shift+P`) and run the <b>CMake: Build</b> command.
