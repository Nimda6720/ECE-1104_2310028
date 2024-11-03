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
#include <math.h>
int main() {
    int x1,y1,x2,y2;
    float distance;
    printf("Enter first coordinates: ");
    scanf("%d %d",&x1,&y1);
    printf("Enter second coordinates: ");
    scanf("%d %d",&x2,&y2);
    int X = x2-x1;
    int Y = y2-y1;
    distance = sqrt(pow(X,2) + pow(Y,2));
    printf("Distance: %f\n",distance);
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/fG23Gc2/Distance.png" alt="Distance" border="0"></a>
</p>

-------------


## **Experiment No : 04**

## **Experiment Name : Write a C program that accepts two item's weight and number of purchases (floating point values) and calculates their average value.**


----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Performing the mathematical Operation :** Taking input as axises as input and figuring average using those value.<br>
- **Displaying the Result :** The result can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
#include <math.h>
int main(){
    int i1,i2,n1,n2;
    float average;
    printf("weight and number of purchases of first item\n");
    scanf("%d %d", &i1, &n1);
    printf("weight and number of purchases of second item\n");
    scanf("%d %d", &i2, &n2);
    average=((i1*n1)+(i2*n2))/(n1+n2);
    printf("%f", average);
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/ypnffKX"><img src="https://i.ibb.co.com/3vyrrV7/average-market.png" alt="average-market" border="0"></a>
</p>

## **Discussion :**
<div align="justify">
I couldn't figure out why I wasn't getting decimals after the main value. Though I used float data type for declaring average variable, result was only shown in integer form.
</div>
------------

## **Experiment No : 05**

## **Experiment Name : Check if a given number is prime or not .**


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
#include<stdio.h>
int main(){
   int num,i;
   int prime=1;
   printf("Enter your number\t");
   scanf("%d",&num);
   if (num<=1){
    prime=0;
    }
    else{
        for(i=2; i<=num/2; i++){
            if (num%i==0){
            prime=0;
            break;
        }
      }
    }
    if (prime){
        printf("Number is prime");
        }else{
            printf("Number is not prime");
        }
    return 0;
   }


```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/rMhcmXj/Not-Prime.png" alt="Not-Prime" border="0"></a>
<a href="https://ibb.co.com/PYLTyWD"><img src="https://i.ibb.co.com/Jd1xTp3/Prime.png" alt="Prime" border="0"></a>
</p>
---------------


## **Experiment No : 06**

## **Experiment Name : Add the sum of all even numbers (range:1-100).**


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
int main(){
   int s;
   s=0;
   for(int i=1;i<=100; i++){
    if(i%2==0){
        s+=i;
    }
   }
   printf("The sum is\t%d",s);
   return 0;
   }


```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/mCHD2t1/even-sum.png" alt="even-sum" border="0"></a>
</p>
