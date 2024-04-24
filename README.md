# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.

## ProgramL:
```
Developed by : kamali E
Reg.no: 212222110015
```

## Import the packages
```
import cv2
import matplotlib.pyplot as plt
```

## Load the image, Convert to grayscale and remove noise
```
import cv2
import matplotlib.pyplot as plt

img=cv2.imread("dogpair.jpg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```

## SOBEL EDGE DETECTOR:

## SOBEL X AXIS
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelx)
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
## SOBEL Y AXIS :
```
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobely)
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
## SOBEL XY AXIS :
 ```
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelxy)
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
## LAPLACIAN EDGE DETECTOR
```
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(lap)
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```

## CANNY EDGE DETECTOR
```
canny=cv2.Canny(gray,120,150)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(canny)
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
### SOBEL EDGE DETECTOR

![319021970-d9855028-b449-4285-a8c4-6197dd2a29dc](https://github.com/Kamali22004796/EDGE-DETECTION/assets/120567837/ae495337-c41d-483e-a5f0-7fc9d76fc3a2)

### LAPLACIAN EDGE DETECTOR


![319022013-6736c8e2-71fa-4057-9492-85e72d0a67cd](https://github.com/Kamali22004796/EDGE-DETECTION/assets/120567837/50cbc0e3-e54a-4dcd-8fb9-2cc3a5558ec1)



### CANNY EDGE DETECTOR

![319022060-e5766fa6-5e45-4bc1-accb-d97e35b02128](https://github.com/Kamali22004796/EDGE-DETECTION/assets/120567837/9a1702d1-e9c5-4ab8-95d5-b536274de79c)


![319022120-1a03977b-7b95-4947-99c6-6cadd729d0ec](https://github.com/Kamali22004796/EDGE-DETECTION/assets/120567837/bd745a8f-8bf7-4893-8e95-25622408a9ad)


![319022168-5865e513-1f64-477b-b3b6-8b1d2bddbd13](https://github.com/Kamali22004796/EDGE-DETECTION/assets/120567837/2f55f3e2-8c24-4b44-9748-c848e3ec0bde)



## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
