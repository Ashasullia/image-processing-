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
program 16: develop an image using blurring<br>
import cv2<br>
import numpy as np<br>

image=cv2.imread("a1.jpg")<br>
cv2.imshow("original image",image)<br>
cv2.waitKey(0)<br>

Gaussian=cv2.GaussianBlur(image,(7,7),0)<br>
cv2.imshow("Gaussian blurring",Gaussian)<br>
cv2.waitKey(0)<br>

median=cv2.medianBlur(image,5)<br>
cv2.imshow("median blurring",median)<br>
cv2.waitKey(0)<br>


bilateral=cv2.bilateralFilter(image,9,75,75)<br>
cv2.imshow("bilateral blurring",bilateral)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
![image](https://user-images.githubusercontent.com/99865138/176414252-06734e0c-8c1a-4528-bf16-03a259d9bdf2.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176414332-162fdeea-1fbb-42ee-ab1f-bed2942b8741.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176414471-aab79085-7873-44e5-896a-d323d703bd34.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176414610-664f83ee-1a37-49fd-a9ec-3f6231bb1354.png)<br>
*****************************************************************************************************************<br>
program 17 : develop an image using enhancement method<br>
from PIL import Image<br>
from PIL import ImageEnhance<br>
image=Image.open("a2.jpg")<br>
image.show()<br>

enh_bri=ImageEnhance.Brightness(image)<br>
brightness=1.5<br>
image_brightened=enh_bri.enhance(brightness)<br>
image_brightened.show()<br>

enh_col=ImageEnhance.Color(image)<br>
color=1.5<br>
image_colored=enh_col.enhance(color)<br>
image_colored.show()<br>

enh_con=ImageEnhance.Contrast(image)<br>
contrast=1.5<br>
image_contrasted=enh_col.enhance(contrast)<br>
image_contrasted.show()<br>

enh_sha=ImageEnhance.Sharpness(image)<br>
sharpness=1.5<br>
image_sharped=enh_col.enhance(sharpness)<br>
image_sharped.show()<br>
![image](https://user-images.githubusercontent.com/99865138/176423251-b1a20be8-333f-4927-a7d8-24840bc3ff17.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176423295-3f6364ad-6a65-4105-9189-921c0bb80669.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176423352-c4ea6adf-c0fd-4cd2-89a7-6c78c7345869.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176423409-84cee290-707e-4f20-ad42-9b5791c055f2.png)<br>
![image](https://user-images.githubusercontent.com/99865138/176423620-66485e60-b39f-4a7f-a213-4ab3127827bf.png)<br>
******************************************************************************************************************<br>
program 18:<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
from PIL import Image,ImageEnhance<br>
img=cv2.imread('a1.jpg',0)<br>
ax=plt.subplots(figsize=(20,10))<br>
kernel=np.ones((5,5),np.uint8)<br>
opening=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)<br>
closing=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)<br>
erosion=cv2.erode(img,kernel,iterations=1)<br>
dilation=cv2.dilate(img,kernel,iterations=1)<br>
gradient=cv2.morphologyEx(img,cv2.MORPH_GRADIENT,kernel)<br>
plt.subplot(151)<br>
plt.imshow(opening)<br>
plt.subplot(152)<br>
plt.imshow(closing)<br>
plt.subplot(153)<br>
plt.imshow(erosion)<br>
plt.subplot(154)<br>
plt.imshow(dilation)<br>
plt.subplot(155)<br>
plt.imshow(gradient)<br>
cv2.waitKey(0)<br>
![image](https://user-images.githubusercontent.com/99865138/176427055-e1313b06-e76b-4f17-aa7d-e14a5086c00f.png)<br>
****************************************************************************************************************
 19:  1.      Develop a program to<br>
(i)                Read the image, convert it into grayscale image<br>
(ii)              write (save) the grayscale image and<br>
(iii)            display the original image and grayscale image<br>

 (Note: To save image to local storage using Python, we use cv2.imwrite() function on OpenCV library )<br>
 
 
import cv2<br>
OriginalImg=cv2.imread('b6.jpg')<br>
GrayImg=cv2.imread('b6.jpg',0)<br>
isSaved=cv2.imwrite('D:/i.jpg',GrayImg)<br>
cv2.imshow("display Original Image",OriginalImg)<br>
cv2.imshow("display Grayscale Image",GrayImg)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
if isSaved:<br>
    print("the image is succesfully saved.")<br>
![image](https://user-images.githubusercontent.com/99865138/178702083-4cdf01bc-503f-4d11-9629-a10b2fd6c636.png)<br>
![image](https://user-images.githubusercontent.com/99865138/178702163-f968d5ee-62aa-4fa8-9c46-8276a659b2cc.png)<br>
![image](https://user-images.githubusercontent.com/99865138/178705660-ce9db1c4-c914-4c2b-9d6a-52b8c2d35df2.png)<br>
the image is succesfully saved.<br>

***************************************************************************************************************<br>
program 20:<br>
slicing with back ground<br>


import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image = cv2.imread("b6.jpg",0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range(0,x):<br>
    for j in range(0,y):<br>
        if (image[i][j]>50 and image[i][j]<150):<br>
            z[i][j]-255<br>
        else:<br>
           z[i][j]=image[i][j]<br>
equ=np.hstack((image,z))<br>
plt.title('gray level slicing with background ')<br>
plt.imshow(equ,'gray')<br>
plt.show() <br>           

![image](https://user-images.githubusercontent.com/99865138/178707197-cb178bb9-b853-4567-85e0-eaf768a0b4f9.png)<br>

**************************************************************************************************************<br>
program 21 :slicing with out background<br>

import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image = cv2.imread("b6.jpg",0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range(0,x):<br>
    for j in range(0,y):<br>
        if (image[i][j]>50 and image[i][j]<150):<br>
            z[i][j]=255<br>
        else:<br>
           z[i][j]=0<br>
equ=np.hstack((image,z))<br>
plt.title('gray level slicing without background ')<br>
plt.imshow(equ,'gray')<br>
plt.show() <br>           
            
![image](https://user-images.githubusercontent.com/99865138/178707925-d60a52ca-4461-4e2d-810b-f395ec42dfad.png)<br>
*************************************************************************************************************<br>
program 22 :<br>
using histogram<br><br><br> 
using variable library <br><br><br>

import matplotlib.pyplot as plt<br><br><br>
import numpy as np<br><br><br>

x = np.random.normal(170, 10, 250)<br><br><br>

plt.hist(x)<br><br><br>
plt.show() <br><br><br>
![image](https://user-images.githubusercontent.com/99865138/178960723-ca7c2937-1354-48c1-b486-a57df21d5c7e.png)<br><br><br>


*********************************************************************************************************************<br>
program 23:<br>
from matplotlib import pyplot as plt<br><br>
import numpy as np<br><br>
fig,ax = plt.subplots(1,1)<br><br>
a = np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27])<br><br>
ax.hist(a, bins = [0,25,50,75,100])<br><br>
ax.set_title("histogram of result")<br><br>
ax.set_xticks([0,25,50,75,100])<br><br>
ax.set_xlabel('marks')<br><br>
ax.set_ylabel('no. of students')<br><br>
plt.show()<br><br>

![image](https://user-images.githubusercontent.com/99865138/178960830-6380e45d-3784-412b-a833-ecd99d215fbb.png)<br><br>

*************************************************************************************************************************<br>
program 24 :<br>
import numpy as np<br><br>
import cv2 as cv<br><br>
from matplotlib import pyplot as plt<br><br>
img = cv.imread('b7.jpg')<br><br>
plt.imshow(img)<br><br>
plt.show()<br><br>
img = cv.imread('b7.jpg',0)<br><br>
plt.hist(img.ravel(),256,[0,256]);<br><br>
plt.show()<br><br>
![image](https://user-images.githubusercontent.com/99865138/178960892-a8401061-5d6b-42a6-9110-ecd935468f27.png)<br><br>


****************************************************************************************************************************<br>
program 25 :<br>
from skimage import io<br>
import matplotlib.pyplot as plt<br>
img = io.imread('b6.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
image = io.imread('b6.jpg')<br>
ax = plt.hist(image.ravel(), bins = 256)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/99865138/178960961-8754d422-ab65-4867-a7d4-4f64ed91bb6e.png)<br>

*********************************************************************************************************************************<br>
program 25 :<br>
from skimage import io<br>
import matplotlib.pyplot as plt<br>
image = io.imread('b7.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
_ = plt.hist(image.ravel(), bins = 256, color = 'orange', )<br>
_ = plt.hist(image[:, :, 0].ravel(), bins = 256, color = 'red', alpha = 0.5)<br>
_ = plt.hist(image[:, :, 1].ravel(), bins = 256, color = 'Green', alpha = 0.5)<br>
_ = plt.hist(image[:, :, 2].ravel(), bins = 256, color = 'Blue', alpha = 0.5)<br>
_ = plt.xlabel('Intensity Value')<br>
_ = plt.ylabel('Count')<br>
_ = plt.legend(['Total', 'Red_Channel', 'Green_Channel', 'Blue_Channel'])<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/99865138/178968127-aad7a80e-d578-40bd-8efa-b0bfbf45ca89.png)<br>
**************************************************************************************************************<br>
1. Program to perform basic image data analysis using intensity transformation:<br>
a) Image negative<br>
b) Log transformation<br>
c) Gamma correction<br>


%matplotlib inline <br>
import imageio<br>
import matplotlib.pyplot as plt<br>
import warnings<br>
import matplotlib.cbook<br>
warnings.filterwarnings("ignore",category=matplotlib.cbook.mplDeprecation)<br>
pic=imageio.imread('b1.jpg')<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(pic);<br>
plt.axis('off');<br>

![image](https://user-images.githubusercontent.com/99865138/179962090-fa2894ba-eb30-4850-9264-10bb4d423516.png)<br>

negative=255-pic<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(negative);<br>
plt.axis('off');<br>

![image](https://user-images.githubusercontent.com/99865138/179962197-b1c260f8-0251-49a2-b5c7-8098903602bc.png)<br>


%matplotlib inline <br>
import imageio<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
pic=imageio.imread('b1.jpg')<br>
gray=lambda rgb:np.dot(rgb[...,:3],[0.299,0.587,0.114])<br>
gray=gray(pic)<br>

max_=np.max(gray)<br>

def log_transform():<br>
    return(255/np.log(1+max_))*np.log(1+gray)<br>
plt.figure(figsize=(5,5))
plt.imshow(log_transform(),cmap=plt.get_cmap(name='gray'))<br>
plt.axis('off');<br>

![image](https://user-images.githubusercontent.com/99865138/179962276-20b22875-040d-4f43-8845-0c672fad24c6.png)<br>


import imageio<br>
import matplotlib.pyplot as plt<br>
pic=imageio.imread('b1.jpg')<br>
gamma=2.2<br>

gamma_correction=((pic/255)**(1/gamma))<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(gamma_correction)<br>
plt.axis('off');<br>
<br>](https://user-images.githubusercontent.com/99865138/179962347-345e4e8c-d930-42ec-859a-a5899516f191.png)<br>
************************************************************************************************************************
2. Program to perform basic image manipulation:<br>
a) Sharpness<br>
b) Flipping<br>
c) Cropping<br>

from PIL import Image
from PIL import ImageFilter<br>
import matplotlib.pyplot as plt<br>

my_image=Image.open("g1.jfif")<br>

sharp=my_image.filter(ImageFilter.SHARPEN)<br>

sharp.save('D:/image.jpg')<br>
sharp.show()<br>
plt.imshow(sharp)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/99865138/179962514-03c1cd53-1673-486b-9f22-101786fd619e.png)<br>
![image](https://user-images.githubusercontent.com/99865138/179963125-62cb1c40-49bb-4aad-940a-efcbe7266b53.png)<br>


import matplotlib.pyplot as plt<br>
image=Image.open('g1.jfif')<br>
plt.imshow(image)<br>
plt.show()<br>

flip=image.transpose(Image.FLIP_LEFT_RIGHT)<br>

flip.save('D:/image_flip.jpg')<br>
plt.imshow(flip)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/99865138/179962575-b37669eb-b153-4de5-a101-1f3ddd3f028e.png)<br>
![image](https://user-images.githubusercontent.com/99865138/179962656-9e41e532-4b00-4bc6-8fa9-8a571c2e5b51.png)<br>

from PIL import Image<br>
import matplotlib.pyplot as plt<br>
im=Image.open('a1.jpg')<br>
plt.imshow(image)<br>
plt.show()<br>

width,height=im.size<br>
im1=im.crop((50,0,150,125))<br>


im1.show()<br>
plt.imshow(im1)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/99865138/179966759-8d8a25d6-79e3-4ef3-b7b9-42865874f993.png)<br>
***************************************************************************************************************************************<br> 
matrix<br>
**************************************************************************************************************************<br>
from PIL import Image<br>
from numpy import array<br>
im_1 = Image.open(r"a1.jpg")<br>
ar = array(im_1)<br>
ar<br>

array([[[233, 224, 215],<br>
        [233, 224, 215],<br>
        [233, 224, 215],<br>
        ...,<br>
        [219, 211, 200],<br>
        [219, 211, 200],<br>
        [219, 211, 200]],<br>
<br>
       [[230, 221, 212],<br>
        [230, 221, 212],<br>
        [230, 221, 212],<br>
        ...,<br>
        [219, 211, 200],<br>
        [219, 211, 200],<br>
        [219, 211, 200]],<br>

       [[229, 220, 211],<br>
        [229, 220, 211],<br>
        [229, 220, 211],<br>
        ...,<br>
        [218, 210, 199],<br>
        [218, 210, 199],<br>
        [218, 210, 199]],<br>

       ...,<br>

       [[243, 244, 249],<br>
        [243, 244, 249],<br>
        [243, 244, 249],<br>
        ...,<br>
        [239, 239, 239],<br>
        [239, 239, 239],<br>
        [239, 239, 239]],<br>

       [[243, 244, 249],<br>
        [243, 244, 249],<br>
        [243, 244, 249],<br>
        ...,<br>
        [239, 239, 239],<br>
        [239, 239, 239],<br>
        [239, 239, 239]],<br>

       [[244, 243, 249],<br>
        [244, 243, 249],<br>
        [244, 243, 249],<br>
        ...,<br>
        [239, 238, 243],<br>
        [239, 238, 243],<br>
        [241, 240, 245]]],<br> dtype=uint8)<br>
import matplotlib.pyplot as plt <br>
import matplotlib.pyplot as plt <br>
from skimage import io<br>
img=io.imread('b7.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
print('The Shape of the image is:',img. shape)<br>
print('The image as array is:')<br>
print(img)<br>

![image](https://user-images.githubusercontent.com/99865138/180202208-7699f5cb-c328-4f84-8cb9-f0736c958ebd.png)<br>


The Shape of the image is: (183, 275, 3)<br>
The image as array is:<br>
[[[13 14 19]<br>
  [13 14 19]<br>
  [13 14 19]<br>
  ...<br>
  [27 32 10]<br>
  [27 32 10]
  [27 32 10]]<br>
 [[13 14 19]<br>
  [13 14 19]
  [13 14 19]<br>
  ...<br>
  [29 34 12]<br>
  [29 34 12]<br>
  [29 34 12]]<br>

 [[14 15 20]<br>
  [14 15 20]<br>
  [14 15 20]<br>
  ...<br>
  [34 39 17]<br>
  [34 39 17]<br>
  [34 39 17]]<br>

 ...<br>

 [[39 44 22]<br>
  [43 48 26]<br>
  [41 46 26]<br>
  ...<br>
  [71 71 71]<br>
  [75 75 75]<br>
  [81 81 81]]<br>

 [[38 43 21]<br>
  [43 48 26]<br>
  [41 46 26]<br>
  ...<br>
  [78 78 78]<br>
  [80 80 80]<br>
  [83 83 83]]<br>

 [[38 43 21]<br>
  [43 48 26]<br>
  [40 45 25]<br>
  ...<br>
  [85 85 85]<br>
  [84 84 84]<br>
  [82 82 82]]]<br>
from PIL import Image<br>
  
Import an image from directory:<br>
input_image = Image.open("a1.jpg")<br>
  
Extracting pixel map:<br>
pixel_map = input_image.load()<br>
  
Extracting the width and height <br>
of the image:<br>
width, height = input_image.size<br>
  
taking half of the width:<br>
for i in range(width//2):<br>
for j in range(height):<br>
        
 getting the RGB pixel value.<br>
 r, g, b = input_image.getpixel((i, j))<br>
          
Apply formula of grayscale:<br>
grayscale = (0.299*r + 0.587*g + 0.114*b)<br>
  
setting the pixel value.<br>
pixel_map[i, j] = (int(grayscale), int(grayscale), int(grayscale))<br>
  
Saving the final output<br>
as "grayscale.png":<br>
input_image.save("grayscale", format="png")<br>
plt.imshow(input_image)<br>
plt.show()   <br> 
 use input_image.show() to see the image on the<br>
output screen.<br>

![image](https://user-images.githubusercontent.com/99865138/180202299-61bf4dd2-373f-4dda-b2e9-f105d2f39d0b.png)<br>
<br>
from PIL import Image<br>
from PIL import Image<br>
import matplotlib.pyplot as plt<br>  <br>
Create an image as input:<br>
input_image = Image.new(mode="RGB", size=(400, 400),<br>
                        color="blue")<br>
  
 save the image as "input.png"<br>
(not mandatory)<br>
input_image.save("input", format="png")<br>
  
 Extracting pixel map:<br><br>
pixel_map = input_image.load()<br><br>
   Extracting the width and height<br><br>
 of the image:<br><br>
width, height = input_image.size<br><br>
z = 100<br><br>
for i in range(width):<br><br>
    for j in range(height):<br><br>
        
        # the following if part will create<br><br>
        # a square with color orange<br><br>
        if((i >= z and i <= width-z) and (j >= z and j <= height-z)):<br><br>
            
            # RGB value of orange.<br><br>
            pixel_map[i, j] = (255, 165, 255)<br><br>
  
 the following else part will fill the<br><br>
rest part with color light salmon.<br><br>
else:<br><br>
            
RGB value of light salmon.<br><br>
pixel_map[i, j] = (255, 160, 122)<br><br>
  
The following loop will create a cross<br><br>
of color blue.<br><br>
for i in range(width):<br><br>
    
RGB value of Blue.<br><br>
pixel_map[i, i] = (255, 0, 255)<br><br>
pixel_map[i, width-i-1] = (0, 255, 255)<br><br>
  
Saving the final output<br><br>
as "output.png":<br><br>
#input_image.save("output", format="png")<br>
plt.imshow(input_image)<br>
plt.show() <br> 
use input_image.show() to see the image on the<br>
output screen.<br>
![image](https://user-images.githubusercontent.com/99865138/180202373-8aa623ed-e380-4321-a757-fbdc4d6f2d7c.png)<br>
<br>
import numpy as np<br>
import matplotlib.pyplot as plt   <br>
imgsize=(650,650)<br>
image = Image.new('RGBA', imgsize)<br>
innerColor = [153,0,0]<br>
for y in range(imgsize[1]):<br>
 for x in range(imgsize[0]):<br>
distanceToCenter =np.sqrt((x - imgsize[0]/2) ** 2 + (y - imgsize[1]/2) ** 2)<br>
distanceToCenter = (distanceToCenter) / (np.sqrt(2) * imgsize[0]/2)<br>
r = distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
g =  distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
b =  distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
image.putpixel((x, y), (int(r), int(g), int(b)))<br>
        
plt.imshow(image)<br>
plt.show()  <br>

![image](https://user-images.githubusercontent.com/99865138/180202480-c87834c6-60c3-4dfe-8858-3eedeed322fa.png)<br>
<br>
import numpy as np<br>
import matplotlib.pyplot as plt <br>  
imgsize=(650,650)<br>
image = Image.new('RGBA', imgsize)<br>
innerColor = [153,0,0]<br>
for y in range(imgsize[1]):<br>
for x in range(imgsize[0]):<br>
distanceToCenter =np.sqrt((x - imgsize[0]/2) ** 2 + (y - imgsize[1]/2) ** 2)<br>
distanceToCenter = (distanceToCenter) / (np.sqrt(2) * imgsize[0]/2)<br>
r = distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
g =  distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
b =  distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
image.putpixel((x, y), (int(r), int(g), int(b)))<br>
        
plt.imshow(image)<br>
plt.show()  <br>
<br>
plt.imshow(image)<br>
plt.show()  <br>
import numpy as np<br>
import matplotlib.pyplot as plt   <br>
imgsize=(650,650)<br>
image = Image.new('RGBA', imgsize)<br>
innerColor = [255,0,0]<br>
for y in range(imgsize[1]):<br>
    for x in range(imgsize[0]):<br>
         distanceToCenter =np.sqrt((x - imgsize[0]/2) ** 2 + (y - imgsize[1]/2) ** 2)<br>
         distanceToCenter = (distanceToCenter) / (np.sqrt(2) * imgsize[0]/2)<br>
         r = distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
         g =  distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
         b =  distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
         image.putpixel((x, y), (int(r), int(g), int(b)))
        
plt.imshow(image)<br>
plt.show() <br> 

512<br>
from PIL import Image<br>
import matplotlib.pyplot as plt<br>  
import numpy as np<br>
w, h = 512,512<br>
data = np.zeros((h, w, 3), dtype=np.uint8)<br>
data[0:256, 0:256] = [255, 0, 0] <br>
data[256:300,256:300] = [120,200,255] <br>
red patch in upper left<br>
img = Image.fromarray(data, 'RGB')<br>
#img.save('my.png')<br>
#img.show()<br>
plt.imshow(img)<br>
plt.show()<br> <br>
![image](https://user-images.githubusercontent.com/99865138/180202088-5e6410c8-7019-44d9-bd9d-5008d8c0e258.png) <br>
************************************************************************************************* <br>
 <br>
import imageio
import numpy as np <br>
import matplotlib.pyplot as plt <br>
img=imageio.imread('a1.jpg' ) <br>
plt.imshow(img) <br>
plt.show() <br>
max_channels = np.amax([np.amax(img[:,:,0]), np.amax(img[:,:,1]),np.amax(img[:,:,2])]) <br>

print(max_channels) <br>

![image](https://user-images.githubusercontent.com/99865138/181229740-ff083dca-db59-4edc-81d6-86df0cd6725b.png) <br>
![image](https://user-images.githubusercontent.com/99865138/181230371-e6ac4958-6a99-40ac-97fe-e9393adb060e.png) <br>

import imageio <br>
import numpy as np <br>
import matplotlib.pyplot as plt <br>
img=imageio.imread('a1.jpg') <br>
plt.imshow(img) <br>
plt.show() <br>
min_channels = np.amin([np.amin(img[:,:,0]), np.amin(img[:,:,1]), np.amin(img[:,:,2])]) <br>

print(min_channels) <br>

![image](https://user-images.githubusercontent.com/99865138/181229837-072a545c-f416-4ab0-8ef9-83508e54f633.png) <br>
![image](https://user-images.githubusercontent.com/99865138/181230432-832c4759-e1c8-45f1-a237-166c38857377.png) <br>

import cv2 <br>
img=cv2.imread("a1.jpg",0) <br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB) <br>
plt.imshow(img) <br>
np.average(img) <br>


![image](https://user-images.githubusercontent.com/99865138/181229893-6466e627-b7d5-46ca-8f67-4aa4a863f9ab.png) <br>
![image](https://user-images.githubusercontent.com/99865138/181230517-d03355e3-8390-416d-a91d-01a6043889da.png) <br>

from PIL import Image,ImageStat <br>
import matplotlib.pyplot as plt <br>
im=Image.open('a1.jpg')
plt.imshow(im) <br>
plt.show() <br>
stat=ImageStat.Stat(im) <br>
print(stat.stddev) <br>

![image](https://user-images.githubusercontent.com/99865138/181229982-f32251d0-b83c-4a32-98ca-4e25abdc9154.png) <br>
![image](https://user-images.githubusercontent.com/99865138/181230620-564b02b5-9186-4c46-bf86-1604e46adeba.png) <br>
*************************************************************************************************************************<br>
BASIC PILLOW FUNCTION <br>


     from PIL import Image,ImageChops,ImageFilter
     from matplotlib import pyplot as plt<br>
     #create PIL a image object<br>
     x=Image.open("oxx.png")<br>
     o=Image.open("oxo.png")
     #find out attributes if image objects<br>
     print('size of the image:',x.size,'color mode:',x.mode)<br>
     print('size of the image:',o.size,'color mode:',o.mode)<br>
     #plot 2 imageone besides the other<br>
     plt.subplot(121),<br>
     plt.imshow(o)<br>
     plt.axis('off')<br>
     plt.subplot(122),<br>
     plt.imshow(x)
     plt.axis('off')<br>
     #multiply images<br>
     merged=ImageChops.multiply(o,x)<br>
     #adding 2 images<br>
     add=ImageChops.add(o,x)
     #convert color mode<br>
     greyscale=merged.convert('L')<br>
     greyscale<br>
</br>
</br>
   ![image](https://user-images.githubusercontent.com/99865138/187696647-dd3b4ffe-f202-4407-a073-a2e1f838cac1.png)<br>
   ![image](https://user-images.githubusercontent.com/99865138/187696869-26062437-55b2-4110-9d25-80739d36306e.png)
   ![image](https://user-images.githubusercontent.com/99865138/187877724-93a28377-ddb0-4f6c-b80b-ca6b87989177.png)<br>
  
  </br>
  </br>

    #mapping the pixels of the iamge so we can use them as coordinates
    pixel=greyscale.load()<br>
    #a nested loop to parse through all the pixels in the image<br>
    for row in range(greyscale.size[0]):
        for column in range(greyscale.size[1]):<br>
            if pixel[row,column]!=(255):
                pixel[row,column]=(0)<br>
    greyscale<br>

    ![image](https://user-images.githubusercontent.com/99865138/187877824-7b3680d1-040c-46a0-9216-67c03d720bfd.png)
    ![image](https://user-images.githubusercontent.com/99865138/187878787-09daad58-5d47-4ce9-a3d8-f1efa7e34624.png)<br>


    blur=greyscale.filter(ImageFilter.GaussianBlur(radius=1))<br>

    edge=blur.filter(ImageFilter.FIND_EDGES)<br>
    edge<br>
</br>
</br>
![Uploading image.png…]()</br>

   edge=edge.convert('RGB')
   bg_red=Image.new('RGB',(256,256),color=(256,0,0))<br>
<br>
   filled_edge=ImageChops.darker(bg_red,edge)<br>
   filled_edge<br>
   

   ![Uploading image.png…]()<br>
   edge.save('processed.png')<br>

</br>
</br>




*******************************************************************************************************************************************
import numpy as np
import imageio
import matplotlib.pyplot as plt
img=imageio.imread("xox.png")
plt.imshow(img)
plt.show()

mask=imageio.imread("xox.png",0)
plt.imshow(mask)
plt.show()

dst=imageio.inpaint(img,mask,3,imageio.INPAINT_TELEA)

cv2.imwrite("dimage_inpainted.png",dst)
plt.imshow(dst)
plt.show()
![Uploading image.png…]()


removes logo<br>

import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
plt.rcParams['figure.figsize']=(10,8)



import numpy as np
import imageio
import matplotlib.pyplot as plt
img=imageio.imread("imlogo.jpg")
plt.imshow(img)
plt.show()

mask=imageio.imread("imlogo.jpg",0)
plt.imshow(mask)
plt.show()

dst=imageio.inpaint(img,mask,3,imageio.INPAINT_TELEA)

cv2.imwrite("dimage_inpainted.png",dst)
plt.imshow(dst)
plt.show()
import numpy as np
import imageio
import matplotlib.pyplot as plt
img=imageio.imread("imlogo.jpg")
plt.imshow(img)
plt.show()

mask=imageio.imread("imlogo.jpg",0)
plt.imshow(mask)
plt.show()

dst=imageio.inpaint(img,mask,3,imageio.INPAINT_TELEA)

cv2.imwrite("dimage_inpainted.png",dst)
plt.imshow(dst)
plt.show()

![Uploading image.png…]()


import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
plt.rcParams['figure.figsize']=(10,8)

def show_image(image,title='Image',cmap_type='gray'):
    plt.imshow(image,cmap=cmap_type)
    plt.title(title)
    plt.axis('off') 
    
def plot_comparison(img_original,img_filtered,img_title_filtered):
    fig,(ax1,ax2)=plt.subplots(ncols=2,figsize=(10,8),sharex=True,sharey=True)
    ax1.imshow(img_original,cmap=plt.cm.gray)
    ax1.set_title('original')
    ax1.axis('off')
    ax2.imshow(img_filtered,cmap=plt.cm.gray)
    ax2.set_title('img_title_filtered')
    ax2.axis('off')
    
    
    
from skimage.restoration import inpaint
from skimage.transform import resize
from skimage import color


image_with_logo=plt.imread('imlogo.jpg')
mask=np.zeros(image_with_logo.shape[:-1])
mask[210:272,360:425]=1
image_logo_removed=inpaint.inpaint_biharmonic(image_with_logo,mask,multichannel=True)
plot_comparison(image_with_logo,image_logo_removed,'Image with logo removed')

![Uploading image.png…]()



from skimage.util import random_noise
fruit_image=plt.imread('fruits.jpg')
noisy_image=random_noise(fruit_image)
plot_comparison(fruit_image,noisy_image,'noisy image')

#from skimage.restoration import denoise_tv_chambolle
#noisy_image=plt.imread('noisy.jpg')
#denoised_image=denoise_tv_chambolle(noisy_image,multichannel=True)
#plot_comparison(noisy_image,denoised_image,'denoised Image')

![Uploading Screenshot 2022-08-31 224723.png…]()
from skimage.restoration import denoise_tv_chambolle
noisy_image=plt.imread('face.jpg')
denoised_image=denoise_tv_chambolle(noisy_image,multichannel=True)
plot_comparison(noisy_image,denoised_image,'denoised Image')
![Uploading image.png…]()


from skimage.restoration import denoise_tv_chambolle
noisy_image=plt.imread('faceing.jpg')
denoised_image=denoise_bilateral(landscape_image,multichannel=True)
plot_comparison(landscape_image,denoised_image,'denoised Image')


from skimage.segmentation import slic
from skimage.color import label2rgb

face_image=plt.imread('face.jpg')
segment=slic(face_image,n_segments=400)

segment_image=label2rgb(segments,face_image,kind='avg')
plot_comparison(face_image,segmented_image,'segmented image,400 superpixels')


def show_image_counter(image,contours):
    plt.figure()
    for n,contour in enumerate(contours):
        plt.plot(contour[:,1],contour[:,0],linewidth=3)
    plt.imshow(image,interpolation='nearest',cmap='gray_r')
    plt.title('Contours')
    plt.axis('off')
    
    
 from skimage import measure,data

horse_image=data.horse()
contour=measure.find_contours(horse_image,level=0.8)
show_image_contour(horse_image,contours)


shape_contours=[cnt.shape[0] for cnt in contours]
max_dots_shape=50
dots_contours=[cnt for cnt in contours if np.shape(cnt)[0]<max_dots_shape]
show_image_contour(binary,contours)
print('dices dots number:{}.'.format(len(dots_contours)))

