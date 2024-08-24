
# Estimation of Object Sizes in Images

This project aims to estimate the dimensions of objects within an image by utilizing a reference object with known size. Both the reference object and the target object must be on the same plane for accurate measurements. The project uses image processing techniques to perform this estimation.

![image](https://github.com/user-attachments/assets/0d828934-7c13-478b-bf4f-a037fd2fe4eb)
![image](https://github.com/user-attachments/assets/bd3168bf-3b56-46f1-828f-9e0350f0a716)



## Features

- **Image Loading and Transformation**:
  - The image is loaded and resized to a standard dimension (700x700 pixels).
  - Translation and rotation transformations are applied to align the image correctly, ensuring that both the reference object and the target object are properly oriented.

- **Manual Object Identification**:
  - Users can manually identify the reference object and the target object by clicking on their corresponding points in the transformed image.
  - The script captures these points and calculates the pixel distances between them.

- **Size Estimation**:
  - The real-world dimensions of the target object are calculated based on the known dimensions of the reference object.
  - The pixel distances are converted into real-world measurements using a scale factor derived from the reference object.
  - Users first select two points along the width and height of the object, and the script then calculates the object's real-world dimensions.

## Example Usage

```python
import cv2
import numpy as np

# Load and transform the image
image = cv2.imread("path_to_image")
# (Additional script details here)

# Manually select points and estimate size
# (Further implementation steps)
```

## How to Use

1. **Prepare the Image**:
   - Ensure that the reference object is clearly visible and positioned on the same plane as the target object in the image.

2. **Run the Script**:
   - Load the image and apply the necessary transformations.
   
   ![image](https://github.com/user-attachments/assets/eb3ed4ab-a73f-4414-96de-2c2455b6809c)

   - Manually click on the image to select points corresponding to the width and height of the objects.
   - The script will output the estimated real-world dimensions of the target object.

## Output
The script will print the estimated width and height of the target object in real-world units based on the known dimensions of the reference object.
![image](https://github.com/user-attachments/assets/27b48c2d-9889-440c-9d5a-3318d5b4c1ad)
![image](https://github.com/user-attachments/assets/4cd0eed2-a5a6-4a61-b0cd-3194087f9c2b)

This project demonstrates the application of computer vision techniques for practical measurement tasks, making it a useful tool in fields such as digital forensics, manufacturing, and quality control.

