<a href="https://ibb.co.com/dMqy78h"><img src="https://i.ibb.co.com/9gLjGQM/image.png" alt="image" border="0"></a>
----------
## **Experiment No : 01**

## **Experiment Name : Use three separate function to
a) take input from a 1d array,
b) sum the elements and
c) show the sum and elements
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>

void in(int ar[], int n)//this order is important. Don't know why but sometimes code doesn't work if you don't put them in this order
{
    for(int i=0; i<n; i++)
    {
      scanf("%d",&ar[i]);
    }
}
void out(int ar[], int n)
{
    for(int i=0; i<n; i++)
    {
      printf("%d\t",ar[i]);
    }
}
int su(int ar[], int n, int sum)
{
    for(int i=0; i<n; i++)
    {
      sum+= ar[i];
    }
    printf("\nSum of all the elements: %d",sum);
    return sum;
}
int main()
{
    int n,sum=0;
    printf("Number of input? ");
    scanf("%d",&n);
    int ar[n];
    in(ar,n);
    out(ar,n);
    su(ar,n,sum);
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/JQymzxM/image.png" alt="image" border="0"></a>
</p>

-----------------------------------------

----------
## **Experiment No : 02**

## **Experiment Name :
For 2d Array:
 Use three separate function to
a) take input from a 2d array,
b) sum the elements and
c) show the sum and elements
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
void in( int n, int a, int ar[n][a])//for 2d array: first put int variables then the arrays in this format
{
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         scanf("%d",&ar[i][j]);
        }
    }
}
void out(int n, int a, int ar[n][a])
{
    printf("Output: \n");
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         printf("%d ",ar[i][j]);
        }
        printf("\n");
    }
    printf("\n");
}
int sum(int n, int m, int arr[n][m])
{
    int total = 0;
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < m; j++)
        {
            total += arr[i][j];
        }
    }
    return total;
}
int main()
{
    int n,a;
    printf("Number of rows? ");
    scanf("%d",&n);
    printf("Number of columns? ");
    scanf("%d",&a);
    int ar[n][a];
    in(n,a,ar);
    out(n,a,ar);
    printf("sum : %d\n", sum(n, a, ar));
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/VMF60BN/image.png" alt="image" border="0"></a>
</p>

----------------------------



## **Experiment No : 03**

## **Experiment Name : Write a program in C to swap two numbers using a function.
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
void in(int ar[], int n)
{
    for(int i=0; i<n; i++)
    {
      scanf("%d",&ar[i]);
    }
}

void sort(int ar[], int n)
{
   for(int i = 0; i < n - 1; i++)
   {
      for(int j = 0; j < n - i - 1; j++)
      {
         if(ar[j] > ar[j+1])
         {
            int temp = ar[j];
            ar[j] = ar[j+1];
            ar[j+1] = temp;
         }
      }
   }
}

void printArray(int ar[], int n)
{
   for(int i = 0; i < n; i++)
   {
      printf("%d ", ar[i]);
   }
}

int main()
{
    int n;
    printf("Number of input? ");
    scanf("%d",&n);
    int ar[n];
    in(ar,n);
    sort(ar,n);
    printArray(ar, n);

   return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/vBZ6MCD/image.png" alt="image" border="0"></a>
</p>

---------------------------------------

----------
## **Experiment No : 04**

## **Experiment Name : Write a program in C to check if a given number is even or odd using the
function.**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include<stdio.h>
void number(int ar[], int a)
{
    for(int i=0; i<a; i++)
    {
        scanf("%d", &ar[i]);
    }
}
void print(int ar[],int a)
{
       printf("Even: ");
        for(int i=0; i<a; i++)
    {
        if(ar[i]%2==0)
        {
            printf("%d ",ar[i]);
        }
    }
       printf ("\nodd: ");
        for(int i=0; i<a; i++)
        {
         if (ar[i]%2>0)
        {
            printf("%d ",ar[i]);
        }
        }
    }
int main()
{
 int a;
 printf("Number of inputs: ");
 scanf("%d",&a);
 int ar[a];
 number(ar,a);
 print(ar,a);
 return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/7YC4QMn/image.png" alt="image" border="0"></a>
</p>

---------------------------------

----------
## **Experiment No : 05**

## **Experiment Name : Write a program in C to get the largest element of an array using the
function.
Test Data :
Input the number of elements to be stored in the array :5
Input 5 elements in the array :
element - 0 : 1
element - 1 : 2
element - 2 : 3
element - 3 : 4
element - 4 : 5
Expected Output :
The largest element in the array is : 5
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include<stdio.h>
void in(int a, int ar[])
{
  for(int i=0; i<a; i++)
  {
      printf("Element-%d: ",i);
      scanf("%d", &ar[i]);
  }
}
void sort(int a, int ar[])
{
    for( int i=0; i<a; i++)
    {
        for ( int j=0; j<a; j++)
        {
            if(ar[j]>ar[j+1])
            {
            int temp = ar[j];
            ar[j] = ar[j+1];
            ar[j+1] = temp;
            }
        }
    }
}
void print(int a, int ar[])
{
    printf("Largest Elements: %d",ar[a-1]);
}

int main()
{
 int a;
 printf("Number of inputs: ");
 scanf("%d",&a);
 int ar[a];
 in(a,ar);
 sort(a,ar);
 print(a,ar);
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/xLtp3R6/image.png" alt="image" border="0"></a>
</p>
---------------------------------------

## **Experiment No : 07**

## **Experiment Name : Write a C program to find the maximum and minimum of some values using
a function that returns an array.
Test Data :
Input 5 values
25
11
35
65
20
Expected Output :
Number of values you want to input: Input 5 values
Minimum value is: 11
Maximum value is: 65
**

## **Submission Date : 22 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include<stdio.h>
void in(int a, int ar[])
{
  for(int i=0; i<a; i++)
  {
      printf("Element-%d: ",i);
      scanf("%d", &ar[i]);
  }
}
void sort(int a, int ar[])
{
    for( int i=0; i<a; i++)
    {
        for ( int j=0; j<a; j++)
        {
            if(ar[j]>ar[j+1])
            {
            int temp = ar[j];
            ar[j] = ar[j+1];
            ar[j+1] = temp;
            }
        }
    }
}
void print(int a, int ar[])
{
    printf("Maximum Value is: %d",ar[a]);
    printf("\nMinimum Value is: %d",ar[0]);
}

int main()
{
 int a;
 printf("Number of inputs: ");
 scanf("%d",&a);
 int ar[a];
 in(a,ar);
 sort(a,ar);
 print(a,ar);
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/Pwk7Cnz/image.png" alt="image" border="0"></a>
</p>

------------------------------

## **Experiment No : 08**

## **Experiment Name :

Write a program in C to insert the values in the array using function(sorted
list).
Test Data :
Input number of elements you want to insert (max 100): 5
Input 5 elements in the array in ascending order:
element - 0 : 2
element - 1 : 3
element - 2 : 4
element - 3 : 7
element - 4 : 8
Input the value to be inserted : 5
The existing array list is :
2 3 4 7 8
After Insert the list is :
2 3 4 5 7 8
**

## **Submission Date : 1 December 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include<stdio.h>

void in(int input,int a[])
{
    for (int i=0; i<input; i++)
    {
        printf("Element -0%d: ",i);
        scanf("%d",&a[i]);
    }
} 

void ins(int insert)
{
    printf("Value to be inserted: ");
    scanf("%d", insert);
}

void out1(int input,int a[])
{
    printf("The number of existing array list is:\n");
    for (int i=0; i<input; i++)
    {
        printf("%d ",a[i]);
    }
    printf("\n");
}

void sort(int input,int a[],int insert)
{ 
    int i=input-1;
    while(i>=0 && a[i]>insert)
    {
        a[i+1]=a[i];
        i--;
    }   
    a[i+1]=insert;
}

void out2(int input, int a[])
{   
    printf("\nAfter insert the list is: \n");
    for (int i=0; i<input+1; i++)
    {
       printf("%d ",a[i]);
    }
    printf("\n");
}

int main()
{
    int input,insert;
    printf("Number of inputs: ");
    scanf("%d",&input);
    int a[input+1];
    in(input,a);
    ins(&insert);
    out1(input,a);
    sort(input,a,insert);
    out2(input,a);
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/7NzCNDp/image.png" alt="image" border="0"></a>
</p>

----------------------

## **Experiment No : 08**

## **Experiment Name :
Write a C program to perform the following operations on two n ×m
matrices using functions:
a) Addition
b) Subtraction

**

## **Submission Date : 1 December 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>
- **Displaying the Result :** The result of the addition can be displayed using the printf function.  <br>

</div>

## **Code :**
```C
#include <stdio.h>
void in( int n, int a, int ar[n][a])
{
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         scanf("%d",&ar[i][j]);
        }
    }
    printf("\n");
}

void in2( int n, int a, int ar2[n][a])
{
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         scanf("%d",&ar2[i][j]);
        }
    }
    printf("\n");
}

void result( int n, int a,int ar[n][a],int ar2[n][a],int res[n][a])
{
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         res[i][j]=ar[i][j] + ar2[i][j];
        }
    }
}

void out( int n, int a, int res[n][a])
{
    printf("Result of addition:\n");
    for(int i=0; i<n; i++)
    {
        for(int j=0; j<a; j++)
        {
         printf("%d ",res[i][j]);
        }
        printf("\n");
    }
}

int main()
{
    int n,a;
    printf("Number of rows? ");
    scanf("%d",&n);
    printf("Number of columns? ");
    scanf("%d",&a);
    int ar[n][a];
    int ar2[n][a];
    int res[n][a];
    in(n,a,ar);
    in2(n,a,ar2);
    result(n,a,ar,ar2,res);
    out(n,a,res);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/pvWRMyb/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>a image</a><br />
</p>




