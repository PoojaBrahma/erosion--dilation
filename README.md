# EXP-9 Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import required libraries (OpenCV, NumPy) and load the image in grayscale.
### Step2:
Define a structuring element (kernel) for morphological operations.
### Step3:
Apply erosion using cv2.erode() on the image with the defined kernel.
### Step4:
Apply dilation using cv2.dilate() on the image with the same kernel.
### Step5:
Display and compare the original, eroded, and dilated images
## Program:
# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Input Image with Text
```
#NAME: POOJA P
#REG NO: 212224230195
import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((500, 500, 3), dtype=np.uint8)
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'MONISH', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB for displaying
plt.title("Input Image with Text")
plt.axis('off')
```
# Erode the image
```
#NAME: MONISH N
#REG NO: 212223240097
kernel = np.ones((3, 3), np.uint8)
eroded_image = cv2.erode(image, kernel, iterations=1)

plt.imshow(cv2.cvtColor(eroded_image, cv2.COLOR_BGR2RGB))
plt.title("Eroded Image")
plt.axis('off')
```
# Dilate the image
```
#NAME: POOJA P
#REG NO: 212224230195
dilated_image = cv2.dilate(image, kernel, iterations=1)


plt.imshow(cv2.cvtColor(dilated_image, cv2.COLOR_BGR2RGB)) 
plt.title("Dilated Image")
plt.axis('off')

```
## Output:

### Display the input Image
<img width="395" height="425" alt="image" src="https://github.com/user-attachments/assets/f6c2d931-87b2-445c-a197-ff16a90c96b2" />


### Display the Eroded Image
<img width="423" height="429" alt="image" src="https://github.com/user-attachments/assets/cad86eb9-d784-429f-af0e-a433a5e7bbf7" />


### Display the Dilated Image
<img width="417" height="417" alt="image" src="https://github.com/user-attachments/assets/155e2e86-3cc9-40f2-8b9b-1bfa46fcd659" />


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
