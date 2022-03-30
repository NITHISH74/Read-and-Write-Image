# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By: NITHISHWAR S
# Register Number: 212221230071

# To Read,display the image

import cv2
color= cv2.imread('spidy.jpg',-1)
cv2.imshow('Ragul AC 212221240042',color)
cv2.waitKey(0)


# To write the image

import cv2
color= cv2.imread('spidy.jpg',-1)
cv2.imwrite('spidy.jpg',color)

# Find the shape of the Image
import cv2
color=cv2.imread('spidy.jpg',1)
print(color.shape)

# To access rows and columns

import cv2
import random
img= cv2.imread('spidy.jpg',-1)
for i in range(300):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('Ragul AC 212221240042',img)
cv2.waitKey(0)


# To cut and paste portion of image


import cv2
img= cv2.imread('spidy.jpg',-1)
tag = img[200:450,200:450]
img[150:400,150:400] = tag
cv2.imshow('Ragul AC 212221240042',img)
cv2.waitKey(0)

```
## Output:

### i) Read and display the image
<br>


### ii)Write the image
<br>


### iii)Shape of the Image

<br>

### iv)Access rows and columns
<br>

### v)Cut and paste portion of image
<br>


## Result:
Thus the images are read, displayed, and written successfully using the python program.


