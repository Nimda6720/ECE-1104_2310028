## **Experiment No : 01**

## **Experiment Name :  Write a program in C to add two numbers using pointers.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

float sum(float *p1, float *p2);

int main()
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

int main()
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

int main()
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

int main()
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

int main()
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
## **Experiment No : 06**

## **Experiment Name : Write a program in C to sort an array using a pointer.**

## **Submission Date : 5 January 2025**

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
<a href="https://ibb.co.com/B6pQVCK"><img src="https://i.ibb.co.com/PWLPZ6z/image.png" alt="image" border="0"></a>
</p>



----------
## **Experiment No : 07**

## **Experiment Name : Write a C program to demonstrate how a function returns a pointer.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

int *sum(int *p1, int *p2);

int main()
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
<a href="https://ibb.co.com/Tq1BbLk"><img src="https://i.ibb.co.com/gFdMPV3/image.png" alt="image" border="0"></a>
</p>



----------
## **Experiment No : 08**

## **Experiment Name :  Write a program in C to compute the sum of all elements in an array using pointers.**

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
void sum(int *p, int n);

int main()
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
<a href="https://ibb.co.com/TbxZLdh"><img src="https://i.ibb.co.com/YyF6Zwj/image.png" alt="image" border="0"></a>
</p>



----------
## **Experiment No : 09**

## **Experiment Name : Write a program in C to print the elements of an array in reverse  order. **

## **Submission Date : 5 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
void reverse(int *p, int n);

int main()
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
<a href="https://ibb.co.com/jVGgDcp"><img src="https://i.ibb.co.com/6vbgF3d/image.png" alt="image" border="0"></a>
</p>




----------
## **Experiment No : 10**

## **Experiment Name : Write a program in C to print all the alphabets using a pointer.**

## **Submission Date : 5 January 2025**

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
<a href="https://ibb.co.com/WgJsPzL"><img src="https://i.ibb.co.com/jgXHWwS/image.png" alt="image" border="0"></a>
</p>



----------

