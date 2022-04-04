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
### Developed By:challa sandeep
### Register Number:212221240011

i) #To Read,display the image
```
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.jpeg',1)
cv2.imshow('212221240011-Read&Display',colorImage)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.jpeg',1)
cv2.imwrite('/Users/eswar1607/Desktop/written.jpg',colorImage)
writtenImage = cv2.imread('/Users/eswar1607/Desktop/written.jpg',1)
cv2.imshow('212221240011-WrittenImage',writtenImage)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.jpeg',1)
print(colorImage.shape)
```
iv) #To access rows and columns

```
import cv2
import random
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.jpeg',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240011-AccessingRowsAndColumns',colorImage)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color_img = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
tag = color_img[50:250,100:300]
color_img[100:300,50:250] = tag
cv2.imshow('212221240011-CutAndPaste',color_img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

<br>
![Github logo](sandeep1.png)
<br>

### ii)Write the image

<br>
![Github logo](sandeep2.png)
<br>

### iii)Shape of the Image

<br>
<img width="697" alt="Screenshot 2022-04-01 at 9 48 53 PM" src="https://user-images.githubusercontent.com/93427522/161304000-26e72c4f-2332-4305-8a3a-17dd07103cea.png">
<br>

### iv)Access rows and columns
<br>
![Github Logo](sandeep3.png)
<br>

### v)Cut and paste portion of image
<br>
![Github Logo](sandeep4.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
