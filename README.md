# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
<br>

### Step2:
Create the Text using cv2.putText
<br>

### Step3:
Create the structuring element
<br>

### Step4:
Use Opening operation
<br>

### Step5:
Use Closing Operation
<br>

## Program:
```
Developed by: SRI SAI PRIYA.S
Register Number:212222240103
```
# Display the input Image
```
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'SAMYUKTHA', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
# Create ths structured element
```
struct_ele = np.ones((9, 9), np.uint8)
```
# Display the result of Opening
```
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
# Display the result of Closing
```
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image

![WhatsApp Image 2024-04-16 at 14 11 38_aa509d4a](https://github.com/SriSaiPriyaSenthilvel/OPENING--AND-CLOSING/assets/119475702/b6ebbe81-7971-4993-ae69-f3fae1b4b12b)
<br>

### Display the result of Opening

![WhatsApp Image 2024-04-16 at 14 12 36_d7893b3c](https://github.com/SriSaiPriyaSenthilvel/OPENING--AND-CLOSING/assets/119475702/e8d68cb0-76f1-4c49-b9b7-9ffa1d0cc934)
<br>

### Display the result of Closing

![WhatsApp Image 2024-04-16 at 14 14 19_562b7334](https://github.com/SriSaiPriyaSenthilvel/OPENING--AND-CLOSING/assets/119475702/ec6dabee-d6ec-4235-9e08-aeae28e501f0)
<br>

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
