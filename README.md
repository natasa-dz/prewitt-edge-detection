# Prewitt Edge Detection

This project implements edge detection using the **Prewitt operator** on grayscale images. The program supports both **sequential** and **parallel** implementations using **OneTBB**, offering performance improvements for larger images and different filter sizes.

### Features:
- **Prewitt Operator** for detecting horizontal and vertical edges.
- **Thresholding**: Post-processes edge-detected images with a global threshold of 128.
- **Parallel Processing**: Utilizes **OneTBB** for faster execution on multi-core systems.
- Adjustable **filter size** (3x3, 5x5, 7x7) and **neighborhood search** for enhanced edge detection.

### Requirements:
- **C++** compiler (GCC, Clang, etc.)
- **EasyBMP** library (provided)
- **OneTBB** for parallelization

### Usage:

1. **Compile the code**:
   ```bash
   g++ -o edge_detection edge_detection.cpp -std=c++17 -ltbb


2. **Run the program**:
   ```bash
   ./edge_detection <input_image.bmp> <output_image.bmp> <filter_size>

3. **Example**:
   ```bash
   ./edge_detection input.bmp output.bmp 3
