# CBR-render-simulation
Checkerboard rendering or sparse rendering, also known as checkerboarding for short, is a 3D computer graphics rendering technique, intended primarily to assist graphics processing units with rendering images at high resolutions. It is different from tiled rendering, a method of subdividing images in order to render them more efficiently, and from the "checkerboard" method of alternate frame rendering.

Original image 
![93457775_p0](https://user-images.githubusercontent.com/111579172/185630490-79635e07-ae55-4c4e-8e55-603d8329b9e2.jpg)


# Basic understanding
In checkerboard rendering we render every alternate pixel and leave the other one blank or with some random color .Using CBR we reduce the load on graphical processing unit as we basically half the number of pixels to be rendered .

In my experiment when i colored the alternate pixel with black this was the result -
![FirstCBR](https://user-images.githubusercontent.com/111579172/185630556-e5c68332-5827-4c15-b848-2ae7b5affd93.jpg)


# Upgrade
Now instead of coloring the alternate pixel with black if you take the average of all the surrounding pixel you get a much more cleaner image which is almsot indistinguishable from the original image when looked at from far view . 
Here in my project i averaged the surrounding pixel and this was the result .

Original image-![93457775_p0](https://user-images.githubusercontent.com/111579172/185630976-dbd5309b-914d-4f39-a4f7-c918004ff14b.jpg) ![FinalCBR](https://user-images.githubusercontent.com/111579172/185630994-b3040189-efdc-41c8-8a41-171207858004.jpg)


