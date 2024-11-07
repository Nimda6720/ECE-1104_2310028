----------
## **Experiment No : 01**

## **Experiment Name : Write a C program to make such a pattern like a pyramid with a number which will repeat the number in the same row**

## **Submission Date : 7 November 2024**

----------

## **Theory :**
<div align="justify">

- **Declaring Integer Variables :** Declare integer variables to store integer values. This reserves memory locations for these integers.<br>
- **Taking Input :** Using the scanf function, the program can receive input values from the user. These values are stored in the previously declared integer variables.<br>

</div>

## **Code :**
```C
#include<stdio.h>
int main()
{
    int rows,space,columns;
    printf("Number of rows you want to print\t");
    scanf("%d",&rows);
    for( int i=1; i<=rows ; i++)
    {
        for(space=1 ; space<=rows-i ; space++)//If input is 5, then for the 1st line it's (5-1)=4; for 2nd line it's (5-2)=3
        {
            printf(" ");
        }
        for(columns=1; columns<= (2*i-1) ; columns++)//for pyramid colmuns are always (2n-1)
        {
            printf("%d", i);
        }
        printf("\n");
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/S6T9G8L/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://usefulwebtool.com/'>font style copy paste</a><br />
</p>
