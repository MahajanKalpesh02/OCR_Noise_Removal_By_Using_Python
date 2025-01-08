# Noise Removal Techniques in Image Processing

This project demonstrates various techniques for noise removal in image processing using Python. The techniques covered include Gaussian Blur, Median Filtering, and Bilateral Filtering, which are commonly used to reduce noise while preserving important features in images.

---

## Requirements

Before running the scripts, ensure you have the required libraries installed. Below is a list of the dependencies with a brief description and installation commands.

### Python Libraries

1. **OpenCV**:
   - OpenCV is an open-source library for computer vision and image processing tasks. It provides functions for noise removal and other image manipulations.
   - Installation Command:
     ```bash
     pip install opencv-python
     ```

2. **NumPy**:
   - NumPy is a fundamental library for numerical computations in Python. It is often used for handling arrays and performing mathematical operations on images.
   - Installation Command:
     ```bash
     pip install numpy
     ```

3. **matplotlib**:
   - matplotlib is used for visualizing and plotting the images before and after applying noise removal techniques.
   - Installation Command:
     ```bash
     pip install matplotlib
     ```

---

## Techniques Included

### 1. Gaussian Blur
- Applies a Gaussian function to smooth the image, reducing noise and detail.
- Usage Example in Script:
  ```python
  blurred = cv2.GaussianBlur(image, (5, 5), 0)
  ```

### 2. Median Filtering
- Replaces each pixel's value with the median value of its neighbors, effective for removing salt-and-pepper noise.
- Usage Example in Script:
  ```python
  median = cv2.medianBlur(image, 5)
  ```

### 3. Bilateral Filtering
- Reduces noise while preserving edges by considering both spatial and intensity differences.
- Usage Example in Script:
  ```python
  bilateral = cv2.bilateralFilter(image, 9, 75, 75)
  ```

---

## Usage Instructions

1. Place your image file in the project directory and update the `image_path` variable in the script with your image's filename.

2. Run the script using:
   ```bash
   python script_name.py
   ```
   Replace `script_name.py` with the actual name of your Python file.

3. The script will:
   - Load the input image.
   - Apply noise removal techniques (Gaussian Blur, Median Filtering, and Bilateral Filtering).
   - Display the original and processed images side by side for comparison.

---

## Output

- Processed images showing the effect of each noise removal technique applied to the input image.

---

## Notes

- Experiment with different kernel sizes and parameters to achieve optimal results for your images.
- Use high-quality input images to better observe the effects of noise removal techniques.

---
---

## License

This project is licensed under the MIT License. Feel free to use and modify the code.

---

### Contribution

If you want to contribute, feel free to submit a pull request or report issues.

---

### Installation Commands Summary

```bash
pip install opencv-python
pip install numpy
pip install matplotlib
```

