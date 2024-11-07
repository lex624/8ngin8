# 8ngin8
3D game engine

This project sets up a basic OpenGL environment in Windows using GLFW and GLAD. It displays an orange triangle using shaders to demonstrate a simple 3D graphics pipeline.

## Getting Started

These instructions will help you set up and run the project in Visual Studio Code on Windows.

### Prerequisites

Ensure you have the following installed on your system:
- **Git**: [Download Git](https://git-scm.com/downloads)
- **Visual Studio Code**: [Download VS Code](https://code.visualstudio.com/)
- **MinGW (Minimalist GNU for Windows)**: Install `gcc` and `g++` compilers.
  - You can use **MSYS2** to install MinGW if you don't have it. [Download MSYS2](https://www.msys2.org/)
  - **Installation Steps** for MSYS2:
    - Open MSYS2 and install the necessary packages:
      ```bash
      pacman -S mingw-w64-ucrt-x86_64-gcc mingw-w64-ucrt-x86_64-gdb
      ```
    - Add MinGW to your PATH, usually found at `C:\msys64\ucrt64\bin`.

### Project Setup

1. **Clone the Repository**:
   ```bash
   git clone <your-repo-url>
   cd <repository-name>

2. Install Dependencies:

Download the GLFW and GLAD libraries if they’re not included in the repository.
Place the following:
GLFW headers in include/GLFW
GLFW library file (libglfw3dll.a) in the lib folder.
glfw3.dll in the project root directory or where the executable will look for it.
GLAD should be similarly organized, with its headers in include/glad and its source file in src/glad.c.

3. Open in Visual Studio Code: Open the project directory in VS Code:

   ```bash
   code .

4. Configure VS Code for Building and Running:

Ensure .vscode/tasks.json is set up to build the project.
Make sure to adjust paths in tasks.json if necessary, especially to point to your g++ compiler in C:\msys64\ucrt64\bin.


Running the Project
	1. In Visual Studio Code, press Ctrl + Shift + B to build the project.
	2. After building, run the executable (cutable.exe) either through VS Code or by double-clicking it in the 	   project    directory.
	3. You should see a window displaying an orange triangle.

Project Structure
Additional Information
GLFW: https://www.glfw.org/
GLAD: https://glad.dav1d.de/
MSYS2: https://www.msys2.org/

Troubleshooting
Shader Compilation Errors: If you see errors related to shader compilation, ensure that vertexShader.glsl and fragmentShader.glsl files are present in the shaders/ directory.
Library Loading Issues: Make sure glfw3.dll is in the same directory as your executable or in a directory included in your system’s PATH.

License
This project is licensed under the MIT License - see the LICENSE file for details.















