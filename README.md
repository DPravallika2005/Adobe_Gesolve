# Curvetopia: A Journey into the World of Curves

## Overview

*Adobe Gensolve* is a project focused on the identification, regularization, and beautification of 2D curves. It explores a wide range of operations on curves such as regularization, symmetry detection, and completion of incomplete curves. The project is particularly useful for processing hand-drawn shapes and converting them into mathematically regularized forms.

## Project Objectives

Adobe Gensolve aims to process 2D curves by:
1. Regularizing curves to conform to specific geometric shapes.
2. Detecting symmetries within closed curves.
3. Completing curves that have been fragmented or partially occluded.

## Features

### Regularize Curves

This feature identifies regular geometric shapes in a given set of curves, such as straight lines, circles, ellipses, rectangles, polygons, and star shapes.

### Exploring Symmetry in Curves

The project includes functionality to detect reflection symmetries in closed shapes.

### Completing Incomplete Curves

Algorithms for completing curves that have gaps due to occlusion, considering smoothness, regularity, and symmetry.

## Installation

To run Adobe Gensolve locally, follow these steps:

1. Clone the repository:
   bash
   git clone https://github.com/your-username/adobe-gensolve.git
2. Navigate to the project directory:
   bash
   cd adobe-gensolve
3. Install the required dependencies:
   bash
   pip install -r requirements.txt

   
## Prerequisites
- Python 3.8 or higher
- NumPy
- OpenCV
- Matplotlib



## Usage

### 1. Regularizing Curves

        To regularize a set of curves, use the provided Python script:
         bash
          import numpy as np
          import matplotlib.pyplot as plt

        # Load your data
        data_XYs = np.genfromtxt('path_to_your/frag0.csv', delimiter=',')
        data_XY2s = np.genfromtxt('path_to_your/frag01_sol.csv', delimiter=',')

        # Run the regularization process
        # (The script processes and visualizes the regularized curves)

### 2. Symmetry Detection

       To detect symmetries within curves, use the count_symmetries function:
        ```python
        import cv2
        from symmetry_detection import count_symmetries

        image_path = 'path_to_your_image.png'
        symmetry_count = count_symmetries(image_path)
        print(f"The number of symmetries found: {symmetry_count}")

## Examples

### Visualization

The project includes several visualization scripts to display the processed curves:

- *Step-by-Step Plotting:* The first set of paths is plotted step-by-step.
- *Complete Set Plotting:* All paths from the first and second sets are plotted together.

### Symmetry Detection Example

The symmetry detection script reads an image file, identifies contours, and calculates the number of vertical and horizontal symmetries.

## Contributing

Contributions are welcome! If you have any ideas, suggestions, or issues, please feel free to submit a pull request or open an issue.

## Acknowledgments

- [OpenCV](https://opencv.org/) - For providing the tools for image processing.
- [NumPy](https://numpy.org/) - For numerical operations.
- [Matplotlib](https://matplotlib.org/) - For visualization capabilities.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
