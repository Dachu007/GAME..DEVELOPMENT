# EX 7 : THREE DIMENSIONAL TRANSFORMATIONS

## AIM :
 
 To implement the various transformations on three dimensional odjects using a c coding.

## EQUIPMENT REQUIRED:

●	Hardware: Personal Computer (PC)

●	Software: C Compiler

## ALGORITHM :


   Step 1 : Start.

   Step 2 : Draw an image with default parameters.

   Step 3 : Get the choice from user.

   Step 4 : Get the parameters for transformation.

   Step 5 : Perform the transformation.

   Step 6 : Display the output.

   Step 7 : Stop.

## Program :

Name: Dharshini S

Reg No: 212224040074

```
#include<stdio.h> 
#include<conio.h> 
#include<graphics.h> 
#include<math.h> 
int maxx,maxy,midx,midy; 
void axis() 
{ 
getch(); 
cleardevice(); 
line(midx,0,midx,maxy); 
line(0,midy,maxx,midy); 
} 
void main() 
{ 
int gd,gm,x,y,z,o,x1,x2,y1,y2; 
detectgraph(&gd,&gm); 
initgraph(&gd,&gm,"C://TURBOC3//BGI"); 
setfillstyle(0,getmaxcolor()); 
maxx=getmaxx(); 
maxy=getmaxy(); 
midx=maxx/2; 
midy=maxy/2; 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Translation Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("after translation"); 
bar3d(midx+(x+50),midy-(y+100),midx+x+60,midy-(y+90),5,1); 
axis(); 
bar3d(midx+50,midy+100,midx+60,midy-90,5,1); 
printf("Enter Scaling Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("After Scaling"); 
bar3d(midx+(x*50),midy-(y*100),midx+(x*60),midy-(y*90),5*z,1); 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Rotating Angle"); 
scanf("%d",&o); 
x1=50*cos(o*3.14/180)-100*sin(o*3.14/180); 
y1=50*cos(o*3.14/180)+100*sin(o*3.14/180); 
x2=60*sin(o*3.14/180)-90*cos(o*3.14/180); 
y2=60*sin(o*3.14/180)+90*cos(o*3.14/180); 
axis(); 
printf("After Rotation about Z Axis"); 
bar3d(midx+x1,midy-y1,midx+x2,midy-y2,5,1); 
axis(); 
printf("After Rotation about X Axis"); 
bar3d(midx+50,midy-x1,midx+60,midy-x2,5,1); 
axis(); 
printf("After Rotation about Y Axis"); 
bar3d(midx+x1,midy-100,midx+x2,midy-90,5,1); 
getch(); 
closegraph(); 
}

```

## Output :

<img width="646" height="476" alt="Screenshot 2025-10-06 110619" src="https://github.com/user-attachments/assets/2fef4892-1b4f-4309-9183-a8cee2d1e39d" />

<img width="641" height="473" alt="Screenshot 2025-10-06 110630" src="https://github.com/user-attachments/assets/e1ad6191-9edc-4250-8ac2-412cf1fbcc6e" />

<img width="638" height="482" alt="Screenshot 2025-10-06 110649" src="https://github.com/user-attachments/assets/c16bf920-61a3-43b1-888b-ec4cb3e5d0d1" />

<img width="634" height="481" alt="Screenshot 2025-10-06 110701" src="https://github.com/user-attachments/assets/a03932a5-57e0-4383-b58a-96e532a68b12" />

<img width="640" height="469" alt="Screenshot 2025-10-06 110712" src="https://github.com/user-attachments/assets/3fe69316-a772-4a08-a453-073bafefcff2" />

<img width="639" height="470" alt="Screenshot 2025-10-06 110722" src="https://github.com/user-attachments/assets/5d35e69f-37df-450a-af57-ad8a55e60bd1" />

<img width="637" height="477" alt="Screenshot 2025-10-06 110739" src="https://github.com/user-attachments/assets/3bc1266c-2634-42e3-b26e-a30f5daa9e80" />

<img width="637" height="480" alt="Screenshot 2025-10-06 110832" src="https://github.com/user-attachments/assets/1ecc8a87-27ad-4e46-b490-9a08577c8d97" />

## Result :

Thus, the C program for performing three-dimensional transformations — including translation, scaling, and rotation about the X, Y, and Z axes — was successfully implemented and the output was verified through graphical representation.

