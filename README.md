# Project README

## Project Overview
TVM(Tensor Virtual Machine) Model Loading, Compilation, and Optimization
This repository contains Python scripts for loading, compiling, tuning, and optimizing ONNX models using TVM (Apache TVM), an open-source deep learning compiler stack.
first install the requirements ``` pip install apache-tvm --pre ```

## load_tune.py
we are extracting the resnet onnx model from github link.
after are loading the model, compiling, and run by using tvm commands.

##optimizer.py
we are extracting the resnet onnx model from github link.
It loads the ONNX model, applies transformations and optimizations using TVM passes, and measures the performance.
The optimization includes auto-tuning the model for better performance on the target hardware.
It provides latency metrics for both optimized and unoptimized versions of the model.


