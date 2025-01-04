## **Experiment No : 01**

## **Experiment Name :  Write a program in C to add two numbers using pointers.**

## **Submission Date : 5 January 2024**

----------

## **Code :**
```C
#include<stdio.h>

float sum(float *p1, float *p2);

int main(void)
{
    float num1, num2;

    printf("Enter two number: ");
    scanf("%f %f",&num1, &num2);

    printf("Sum: %.2f\n", sum(&num1, &num2));
    return 0;
}

float sum(float *p1, float *p2)
{
    return *p1 + *p2;
}


```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/87S0mpz"><img src="https://i.ibb.co.com/FDjKhMs/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>upload</a><br />
</p>

