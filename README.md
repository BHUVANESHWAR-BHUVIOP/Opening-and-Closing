# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step1:
Import the necessary packages.
<br>

### Step2:
Create the Text using cv2.putText.
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

``` Python
# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt
# Load the Image
img1=np.zeros((100,600),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
# Create the Text using cv2.putText
cv2.putText(img1,' GRAND THEFT AUTO ',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')
plt.title('Input Text'), plt.xticks([]), plt.yticks([])
plt.show()
# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
# Use Opening operation
image1=cv2.morphologyEx(im,cv2.MORPH_OPEN,kernel1)
plt.imshow(image1,cmap='gray')
plt.title('OPENING'), plt.xticks([]), plt.yticks([])
plt.show()
# Use Closing Operation
image1=cv2.morphologyEx(im,cv2.MORPH_CLOSE,kernel1)
plt.imshow(image1,cmap='gray')
plt.title('CLOSING'), plt.xticks([]), plt.yticks([])
plt.show()
```
## Output:

### Display the input Image
![OUTPUT](OP1.png)
<br>
<br>
<br>
<br>
<br>
<br>

### Display the result of Opening
![OUTPUT](OP2.png)
<br>
<br>
<br>
<br>
<br>
<br>

### Display the result of Closing
![OUTPUT](OP3.png)
<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.![OP3](https://user-images.githubusercontent.com/94155099/172343199-7115cd5a-5a27-4260-b9fd-1ac8928a3bc8.png)
![OP1](https://user-images.githubusercontent.com/94155099/172343205-22bd0f32-ed04-483e-9db6-ad93dd3cb071.png)
![OP2](https://user-images.githubusercontent.com/94155099/172343208-e518aa12-7c6e-4a06-af0c-6e78bad928dc.png)
