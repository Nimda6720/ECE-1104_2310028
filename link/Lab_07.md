## **Experiment No : 01**

## **Experiment Name :  Write a program in C to add two numbers using pointers.**

## **Submission Date : 5 January 2025**

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

----------
## **Experiment No : 02**

## **Experiment Name : Write a program in C to add three numbers using pointers.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

float sum(float *p1, float *p2, float *p3);

int main(void)
{
    float num1, num2, num3;

    printf("Enter three number: ");
    scanf("%f %f %f",&num1, &num2, &num3);
    printf("Sum: %.2f\n",sum(&num1, &num2, &num3));

}

float sum(float *p1, float *p2, float *p3)
{
    return (*p1 + *p2 + *p3);

}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/P4m7wKY"><img src="https://i.ibb.co.com/RPvxzfS/image.png" alt="image" border="0"></a>
</p>


----------
