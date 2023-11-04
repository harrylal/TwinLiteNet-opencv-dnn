
<div align="center">

# TwinLiteNet ONNX Model Inference with OpenCV DNN

</div>

This repository contains a C++ implementation for performing inference with the state-of-the-art [TwinLiteNet model](https://github.com/chequanghuy/TwinLiteNet) using OpenCV's DNN module. TwinLiteNet is a cutting-edge lane detection and drivable area segmentation model. This implementation offers support for both CUDA and CPU inference through build options.

<div align="center">
<img src="assets/results.jpg" alt="Detection Results">
</div>

<br>

## Acknowledgment

I would like to express sincere gratitude to the creators of the [TwinLiteNet model](https://github.com/chequanghuy/TwinLiteNet) for their remarkable work .Their open-source contribution has had a profound impact on the community and has paved the way for numerous applications in autonomous driving, robotics, and beyond.Thank you for your exceptional work.

## Prerequisites

- OpenCV 4.8 +

## Build Options

- **CUDA Inference:** To enable CUDA support for GPU acceleration, build with the `-DWITH_CUDA=ON` CMake option.
- **CPU Inference:** For CPU-based inference, no additional options are required.

## Usage

1. Clone this repository.
2. Build the project using CMake with your preferred build options.
```cpp
mkdir build
cd build
cmake  -DWITH_CUDA=ON ..
make -j8
```
4. Execute `./main` and Enjoy accurate lane detection and drivable area results!

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use it in both open-source and commercial applications.