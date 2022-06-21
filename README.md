### EXP NO:01
### DATE:

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
# Developed By:SARAN M
# Register Number:212220230044
# To Read,display the image

import numpy as np
import cv2
img = cv2.imread('bike.jpg',1)
cv2.imshow('Bike',img)
cv2.waitKey(0)


# To write the image

cv2.imwrite('dk.jpg',img)


# Find the shape of the Image

print(img.shape)


# To access rows and columns

import random
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j]= [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('Bike',img)
cv2.waitKey(0)



# To cut and paste portion of image

bw2=cv2.imread("bike.jpg",1)
tag=bw2[30:100,30:120]
bw2[50:120,100:190]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
## Output:

### i) Read and display the image
![n1](https://user-images.githubusercontent.com/75235427/160874430-fa07a5a1-5c1c-443f-86fe-76d4f08f67d5.jpg)


### ii)Write the image
![n2](https://user-images.githubusercontent.com/75235427/160874457-3b3a144e-6927-4b4c-b3b3-c0c9b4be4bea.jpg)


### iii)Shape of the Image
![n2](https://user-images.githubusercontent.com/75235427/160874484-561f62f4-4f4a-4e21-b649-2bd7cd2f00e1.jpg)


### iv)Access rows and columns
![n3](https://user-images.githubusercontent.com/75235427/160874521-2ff2801f-8ae8-4390-a3fb-21d0acbc05e9.jpg)


### v)Cut and paste portion of image
![n4](https://user-images.githubusercontent.com/75235427/160874552-c2ae829d-fa21-4a69-856a-42956b14093f.jpg)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


