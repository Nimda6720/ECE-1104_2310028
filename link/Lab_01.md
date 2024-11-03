----------
## **Experiment No : 01**

## **Experiment Name : Write a C program that accepts two integers from the user and calculates the sum of the two integers.**

## **Submission Date : 3 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the Addition Operation :** Add the two integers using the + operator, which is the arithmetic operator in C for addition.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
int main(){
int num1,num2,sum;
printf("Enter two numbers\n");
scanf("%d%d",&num1,&num2);
sum=num1+num2;
printf("The sum is\t%d",sum);
return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/Rv1ZJqL/Screenshot-2024-11-03-160447.png" alt="Screenshot-2024-11-03-160447" border="0"></a>
</p>


## **Discussion :**
<div align="justify">
Input and Output : scanf to take two integer inputs and printf to display the result.<br>
Arithmetic Operation : A simple addition operation using the variables a and b.<br>
Format Specifiers : %d handle integer values for both input and output.<br>
</div>

## **Conclusion :**
<div align="justify">
The program effectively sums up two numbers”<br>
</div>
----------



## **Experiment No : 02**

## **Experiment Name : Write a C program to convert specified days into years, weeks and days (Note: Ignore leap year.).**


----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the mathematical Operation :** Taking input as dates converting it into day,weeks,years.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
#include <math.h>
int main(){
int d,w,y,r;
printf("Enter the number of days\t");
scanf("%d",&d);
y=d/365;
w=(d%365)/7;
r=(d%365)%7;
printf("%d number of year\n",y);
printf("%d number of weeks\n",w);
printf("%d number of days\n",r);
return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/g96JcsD/year-converter.png" alt="year-converter" border="0"></a>
</p>

--------------


## **Experiment No : 03**

## **Experiment Name : Write a C program to calculate the distance between two points..**


----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the mathematical Operation :** Taking input as axises as input and figuring distance using those value.<br>
- **Displaying the Result :** The result can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
#include<math.h>
int main(){
printf("enter first co-ordinates\n");
int X,Y,x1,y1,x2,y2;
float distance;
X=x2-x1;
Y=y2-y1;
scanf("%d%d",&x1,&y1);
printf("enter second co-ordinates\n");
scanf("%d%d",&x2,&y2);
distance=sqrt(pow(X,2)+pow(Y,2));
printf("%f",distance);
return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/tbGv1Mt/distance.png" alt="distance" border="0"></a>
</p>
