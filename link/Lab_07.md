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
<a href="https://ibb.co.com/87S0mpz"><img src="https://i.ibb.co.com/FDjKhMs/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'></a><br />
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
## **Experiment No : 03**

## **Experiment Name :  Write a program in C to find the maximum number between two  numbers using a pointer.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

int sum(float *p1, float *p2);

int main(void)
{
    float num1, num2;

    printf("Enter two number: ");
    scanf("%f %f",&num1, &num2);
    sum(&num1, &num2);
}

int sum(float *p1, float *p2)
{
    if (*p1 > *p2)
    {
        printf("%.2f is greater than %.2f\n", *p1, *p2);
    }
    else if (*p1 < *p2)
    {
        printf("%.2f is greater than %.2f\n", *p2, *p1);
    }
    else{
        printf("Two numbers are equal\n");
    }
    return 0;

}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/DGvp6Kv"><img src="https://i.ibb.co.com/4sXdDNX/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://dedupelist.com/'></a><br />
</p>


----------
## **Experiment No : 04**

## **Experiment Name : Write a program in C to store n elements in an array and print the  elements using a pointer.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

void print(int *p, int n);

int main(void)
{
    int n;
    printf("Enter the size of array: ");
    scanf("%d", &n);

    int array[n];
    for (int i = 0; i < n; i++)
    {
        printf("Element_%d: ", i);
        scanf("%d", &array[i]);
    }

    print(&array[0], n);


}

void print(int *p,int n)
{
    for (int i = 0; i < n; i++)
    {
        printf("%d ", *(p+i));

    }
}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/MDqB979"><img src="https://i.ibb.co.com/JRX3CHC/image.png" alt="image" border="0"></a>
</p>



----------
## **Experiment No : 05**

## **Experiment Name :  Write a program in C to swap elements using call by reference.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

int swap(int *p1, int *p2);

int main(void)
{
    int num1, num2;

    printf("Enter two number: ");
    scanf("%d %d",&num1, &num2);

    swap(&num1, &num2);
}

int swap(int *p1, int *p2)
{
    int temp = *p1;
    *p1 = *p2;
    *p2 = temp;
    printf("%d %d\n",*p1, *p2);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/PN5TvGC"><img src="https://i.ibb.co.com/565Yghc/image.png" alt="image" border="0"></a>
</p>



----------
