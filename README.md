# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Program:

# Python
# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
```
image = np.zeros((500, 500, 3), dtype=np.uint8)
```
# Create the Text using cv2.putText
```

array([[[0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
        ...,
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0]],

       [[0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
        ...,
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0]],

       [[0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
        ...,
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0]],

       ...,

       [[0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
        ...,
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0]],

       [[0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
        ...,
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0]],

       [[0, 0, 0],
        [0, 0, 0],
        [0, 0, 0],
        ...,
        [0, 0, 0],
        [0, 0, 0],
        [0, 0, 0]]], shape=(500, 500, 3), dtype=uint8)

```
# Create the structuring element

```
kernel = np.ones((3, 3), np.uint8)
```

# Use Opening operation

```
opened_image = cv2.morphologyEx(image, cv2.MORPH_OPEN, kernel)

```
# Use Closing Operation

```
closed_image = cv2.morphologyEx(image, cv2.MORPH_CLOSE, kernel)


```
## Output:

### Display the input Image
<img width="389" height="409" alt="image" src="https://github.com/user-attachments/assets/7de36d8f-eec5-45df-9b88-c173ebcb348d" />

### Display the result of Opening
<img width="389" height="409" alt="image" src="https://github.com/user-attachments/assets/319dcf46-57c5-4dce-b7d9-68ca7738a079" />


### Display the result of Closing


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
