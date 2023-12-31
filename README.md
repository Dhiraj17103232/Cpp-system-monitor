# Cpp-System-Monitor
A system monitoring tool similar to htop, written in C++.  

![Starting System Monitor](images/monitor.png)

## ncurses
[ncurses](https://www.gnu.org/software/ncurses/) is a library that facilitates text-based graphical output in the terminal. This project relies on ncurses for display output.

Install ncurses within your Linux environment:  
Debian based system: `sudo apt install libncurses5-dev libncursesw5-dev`  
Arch based systems: `sudo pacman -S ncurses`  

## Make
This project uses [Make](https://www.gnu.org/software/make/). The Makefile has four targets:
* `build` compiles the source code and generates an executable
* `format` applies [ClangFormat](https://clang.llvm.org/docs/ClangFormat.html) to style the source code
* `debug` compiles the source code and generates an executable, including debugging symbols
* `clean` deletes the `build/` directory, including all of the build artifacts

## Build Instructions

1. Clone the project repository: `git clone https://github.com/utkarsh914/Cpp-system-monitor.git`

2. Build the project: `make build`

3. Run the resulting executable: `./build/monitor`
