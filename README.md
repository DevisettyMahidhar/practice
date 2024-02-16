# Project README

## Project Overview
The project involves implementing convolutional, max pooling, ReLU, dense, flatten, and softmax layers in C++, along with cross-validation using PyTorch outputs. Additionally, two datasets, CIFAR and MNIST, have been implemented, along with unit layer tests.

## Contents of the Project Folder

### `build`
- Contains the build files of all the operators and utility functions along with CMake files.

### `configs`
- Contains JSON files holding information about layers, shapes, input paths, PyTorch outputs, CPP outputs, and other parameters.
  - `mnist.json`: Contains configurations for the MNIST dataset.
  - `cifar.json`: Contains configurations for the CIFAR dataset.
  - `unit_test.json`: Contains configurations for unit tests.

### `data`
- Contains data related to CIFAR, MNIST, and unit layer tests.
  - `cifar` and `mnist` subfolders:
    - `cpp_output`: Stores the C++ output.
    - `input`: Contains input files like bias and weight files for dense and convolutional layers.
    - `pyt_output`: Stores layer-wise output from PyTorch.
    - `input_file`: Additional input files.
  - `unit_layer_test` subfolder contains input data for unit layer testing.

### `include`
- Contains header files.

### `operators`
- Contains source code for various layers.
- `src`: Includes cpp files for convolution, apply ReLU, flatten, dense, softmax, and pooling.
- `include`: Includes header files.

### `report`
- Contains TXT files corresponding to CIFAR, MNIST datasets, and unit layer tests.
- TXT files store information such as the count of layers, layer names, executed functions, and pass/fail status.

### `src`
- Includes the main.cpp file.

### `utilities`
- Additional subfolders for utility functions.
- `include`: Contains .hpp and .h files for reading JSON and NPY files.
- `src`: Includes source files for comparing vectors.

## OS, Tools, and Versions Used
- **OS**: Microsoft Windows with Linux distribution installed through Windows Subsystem for Linux (WSL).
- **Tools**: Visual Studio Code for code editing, Git for version control, CMake for build management, g++ for compiling C++ code, and gdb for debugging.
- **Versions**: CMake version 3.0.

## Build/Compile and Run Instructions
1. Open your terminal and navigate to the project directory.
2. Run the following commands:
   ```bash
   cmake -S . -B build
   cd build
   make
   ./MyProject
