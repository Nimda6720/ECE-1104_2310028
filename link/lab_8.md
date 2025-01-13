
<h>Problems From previous Lab: </h>
## **Experiment No : 01**

## **Experiment Name :  Write a program in C to compute the sum of all elements in an array using pointers.**

## **Submission Date : 13 January 2025**

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
## **Experiment No : 02**

## **Experiment Name : Write a program in C to print the elements of an array in reverse  order. **

## **Submission Date : 13 January 2025**

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


New Problems:
-------------------

## **Experiment No : 01**

## **Experiment Name :  Write a program in C to sort all elements in an array using pointers.**

## **Submission Date : 13 January 2025**

----------

## **Code :**
```C
#include <stdio.h>
void sort(int *p, int n);
int main()
{ 
  int n;
  printf("Number of inputs: ");
  scanf("%d", &n);
  int a[n];
  for (int i=0; i<n; i++)
  {
    printf("Element_%d: ", i);
    scanf("%d", &a[i]);
  }
  sort(&a[0],n);
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
    printf ("The elements of array after printing\n");
    for (int i = 0; i < n;i++)
    {
        printf("\nElement_%d:",i);
        printf("%d ", *(p+i));
    }
}

```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/nmJw560"><img src="https://i.ibb.co.com/zxvm0Q5/image.png" alt="image" border="0"></a>
</p>

------------------------

-------------------

## **Experiment No : 01**

## **Experiment Name :  Write a program in C to sort all elements in an array using pointers.**

## **Submission Date : 13 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
int gcd( int m, int n);
int main()
{
    int r,m,n;
    printf("Enter two numbers:");
    scanf("%d %d",&m,&n);
    printf("The gcd is %d",gcd(m,n));
    return 0;
}
int gcd( int m, int n)
{
    if(n==0)  
        return m;
    else 
    return gcd(n, m%n);
}

```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/fqVLqhY"><img src="https://i.ibb.co.com/wBZjB9N/image.png" alt="image" border="0"></a>
</p>
