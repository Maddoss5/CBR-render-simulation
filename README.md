# CBR-render-simulation
Checkerboard rendering or sparse rendering, also known as checkerboarding for short, is a 3D computer graphics rendering technique, intended primarily to assist graphics processing units with rendering images at high resolutions. It is different from tiled rendering, a method of subdividing images in order to render them more efficiently, and from the "checkerboard" method of alternate frame rendering.

Original image 
![93457775_p0](https://user-images.githubusercontent.com/111579172/185630490-79635e07-ae55-4c4e-8e55-603d8329b9e2.jpg)


# Basic understanding
In checkerboard rendering we render every alternate pixel and leave the other one blank or with some random color .Using CBR we reduce the load on graphical processing unit as we basically half the number of pixels to be rendered . CBR render can be godsend for people with lower end computers and still manage to run application with high graphic processing 

In my experiment when i colored the alternate pixel with black this was the result -
![FirstCBR](https://user-images.githubusercontent.com/111579172/185630556-e5c68332-5827-4c15-b848-2ae7b5affd93.jpg)


# Upgrade
Now instead of coloring the alternate pixel with black if you take the average of all the surrounding pixel you get a much more cleaner image which is almsot indistinguishable from the original image when looked at from far view . 
Here in my project i averaged the surrounding pixel and this was the result .

Original image-![93457775_p0](https://user-images.githubusercontent.com/111579172/185630976-dbd5309b-914d-4f39-a4f7-c918004ff14b.jpg) 
CBR render ![FinalCBR](https://user-images.githubusercontent.com/111579172/185630994-b3040189-efdc-41c8-8a41-171207858004.jpg)

# Problem arising with CBR 
Although from a far distance the two images look near identical , from closer inspection we can see CBR versoin has much more noise than the original image . One such example is posted here 

Original image -![original image better details](https://user-images.githubusercontent.com/111579172/185631380-2d1ed843-6df7-4b16-ad78-db45edb04570.png)
CBR version- ![CBR version messy details](https://user-images.githubusercontent.com/111579172/185631412-677a828c-accc-4469-a184-82d1d2ec039a.png)

The noise in CBR version should be really clear when done a closer inspection . 

# Further work
The modern way for CBR render is to use vectors for each pixel and predict what direction they are goign in .

