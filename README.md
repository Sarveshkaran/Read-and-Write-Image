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
#### Developed By: SARVESHKARAN
#### Register Number: 212221230089
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('sun2.jpg',1)
cv2.imshow('sun2',color_image)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
color_image = cv2.imread('sun2.jpg',1)
h = cv2.imwrite('sun2.jpg',color_image)
cv2.imshow('hari',color_image)
cv2.waitKey(0) 
```
iii) #Find the shape of the Image
```
import cv2
color_image = cv2.imread('sun2.jpg',1)
print(color_image.shape)
```
iv) #To access rows and columns
```
import random
import cv2
color_image = cv2.imread('sun2.jpg',1)
for i in range(150):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('sun2.jpg',color_image)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color_image = cv2.imread('sun2.jpg',1)
part = color_image[300:400,300:400]
color_image[50:150,50:150] = part
cv2.imshow("hari",color_image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
![dip11](https://user-images.githubusercontent.com/93427253/224548594-4d6a34cb-355d-4830-8210-ca4b92d6059f.png)


### ii)Write the image
![dip12](https://user-images.githubusercontent.com/93427253/224548613-b076986d-adb9-4547-9982-8abe750d8da8.png)


### iii)Shape of the Image
![image](https://user-images.githubusercontent.com/93427253/224548704-93bf0e1e-852d-4340-9c12-58b459e6819b.png)


### iv)Access rows and columns
![dip13](https://user-images.githubusercontent.com/93427253/224548726-fad286f5-abe6-4f16-9b64-f252248175a2.png)


### v)Cut and paste portion of image
![dip14](https://user-images.githubusercontent.com/93427253/224548753-b004e7a2-24b5-43ae-a2e1-bc9306108df4.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
