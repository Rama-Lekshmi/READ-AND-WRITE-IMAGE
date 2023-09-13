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
```
### Developed By: Rama E.K. Lekshmi
### Register Number:212222240082
``` 
i) #To Read,display the image
```
import cv2
image=cv2.imread("theodore.jpg",1)
cv2.imshow("21222240082_Rama E.K. Lekshmi",image)
cv2.waitKey(0)
cv2.destroyAllwindows()
  ```
ii) #To write the image
```
import cv2
image=cv2.imread("theodore.jpg",1)
cv2.imwrite("theodore.jpg",image)
cv2.imshow("21222240082_Rama E.K. Lekshmi",image)
cv2.waitKey(0)
cv2.destroyAllwindows()



```
iii) #Find the shape of the Image
```
import cv2
picture=cv2.imread("theodore.jpg",1)
print(picture.shape)
```


iv) #To access rows and columns

```
import random
import cv2
image=cv2.imread("theodore.jpg",1)
for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("21222240082_Rama E.K. Lekshmi",image)
cv2.waitKey(0)
cv2.destroyAllwindows()


```
v) #To cut and paste portion of image
```
import cv2
img = cv2.imread('theodore.jpg', 1)
tag = img[20:80:, 20:80]
img[90:150, 90:150] = tag
cv2.imshow('221222240082_Rama E.K. Lekshmi', img)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image


 ![WhatsApp Image 2023-09-13 at 1 46 25 PM](https://github.com/Rama-Lekshmi/READ-AND-WRITE-IMAGE/assets/118541549/c40a5ca3-597b-48e6-8be2-72fd76284789)


### ii)Write the image


![WhatsApp Image 2023-09-13 at 1 46 25 PM](https://github.com/Rama-Lekshmi/READ-AND-WRITE-IMAGE/assets/118541549/9dc5d0a4-e118-4a31-8ff7-6ca53fa66df2)


### iii)Shape of the Image


![WhatsApp Image 2023-09-13 at 1 50 41 PM](https://github.com/Rama-Lekshmi/READ-AND-WRITE-IMAGE/assets/118541549/d1f4cde3-3b02-4157-a7f4-b93d160392e5)


### iv)Access rows and columns

![WhatsApp Image 2023-09-13 at 1 46 38 PM](https://github.com/Rama-Lekshmi/READ-AND-WRITE-IMAGE/assets/118541549/93d2c916-e554-4d07-83a7-fecfd51bf60d)



### v)Cut and paste portion of image

![shape](https://github.com/Rama-Lekshmi/READ-AND-WRITE-IMAGE/assets/118541549/933f9ee9-03ff-43a0-a1dd-31200f812648)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
