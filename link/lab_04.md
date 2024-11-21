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

