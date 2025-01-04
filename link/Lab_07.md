
## **Experiment No : 01**

## **Experiment Name :  Write a program in C to add two numbers using pointers.**

## **Submission Date : 15 December 2024**

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
<img src="https://github.com/user-attachments/assets/2230e0cb-825a-48c6-b49a-dd7ebe7ea279">
</p>



----------
## **Experiment No : 02**

## **Experiment Name : Write a program in C to add three numbers using pointers.**

## **Submission Date : 15 December 2024**

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
<img src="https://github.com/user-attachments/assets/715bb5e2-17d2-4db1-9a56-405b7867c124">
</p>


----------
## **Experiment No : 03**

## **Experiment Name :  Write a program in C to find the maximum number between two  numbers using a pointer.**

## **Submission Date : 15 December 2024**

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
<img src="https://github.com/user-attachments/assets/afcf2e4a-4126-464b-989d-0d9ec9e3e63e">
</p>


----------
## **Experiment No : 04**

## **Experiment Name : Write a program in C to store n elements in an array and print the  elements using a pointer.**

## **Submission Date : 15 December 2024**

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
<img src="https://github.com/user-attachments/assets/115ae921-67d6-4b9d-8944-9eca582700a6">
</p>



----------
## **Experiment No : 05**

## **Experiment Name :  Write a program in C to swap elements using call by reference.**

## **Submission Date : 15 December 2024**

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
<img src="https://github.com/user-attachments/assets/39db9fd7-b69e-4ed4-9fac-bff04c7bc576">
</p>



----------
## **Experiment No : 06**

## **Experiment Name : Write a program in C to sort an array using a pointer.**

## **Submission Date : 15 December 2024**

----------

## **Code :**
```C
#include<stdio.h>

void sort(int *p , int n);

int main()
{
    int size;
    printf("Enter the size of an array: ");
    scanf("%d",&size);

    int array[size];
    for (int i = 0; i < size; i++)
    {
        printf("Element_%d: ", i);
        scanf("%d", &array[i]);
    }

    sort(&array[0], size);
}

void sort(int *p , int n)
{
    for (int i = 0; i < n-1; i++)
    {
        for(int j = 0; j < n-1-i; j++)
        {
            if (*(p+j)>*(p+1+j))
            {
                int temp = *(p+j+1);
                *(p+1+j) = *(p+j);
                *(p+j) = temp;
            }
        }
    }

    for (int i = 0; i < n;i++)
    {
        printf("%d ", *(p+i));
    }
}
```

## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/024e2037-d1eb-4dfa-9a8c-affac2204f75">
</p>



----------
## **Experiment No : 07**

## **Experiment Name : Write a C program to demonstrate how a function returns a pointer.**

## **Submission Date : 15 December 2024**

----------

## **Code :**
```C
#include<stdio.h>

int *sum(int *p1, int *p2);

int main(void)
{
    int num1, num2;

    printf("Enter two number: ");
    scanf("%d %d",&num1, &num2);
    int *p = sum(&num1, &num2);

    printf("%d is greater.\n", *p);
}

int *sum(int *p1, int *p2)
{
    if (*p1 > *p2)
    {
        return p1;
    }
    else if (*p1 < *p2)
    {
        return p2;
    }
    printf("Two number are equal\n");
}
```

## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/34e499de-a196-40a5-a5fb-109808f37515">
</p>




----------
## **Experiment No : 08**

## **Experiment Name :  Write a program in C to compute the sum of all elements in an array using pointers.**

## **Submission Date : 15 December 2024**

----------

## **Code :**
```C
#include<stdio.h>
void sum(int *p, int n);

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

    sum(&array[0], n);

}

void sum(int *p, int n)
{
    int sum1=0;
    for (int i = 0; i < n; i++)
    {
        sum1 += *(p+i);
    }

    printf("Sum: %d\n", sum1);
}
```

## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/fd240c58-dcb2-48f9-8124-1392b7ffce26">
</p>




----------
## **Experiment No : 09**

## **Experiment Name : Write a program in C to print the elements of an array in reverse  order. **

## **Submission Date : 15 December 2024**

----------

## **Code :**
```C
#include<stdio.h>
void reverse(int *p, int n);

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

    reverse(&array[n-1], n);
}

void reverse(int *p, int n)
{
    printf("Reverse: ");
    for (int i = 0; i < n; i++)
    {
        printf("%d ",*(p-i));
    }
}
```

## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/ec02eb91-6b85-4695-8715-52d981c2a891">
</p>




----------
## **Experiment No : 10**

## **Experiment Name : Write a program in C to print all the alphabets using a pointer.**

## **Submission Date : 15 December 2024**

----------

## **Code :**
```C
#include<stdio.h>

int main()
{
    int array[26];
    for (int i = 0; i <=25; i++)
    {
        array[i] = 65+i;
    }
    int *p = &array[0];

    for(int i = 0; i <= 25; i++)
    {
        printf("%c ", *(p+i));
    }
    printf("\n");

    int array1[26];
    for (int i = 0; i <=25; i++)
    {
        array[i] = 97+i;
    }
    int *p1 = &array[0];

    for(int i = 0; i <= 25; i++)
    {
        printf("%c ", *(p1+i));
    }

}
```

## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/5e602f3f-8958-42b9-a306-87d551134fb1">
</p>



----------
## **Experiment No : 11**

## **Experiment Name : Access value of 1 and 2 dimensional array using pointer.**

## **Submission Date : 15 December 2024**

----------

## **Code :**
```C
#include<stdio.h>

void print_one();
void print_two();

int main(void)
{
    print_one();
    print_two();
}

void print_one()
{
    int num;
    printf("Enter the length of an array: ");
    scanf("%d", &num);

    int array[num];

    for (int i = 0; i < num; i++)
    {
        printf("element_%d: ", i);
        scanf("%d", &array[i]);
    }
    for (int i = 0; i < num; i++)
    {
        printf("%d ", array[i]);
    }
    printf("\n");
}

void print_two()
{
    int num1, num2;
    printf("Enter length, width of an array: ");
    scanf("%d %d", &num1, &num2);

    int array[num1][num2];

    for (int i = 0; i < num1; i++)
    {
        for (int j = 0; j <num2; j++)
        {
            printf("Enter elements(%d, %d): ", i, j);
            scanf("%d", &array[i][j]);
        }
    }

    printf("\n");

    for (int i = 0; i < num1; i++)
    {
        for (int j = 0; j <num2; j++)
        {
            int *p = &array[i][j];
            printf("%d ", *p);
        }
        printf("\n");
    }
}
```

## **Output :**
<p align="center">
<img src="https://github.com/user-attachments/assets/6a33761a-1b57-4747-aec7-52a2d72bf8ee">
</p>
