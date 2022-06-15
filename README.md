# image-processing-<br>
program 1: Develop a program to display grayscale image usingread and write operation <br>
import cv<br>
img=cv2.imread("butter.jpg",0)<br>
cv2.imshow("butter",img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/99865138/173808282-3df0a570-73a7-43bb-99e9-6daa38728069.png)<br>
coloured image<br>
import cv2<br>
img=cv2.imread("butter.jpg",1)<br>
cv2.imshow("butter",img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/99865138/173814052-60ce2859-f8df-4b86-b784-f75c9eb92931.png)<br>
***********************************************************************************************************************
 Program2:Develop a program to perform linear transformation to rotation<br>
from PIL import Image<br>
img=Image.open("plant.jpg")<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/99865138/173809376-9093987f-301d-4d56-99c9-351e7f9733e9.png)<br>
*********************************************************************************************************************
program3:Develop a program to display image using malplot lib<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=mping.imread("flower.jpg")<br>
plt.imshow(img)<br>
Output:<br>
![image](https://user-images.githubusercontent.com/99865138/173810377-39d1c669-e53d-4f3f-9f22-000935e139d4.png)<br>
*********************************************************************************************************************<br>
Program4:Develop a program to convert colors string to RGB color values<br>
from PIL import ImageColor<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
img2=ImageColor.getrgb("red")<br>
print(img2)<br>
img3=ImageColor.getrgb("white")<br>
print(img3)<br>
img4=ImageColor.getrgb("pink")<br>
print(img4)<br>
img5=ImageColor.getrgb("blue")<br>
print(img5)<br>
img6=ImageColor.getrgb("green")<br>
print(img6)<br>
Output:<br>
(255, 255, 0)<br>
(255, 0, 0)<br>
(255, 255, 255)<br>
(255, 192, 203)<br>
(0, 0, 255)<br>
(0, 128, 0)<br>
************************************************************************************************************************<br>
Program5: Write a program to create image using color<br>
from PIL import Image<br>
img=Image.new("RGB",(200,400),(255,0,0))<br>
img.show()<br>
![image](https://user-images.githubusercontent.com/99865138/173811387-68dc949d-48fe-4df4-9d10-16a95ace1f43.png)<br>
************************************************************************************************************************<br>
program6: write a program to visual the image using various color space<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=cv2.imread("flower1.jpg")<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
plt.imshow(img)<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/99865138/173812933-2a8f212e-5473-4a6e-bd12-b47cf0a29bb4.png)<br>
![image](https://user-images.githubusercontent.com/99865138/173813006-4abfa48f-75c0-47bc-b974-060d5764e2de.png)<br>
************************************************************************************************************************<br>
Program to display the attributes of image<br>from PIL import Image<br>
image=Image.open("flower1.jpg")<br>
print("file name: ",image.filename)<br>
print("formate: ",image.format)<br>
print("mode: ",image.mode)
print("size: ",image.size)<br>
print("width: ",image.width)<br>
print("height : ",image.height)<br>
image.close();<br>
Output:<br>
file name:  flower1.jpg<br>
formate:  JPEG<br>
mode:  RGB<br>
size:  (225, 225)<br>
width:  225<br>
height :  225<br>

