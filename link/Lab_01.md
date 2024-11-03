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
