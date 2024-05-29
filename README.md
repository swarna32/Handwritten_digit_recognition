# Handwritten Digit Recognition


## Overview
This project implements a system for recognizing handwritten digits using image processing techniques with OpenCV. The system compares a test image with candidate images to find the closest matching digit based on normalized cross-correlation.

## Dataset
- **Candidate Images**: A set of images representing the digits 0-9.
- **Test Image**: An image containing handwritten digits to be recognized.

## Preprocessing and Feature Extraction
1. **Load Images**: Candidate and test images are loaded using OpenCV.
2. **Convert to Grayscale**: Images are converted to grayscale for processing.
3. **Apply Thresholding**: Adaptive thresholding is applied to binarize the images.
4. **Find Contours**: Contours are detected in the thresholded images to isolate individual digits.
5. **Resize and Normalize**: Detected digits are resized to 50x50 pixels and normalized.

## Recognition Process
1. **Extract Digit Contours**: For each candidate image, contours are found to isolate the digit.
2. **Resize Candidate Digit**: The isolated digit is resized to 50x50 pixels and normalized.
3. **Extract Test Digit Contours**: Similar preprocessing is applied to the test image to find digit contours.
4. **Calculate NCC**: Normalized Cross-Correlation (NCC) is calculated between the candidate digit and each digit in the test image to find the closest match.
5. **Display Results**: The closest matching digit from the candidate set is displayed alongside the test image with the matched digit highlighted.

## Results
The closest matching digit from the candidate set is displayed alongside the test image with the matched digit highlighted. This visualization helps in understanding the performance of the digit recognition system.

### Visualizations
- **Candidate Digit and Best Match**
  - ![Candidate Digit](https://i.ibb.co/q7NL1Gh/01.png)
