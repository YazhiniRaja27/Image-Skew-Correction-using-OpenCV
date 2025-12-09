# Image Deskewing with OpenCV

## Project Description
This project demonstrates how to detect and correct skew in an image using OpenCV in Python. It involves loading a grayscale image, applying image preprocessing techniques such as binarization and Canny edge detection, and then utilizing the Hough Line Transform to identify lines within the image. From the detected lines, the skew angle of the image is calculated. Finally, the image is rotated by the calculated skew angle to produce a corrected, deskewed image. The original and corrected images are displayed for visual comparison.

## Features
- Load grayscale images.
- Preprocess images using binarization and Canny edge detection.
- Detect lines using Hough Line Transform.
- Calculate the skew angle of the image.
- Rotate the image to correct the skew.
- Display original and corrected images for comparison.

## Requirements
- Python 3.x
- OpenCV (`opencv-python`)
- NumPy (`numpy`)

These can be installed using pip:
```bash
pip install opencv-python numpy
```

## Usage
1.  **Mount Google Drive**: Ensure your Google Drive is mounted to `/content/drive` as shown in the notebook to access your image files.
2.  **Image Path**: Place your skewed image file (e.g., `skew.jpg`) in your Google Drive and update the `image_path` variable in the code cell to point to its location.
    ```python
    image_path = '/content/drive/MyDrive/skew.jpg'
    ```
3.  **Run the Notebook**: Execute all cells in the Colab notebook. The script will:
    - Load and display the original skewed image.
    - Process the image to detect its skew angle.
    - Rotate the image to correct the skew.
    - Display the corrected, deskewed image.

## Example Output
The notebook will output two images: the original input image with detected skew, and the rotated image where the skew has been corrected. It will also print the detected skew angle in degrees.

