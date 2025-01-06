---

# Face Detection using MTCNN

This repository demonstrates how to detect faces in images using the MTCNN (Multi-task Cascaded Convolutional Networks) model. The script processes a group photo, detects faces, and then draws red bounding boxes around the detected faces. The images are displayed and saved with the bounding boxes to visualize the results.

## Folder Structure

To make it easier to understand the repository structure, here's a breakdown of the contents:

```
/Face-Detection-MTCNN
│
├── assets/               # Folder containing the original and processed images
│   ├── image 1.jpg   # The original image of a group
│   └── download.jpg  # The image with red bounding boxes around detected faces
│
├── Face_Counting.ipynb       # Main script for face detection and image processing
├── requirements.txt      # Dependencies for the project
└── README.md             # This file, explaining how to use the repository
```

### `assets/` folder
- `image 1.jpg`: The original image of the group.
- `download.jpg`: The same image, but with red bounding boxes drawn around the detected faces.

### `Face_Counting.ipynb`
The Python script that loads an image, detects faces using MTCNN, and then visualizes the results by drawing bounding boxes around the detected faces. It uses OpenCV for image processing and Matplotlib for displaying the final image.

### `requirements.txt`
Contains a list of Python dependencies needed for the project:
- `opencv-python`
- `numpy`
- `matplotlib`
- `mtcnn`

## Installation

Before running the script, make sure to install the required dependencies. You can do this by running:

```
pip install -r requirements.txt
```

## Usage

1. **Place the image in the `assets/` folder:**  
   Put your image (e.g., a group photo) inside the `assets/` folder, or use the example image `group_photo.jpg`.

2. **Run the face detection script:**  
   Execute the script `detect_faces.py` to detect faces in the provided image and draw red bounding boxes around them.

   ```bash
   python detect_faces.py
   ```

3. **View the result:**  
   After running the script, the processed image with the detected faces and red bounding boxes will be displayed using Matplotlib. The output image will also be saved as `group_photo_with_faces.jpg` in the `assets/` folder.

## Example

Here is an example of how the images are processed:

- **Original Image:**

  ![Original Image](https://github.com/realaryagupta/MTCNN-Face-Detection/blob/master/assets/images%201.jpeg)

- **Processed Image (with red bounding boxes):**

  ![Processed Image](https://github.com/realaryagupta/MTCNN-Face-Detection/blob/master/assets/download.png)
