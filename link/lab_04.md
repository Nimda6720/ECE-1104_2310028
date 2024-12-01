----------
## **Experiment No : 01**

## **Experiment Name : Write a program in C to copy the elements of one array into another array. 

Test Data : 
Input the number of elements to be stored in the array :3 
Input 3 elements in the array : 
element - 0 : 15 
element - 1 : 10 
element - 2 : 12 
Expected Output : 
The elements stored in the first array are : 
15 10 12 
The elements copied into the second array are : 
15 10 12 
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
int main()
{
    int n;
    printf("Numbers of number you want to input:  ");
    scanf("%d",&n);
    int a1[n],a2[n];
    for (int i=0; i<n; i++)
    {
        printf("Element %d: ",i);
        scanf("%d",&a1[i]);
        a2[i]=a1[i];
    }
           printf("Numbers of first array are: \n");
    for (int i=0; i<n; i++)
    {
        printf("%d ",a1[i]);
    }
            printf("\nNumbers of second array are: \n");
    for (int i=0; i<n; i++)
    {
        printf("%d ",a2[i]);
    }        
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/Db1KG8M/image.png" alt="image" border="0"></a>
</p>

------------------------------------------------------------


----------
## **Experiment No : 02**

## **Experiment Name :Write a program in C to count the total number of duplicate elements in an array.


Test Data : 
Input the number of elements to be stored in the array :3 
Input 3 elements in the array : 
element - 0 : 5 
element - 1 : 1 
element - 2 : 1 
Expected Output : 
Total number of duplicate elements found in the array is : 1 

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
int main()
{
    int n,a1[10],count=0;
    printf("Enter the number of inputs you want to take: ");
    scanf("%d",&n);
    for(int i=0; i<n; i++)
    {
        printf("Element %d:",i);
        scanf("%d",&a1[i]);
    }
    for(int i=0; i<n; i++)
    {
        for( int j=i+1; j<n; j++)
        {
            if( a1[i] == a1[j])
            {
                count++;
                break;
            }
        }
    }
    printf("Number of duplicates %d",count);
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/87xThhY/image.png" alt="image" border="0"></a>
</p>

------------------------------------

## **Experiment No : 03**

## **Experiment Name : Write a program in C to print all unique elements in an array. 

Test Data : 
Print all unique elements of an array: 
------------------------------------------ 
Input the number of elements to be stored in the array: 4 
Input 4 elements in the array : 
element - 0 : 3 
element - 1 : 2 
element - 2 : 2 
element - 3 : 5 
Expected Output : 
The unique elements found in the array are: 
3 5 

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
int main()
{
    int n;
    printf("Number of inputs? : ");
    scanf("%d",&n);
    int a[n];
    for(int i=0; i<n; i++)
    {
        printf("Element %d- ",i);
        scanf("%d",&a[i]);
    }
    for(int i=0; i<n; i++)
    {
        for(int j=i+1; j<n; j++)
        {
            if(a[i]== a[j])
            {
                a[i]=0;
                a[j]=0;
            }
        }
    }
    printf("Unique Elements are: ");
       for(int i=0; i<n; i++)
       {
        if(a[i]!=0)
        {
            printf("%d ",a[i]);
        }
       }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/xSZ3vyF/image.png" alt="image" border="0"></a>
</p>
-------------------------------------


## **Experiment No : 05**

## **Experiment Name :Write a program in C to separate odd and even integers into separate arrays. 

Test Data : 
Input the number of elements to be stored in the array :5 
Input 5 elements in the array : 
element - 0 : 25 
element - 1 : 47 
element - 2 : 42 
element - 3 : 56 
element - 4 : 32 
Expected Output : 
The Even elements are : 
42 56 32 
The Odd elements are : 
25 47 

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
int main()
{
    int n;
    printf("Number of inputs? : ");
    scanf("%d",&n);
    int a[n];
    for(int i=0; i<n; i++)
    {
        printf("Element %d- ",i);
        scanf("%d",&a[i]);
    }
    
    printf("The even Elements are:\n");
    for(int i=0; i<n; i++)
    {
        if( a[i]%2 == 0)
        {
          printf("%d ",a[i]);
        }
    }
        printf("\nThe odd Elements are:\n");
    for(int i=0; i<n; i++)
    {
        if( a[i]%2 >= 1 )
        {
          printf("%d ",a[i]);
        }
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/xFx1Vp7/image.png" alt="image" border="0"></a>
</p>
------------------------------------

## **Experiment No : 06**

## **Experiment Name : Write a program in C to find the smallest missing element in a sorted array. Expected Output : 
The given array is : 0 1 3 4 5 6 7 9 
The missing smallest element is: 2 
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
#include<stdio.h> //a[i]!=i, print i, break.
int main()
{
    int n;
    printf("Number of inputs? : ");
    scanf("%d",&n);
    int a[n];
    for(int i=0; i<n; i++)
    {
        printf("Element %d- ",i);
        scanf("%d",&a[i]);
    }
    printf("The missing smallest elemnt is:\n");
    for(int i=0; i<n; i++)
    {
        if (a[i]!=i)
        {
            printf("%d",i);
            break;
        }
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/QrNbGgS/image.png" alt="image" border="0"></a>
</p>

-----------------------------------------


## **Experiment No : 07**

## **Experiment Name : Write a program in C to sort an array of 0s, 1s and 2s. 

Expected Output : 
The given array is : 0 1 2 2 1 0 0 2 0 1 1 0 
After sorting the elements in the array are: 
0 0 0 0 0 1 1 1 1 2 2 2 

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
int main()
{
    int n;
    printf("Enter the number of inputs you want to take: ");
    scanf("%d",&n)
    int a[n];
    for(int i=0; i<n; i++)
    {
        printf("Element %d: ",i);
        scanf("%d",&a1[i]);
    }
     printf("After Sorting: ");
    for(int i=0; i<n; i++)
    {
        for( int j=i+1; j<n; j++)
        {
            if( a1[i]>a1[j] )
            {
                int temp= a1[i];
                a1[i]=a1[j];
                a1[j]= temp;
            }
        }
       printf("%d ",a1[i]);
    }
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/WFvFZWV/image.png" alt="image" border="0"></a>
</p>

-------------------------------

## **Experiment No : 04**

## **
Write a program in C to count the frequency of each element of an array. Test Data : 
Input the number of elements to be stored in the array :3 
Input 3 elements in the array : 
element - 0 : 25 
element - 1 : 12 
element - 2 : 43 
Expected Output : 
The frequency of all elements of an array : 
25 occurs 1 times 
12 occurs 1 times 
43 occurs 1 times


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
int main()
{
    int input,count;
    printf("Number of Elemnets you want to input: ");
    scanf("%d",&input);
    
    int a[input],fre[input];
    
    for (int i=0; i<input; i++)
    {
        printf("Elements -%d: ",i);
        scanf("%d",&a[i]);
        fre[i]=-1;
    }

    for (int i=0; i<input; i++)
    {
        count=1;
        for (int j=i+1; j<input; j++)
        {
            if(a[i]==a[j])
            { 
                count++;
                fre[j]=0;
            }
        }
        if (fre[i]!=0)
        {
          fre[i]=count;
        }
    }
    
    printf("The frequency of all the elements of an array\n");
    for (int i=0; i<input; i++)
    {
      if(fre[i]!=0)
        {  
         printf("%d occurs %d times\n",a[i],fre[i]);
        }
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/DQVnJ7p/image.png" alt="image" border="0"></a>
</p>
---------------------------

## **Experiment No : 08**

## **Write a program in C to insert the values in the array (sorted list). Test Data : 
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
int main()
{
    int input;
    printf("Number of inputs: ");
    scanf("%d",&input);
    int a[input+1];
    for (int i=0; i<input; i++)
    {
        printf("Elements-%d: ",i);
        scanf("%d",&a[i]);
    }
    int insert;
    printf("Value to be inserted: ");
    scanf("%d",&insert);
    
    printf("The existing list of array is:\n");
    for (int i=0; i<input; i++)
    {
        printf("%d ",a[i]);
    }
    
    int i=input-1;
    while(i>=0 && a[i]>insert)
    {
        a[i+1]=a[i];
        i--;
    }
    a[i+1]=insert;
    
    printf("\nafter insert:\n");
    for (int i=0; i<input+1; i++)
    {
        printf("%d ",a[i]);
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/wK6y0FP/image.png" alt="image" border="0"></a>
</p>

