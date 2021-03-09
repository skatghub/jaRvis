# jaRvis
This is my first proJect

/* A Calculator using switch-case statements
 which takes two no input from user and 
display the result*/

#include<stdio.h>
#include<math.h>
#include<conio.h>

float add(float, float);
float sub(float, float);
float mul(float, float);
float div(float, float);
float pow(float, float);
 void print ();
float res;

void main ()
 { 
   int a,b,c;
   a=0; b=0; c=0;
   clrscr();
   cout<<"welcom to jaRvis caLcuLator\n";
   cout<<"Enter the numbers for calculation\n";
   cout<<"Enter A=";
   cin>>a;
   cout<<"\n Enter B=";
   cin>>b;
   cout<<Choose your operation\n";
   cout<<"1-for Addition\n 
          2-for Substraction\n
          3-for Multiplication\n
          4-for Division\n
          5-for Exponential\n";
   cin>>c;
   if(0>=c||c>=6)
      {cout"Not a valid operation, please enter 
         a valid operation";
      cin>>c;
       }
   switch(c)
   case 1:  add(a,b);
   Break;
   case 2:  sub(a,b);
   Break;
   case 3:  mul(a,b);
   Break;
   case 4:  div(a,b);
   Break;
   case 5:  pow(a,b);

   cout<<"The result is="<<res;
   getch();


 }




float add(float x, float y)
 {
  res= x+y;
 }

float sub(float x, float y)
 { if(y>x)
   res= y-x;
   res= x-y;
 }

float mul(float x, float y)
 {
  res= x*y;

 }

float div(float x, float)
 { 
  res= x/y;
 }

float pow(float, float y)
 {
  res= pow(x,y);
 }



