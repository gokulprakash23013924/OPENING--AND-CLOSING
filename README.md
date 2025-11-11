# EX-10 OPENING--AND-CLOSING
# Name : Gokul prakash m
# Register Number : 212223240041
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

 
## Program:
```

import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((500, 500, 3), dtype=np.uint8)
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'Open and Close', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
kernel = np.ones((3, 3), np.uint8)
plt.subplot(1, 3, 1)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title("Input Image")
plt.axis('off')
plt.subplot(1, 3, 2)
plt.imshow(cv2.cvtColor(opened_image, cv2.COLOR_BGR2RGB))
plt.title("Opening Operation")
plt.axis('off')
plt.subplot(1, 3, 3)
plt.imshow(cv2.cvtColor(closed_image, cv2.COLOR_BGR2RGB))
plt.title("Closing Operation")
plt.axis('off')



```
## Output:

### Display the input Image
<img width="380" height="398" alt="image" src="https://github.com/user-attachments/assets/8f39bca2-bbe8-4ca8-839b-9c15f827694e" />


### Display the result of Opening
<img width="376" height="398" alt="image" src="https://github.com/user-attachments/assets/b09d90d8-c125-459d-8973-fa841681c1fe" />



### Display the result of Closing
<img width="372" height="394" alt="image" src="https://github.com/user-attachments/assets/db30c196-5602-45be-866f-233d1edbdc24" />




## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
