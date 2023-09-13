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
### Developed By: KAVYA K
### Register Number: 212222230065
i) #To Read,display the image
```
image=cv2.imread("nature.jpg",1)
cv2_imshow(image)  

```
ii) #To write the image
```
image = cv2.imread("nature.jpg",-1)
cv2.imwrite("pain.jpg",image)


```
iii) #Find the shape of the Image
```python3
print(image.shape)


```
iv) #To access rows and columns

```python3

for i in range(150):
    for j in range(image.shape[1]):
        image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(image)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3
image= cv2.imread('pranav.jpg',-1)
new = image[200:450,200:450]
image[150:400,150:400] = new
cv2_imshow(image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>

![](nature.jpg)
<br>

### ii)Write the image

<br>

![](true.png)
<br>

### iii)Shape of the Image

<br>

![](res.jpg)
<br>

### iv)Access rows and columns
<br>

![](2.png)
<br>

### v)Cut and paste portion of image
<br>

![](3.png)
<br>
<br><br>
<br><br>
<br>
<br>
<br>
<br>
<br>
<br><br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br><br><br>


<br>



























## Result:
Thus the images are read, displayed, and written successfully using the python program.


