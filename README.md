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
In rotation 90<br>
from PIL import Image<br>
img=Image.open("plant.jpg")<br>
img=img.rotate(90)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/99865138/173814757-8f91f3fb-52c5-4c18-a381-96477c2169e8.png)<br>

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
Program7: to display the attributes of image<br>from PIL import Image<br>
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
************************************************************************************************************************************<br>
program 8:resize the original image<br>
import cv2 <br>
img=cv2.imread("flower.jpg")<br>
print("original image length and width",img.shape)<br>
cv2.imshow("original image",img)<br>
cv2.waitKey(0)<br>
imgresize=cv2.resize(img,(150,150))<br>
cv2.imshow("resized image",imgresize)<br>
print("resized  image length and width",imgresize.shape)<br>
cv2.waitKey(0)<br>
![image](https://user-images.githubusercontent.com/99865138/175275336-5073426e-55fa-4549-b527-b0b2c74e993f.png)<br>
***************************************************************************************************************************<br>
program 9:convert the original image to gray scale and then to display binary<br>
import cv2<br>
img=cv2.imread('flower1.jpg')<br>
cv2.imshow("RGB",img)<br>
cv2.waitKey(0)<br>

img=cv2.imread('flower1.jpg')<br>
cv2.imshow("Gray",img)<br>
cv2.waitKey(0)<br>

ret,bw_ing=cv2.threshold(img,127,255,cv2.THRESH_BINARY)<br>

cv2.imshow("binary",bw_ing)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
![image](https://user-images.githubusercontent.com/99865138/175283628-61397272-a5f7-45c1-a78b-024d302a0715.png)<br>
![image](https://user-images.githubusercontent.com/99865138/175283686-568894c3-a98b-46e0-9a07-b31d4a2c7553.png)<br>
![image](https://user-images.githubusercontent.com/99865138/175283735-0af573a1-cf68-4269-9e2b-a8a34f5d2404.png)<br>

****************************************************************************************************************************************<br>
program 10: Develop a program to readimage using URL.<br>
from skimage import io<br>
import matplotlib.pyplot as plt<br>
url='https://th.bing.com/th/id/OIP.Tr0An6GO1XiVM3am60LKMwHaGC?w=224&h=183&c=7&r=0&o=5&pid=1.7.jpg'<br>
image=io.imread(url)<br>
plt.imshow(image)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/175005312-c7c1e787-99ac-49ee-a50b-1dee2a729a24.png)<br>
******************************************************************************************************************************<br>
program 11 :Write a program to perform arithmatic operations on images<br>
 import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('fish.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/175016673-ee57fa8c-c951-48e0-93c7-e28345181bc8.png)<br>
hsv_img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
light_orange=(1,190,200)<br>
dark_orange=(18,255,255)<br>
mask=cv2.inRange(img,light_orange,dark_orange)<br>
result=cv2.bitwise_and(img,img,mask=mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/175016836-eb3151e4-d77d-4019-89ff-00ef1b263ab1.png)<br>
light_white=(0,0,200)<br>
dark_white=(145,60,255)<br>
mask_white=cv2.inRange(hsv_img,light_white,dark_white)<br>
result_white=cv2.bitwise_and(img,img,mask=mask_white)<br>
plt.subplot(1,2,1)<br>
plt.imshow(mask_white,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result_white)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/175016925-ed6726ae-c305-4a5c-8870-363536006c17.png)<br>
final_mask=mask+mask_white<br>
final_result=cv2.bitwise_and(img,img,mask=final_mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(final_mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result_white)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/175017012-9b57e6a1-7943-473b-9bee-ebee724016f7.png)<br>
blur=cv2.GaussianBlur(final_result,(7,7),0)<br>
plt.imshow(blur)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/175017126-edae4b01-edb3-442a-8c0c-4ff18b9bd4be.png)<br>
**********************************************************************************************************************************<br>
program 12: Write a program to perform arithmatic operations on images<br>
import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>

img1=cv2.imread('f2.jpg')<br>
img2=cv2.imread('f3.jpg')<br>

fimg1=img1+img2<br>
plt.imshow(fimg1)<br>
plt.show()<br>

cv2.imwrite('output.jpg',fimg1)<br>
fimg2=img1-img2<br>
plt.imshow(fimg2)<br>
plt.show()<br>

cv2.imwrite('output.jpg',fimg2)<br>
fimg3=img1*img2<br>
plt.imshow(fimg3)<br>
plt.show()<br>

cv2.imwrite('output.jpg',fimg3)<br>
fimg4=img1/img2<br>
plt.imshow(fimg4)<br>
plt.show()<br>

cv2.imwrite('output.jpg',fimg4)<br>
![image](https://user-images.githubusercontent.com/99865138/175019852-12f8a408-0e21-479e-9c22-0e6654c1969c.png)<br>
C:\Users\User\AppData\Local\Temp\ipykernel_13152\756045841.py:23: RuntimeWarning: divide by zero encountered in true_divide<br>
  fimg4=img1/img2<br>
C:\Users\User\AppData\Local\Temp\ipykernel_13152\756045841.py:23: RuntimeWarning: invalid value encountered in true_divide<br>
  fimg4=img1/img2
Clipping input data to the valid range for imshow with RGB data ([0..1] for floats or [0..255] for integers).<br>
![image](https://user-images.githubusercontent.com/99865138/175019959-471502be-0249-4d11-a0f8-cc0f19d4ea3a.png)!<br>
*****************************************************************************************************************************<br>
program 13: develop the program to change the image to different color space<br>
import cv2<br> 
img=cv2.imread("E:\plant1.jpg")<br>
gray=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)<br>
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)<br>
lab=cv2.cvtColor(img,cv2.COLOR_BGR2LAB)<br>
hls=cv2.cvtColor(img,cv2.COLOR_BGR2HLS)<br>
yuv=cv2.cvtColor(img,cv2.COLOR_BGR2YUV)<br>
cv2.imshow("GRAY image",gray)<br>
cv2.imshow("HSV image",hsv)<br>
cv2.imshow("LAB image",lab)<br>
cv2.imshow("HSL image",hls)<br>
cv2.imshow("YUV image",yuv)<br>
cv2.waitKey(0)<br>
cv2.destoryAllWindows()<br>
![image](https://user-images.githubusercontent.com/99865138/175267198-cc80280e-bed0-4b5a-83ee-2af9f9ddf769.png)<br>

![image](https://user-images.githubusercontent.com/99865138/175267265-505b8f03-f93a-43f2-a2d6-c8dcc42d1959.png)<br>
![image](https://user-images.githubusercontent.com/99865138/175267412-e3462df4-8c27-492f-a973-04849ffddf00.png)<br>
![image](https://user-images.githubusercontent.com/99865138/175267525-dd44954b-a3d5-4eba-887b-534c88c8772e.png)<br>
![image](https://user-images.githubusercontent.com/99865138/175268077-c617ad0a-8e08-45e8-89a9-dfeb41eab630.png)<br>
********************************************************************************************************************<br>
Program  14:to develop an image using 2D array<br>
import cv2 as c<br>
import numpy as np<br>
from PIL import Image<br>
array=np.zeros([100,200,3],dtype=np.uint8)<br>
array[:,:100]=[255,0,0]<br>
array[:,100:]=[0,0,255]<br>
img=Image.fromarray(array)<br>
img.save('image1.jpg')<br>
img.show()<br>
c.waitKey(0)<br>
![image](https://user-images.githubusercontent.com/99865138/175270940-31b8aa75-07ea-4027-8d2f-6e6c725a1554.png)<br>
****************************************************************************************************************************<br>
program 15:develope an image using bitwise operation<br>
************************************************************************************************************************<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
image1=cv2.imread("b1.jpg",1)<br>
image2=cv2.imread("b1.jpg")<br>
ax=plt.subplots(figsize=(15,10))<br>
bitwiseAnd=cv2.bitwise_and(image1,image2)<br>
bitwiseOr=cv2.bitwise_or(image1,image2)<br>
bitwiseXor=cv2.bitwise_xor(image1,image2)<br>
bitwiseNot_img1=cv2.bitwise_not(image1)<br>
bitwiseNot_img2=cv2.bitwise_not(image2)<br>
plt.subplot(151)<br>
plt.imshow(bitwiseAnd)<br>
plt.subplot(152)<br>
plt.imshow(bitwiseOr)<br>
plt.subplot(153)<br>
plt.imshow(bitwiseXor)<br>
plt.subplot(154)<br>
plt.imshow(bitwiseNot_img1)<br>
plt.subplot(155)<br>
plt.imshow(bitwiseNot_img2)<br>
cv2.waitKey(0)<br>
![image](https://user-images.githubusercontent.com/99865138/176406989-3a61812a-5614-442d-aa1f-4112ff75f2f1.png)<br>
*also using different image<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
image1=cv2.imread("a1.jpg",1)<br>
image2=cv2.imread("s1.jpg")<br>
ax=plt.subplots(figsize=(15,10))<br>
bitwiseAnd=cv2.bitwise_and(image1,image2)<br>
bitwiseOr=cv2.bitwise_or(image1,image2)<br>
bitwiseXor=cv2.bitwise_xor(image1,image2)<br>
bitwiseNot_img1=cv2.bitwise_not(image1)<br>
bitwiseNot_img2=cv2.bitwise_not(image2)<br>
plt.subplot(151)<br>
plt.imshow(bitwiseAnd)<br>
plt.subplot(152)<br>
plt.imshow(bitwiseOr)<br>
plt.subplot(153)<br>
plt.imshow(bitwiseXor)<br>
plt.subplot(154)<br>
plt.imshow(bitwiseNot_img1)<br>
plt.subplot(155)<br>
plt.imshow(bitwiseNot_img2)<br>
cv2.waitKey(0)<br>
![image](https://user-images.githubusercontent.com/99865138/176407181-bcadef59-3a60-42e2-8e38-6d0f45dec2f6.png)<br>
**********************************************************************************************************<br>
