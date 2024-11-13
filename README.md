# EX-10
# OPENING AND CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
- Step1: Import the necessary packages
- Step2: Give the input text using cv2.putText()
- Step3: Perform opening operation and display the result
- Step4: Similarly, perform closing operation and display the result
- 
## Program:
### NAME: Ashwin Kumar S
### REG.No:212222240013

# Import the necessary packages
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
image = np.zeros((300, 600, 3), dtype="uint8")
text = "ASHWIN KUMAR S"
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, text, (50, 150), font, 2, (255, 255, 255), 3)

```
# Create the structuring element
```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
```
# Use Opening operation
```
opening_image = cv2.morphologyEx(image, cv2.MORPH_OPEN, kernel)
plt.imshow(opening_image_rgb)
plt.title("Opening Operation")
plt.axis("off")
```
# Use Closing Operation
```
closing_image = cv2.morphologyEx(image, cv2.MORPH_CLOSE, kernel)
plt.imshow(closing_image_rgb)
plt.title("Closing Operation")
plt.axis("off")
```
## Output:
### Display the input Image
![image](https://github.com/user-attachments/assets/869b9568-d7bf-4561-b95c-500321ed9277)

### Display the result of Opening
![image](https://github.com/user-attachments/assets/ceb453fb-c6a3-43ba-b521-7ef431deeaa9)

### Display the result of Closing
![image](https://github.com/user-attachments/assets/ed8c5d96-8f89-49ef-8a56-387b796c2095)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
