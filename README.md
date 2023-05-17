## EX.NO: 10 <br>
## DATE: 
## <p align="center">IMPLEMENTATION OF EROSION AND DILATION</p>

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages.


### Step2:
<br>Create the Text using cv2.putText.

### Step3:
<br>Create the structuring element.

### Step4:
<br>Erode and Dilate the image.

### Step5:
<br>End Program.

 
## Program:
```
DEVELOPED BY : VIGNESH M
REG NO : 212220233002
```

``` Python
# Import the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt



# Create the Text using cv2.putText
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX
cv2.putText(img1,'Vignesh',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1)


# Create the structuring element
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))




# Erode the image

image_erode=cv2.erode(img1,kernel)
plt.imshow(image_erode)
plt.axis('off')
plt.title('Erosion')



# Dilate the image

image_dilate=cv2.dilate(img1,kernel)
plt.imshow(image_dilate)
plt.axis('off')
plt.title('Dilation')



```
## Output:

### Display the input Image
<br>![image](https://github.com/vignesh0011/Implementation-of-Erosion-and-Dilation/assets/53014593/1cad1e05-7a0c-4dab-8a83-1421e4873508)

<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
<br>![image](https://github.com/vignesh0011/Implementation-of-Erosion-and-Dilation/assets/53014593/dd185e84-f057-4d2f-a853-079ec479bc95)

<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image
<br>![image](https://github.com/vignesh0011/Implementation-of-Erosion-and-Dilation/assets/53014593/9b5eeda8-b352-4552-bbd1-bd43d86230a5)
<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
