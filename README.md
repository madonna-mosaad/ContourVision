# ContourVision - Edge and Boundary Detection

## Project Overview
This project implements the Hough Transform for detecting lines, circles, and ellipses, alongside the Active Contour Model (Snake) for dynamic contour modeling. All algorithms are custom-written in Python without relying on OpenCV's built-in functions. The project includes a PyQt-based graphical user interface (GUI) for interactive parameter adjustments and real-time visualization of results.

---

## Features

### 1. **Edge Detection Using Canny**
- **Parameters**:
  - Gaussian Kernel Size
  - Sigma (σ)
  - High and Low Thresholds
  - Sobel Kernel Size
  - Gradient Method (Manhattan or Euclidean Distance)
- **User Interaction**: Adjust parameters via the GUI and click "Apply" to update results.
- **Observation**: The choice of gradient method and threshold settings significantly impacts edge detection quality.
![image](https://github.com/user-attachments/assets/d8c739ae-b6b1-43e5-80dd-4f208cb59d4c)

### 2. **Shape Detection (Lines, Circles, Ellipses)**
- **Parameters**:
  - Single Threshold for sensitivity control.
- **User Interaction**: Modify the threshold and observe real-time changes in shape detection.
- **Observation**: Proper threshold balancing is crucial for minimizing false positives in complex images.
- **Line Detection**
![image](https://github.com/user-attachments/assets/de14684e-76ee-4bd1-8974-b7bd0381f3ee)
- **Cicle Detection**
  ![image](https://github.com/user-attachments/assets/ee8de06c-cfc1-4bb1-bd4b-a81714920de0)
- **Ellipse Detection**
- ![image](https://github.com/user-attachments/assets/f64fca35-4e3c-4211-a313-3452b9b482d3)


### 3. **Active Contour Model (Snake)**
- **Parameters**:
  - Number of Points
  - Weights (`W_Line`, `W_Edge`, Alpha, Beta, Gamma)
  - Number of Iterations
- **User Interaction**: Adjust parameters and click "Apply Contour" to visualize the evolving snake.
- **Observation**: Calibration of weights and points is essential for accurate contour modeling.
- **Tooth Contouring**
- ![image](https://github.com/user-attachments/assets/5503db4a-3eb6-4196-8195-409fd9daf48c)
- **Apple Contouring**
- ![image](https://github.com/user-attachments/assets/8fe4237d-504f-467f-8c99-12ca1184d953)


---

## Installation
1. **Prerequisites**:
   - Python 3.9
   - Libraries: PyQt5, NumPy, Matplotlib, SciPy
2. **Clone Project**:
   ```bash
   git clone https://github.com/nancymahmoud1/ContourVision.git
