# image-processing-<br>
program 1: Develop a program to display grayscale image usingread and write operation <br>
import cv<br>
img=cv2.imread("butter.jpg",0)<br>
cv2.imshow("butter",img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
![image](https://user-images.githubusercontent.com/99865138/173808282-3df0a570-73a7-43bb-99e9-6daa38728069.png)<br>
Develop a program to perform linear transformation to rotation<br>
from PIL import Image<br>
img=Image.open("plant.jpg")<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
![image](https://user-images.githubusercontent.com/99865138/173809376-9093987f-301d-4d56-99c9-351e7f9733e9.png)<br>
