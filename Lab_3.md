<a href="https://ibb.co.com/vJr1yx6"><img src="https://i.ibb.co.com/jLxh0vP/image.png" alt="image" border="0"></a>
----------
## **Experiment No : 01**

## **Experiment Name : Prinitng Diamond**

## **Submission Date : 17 November 2024**

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
            printf("*");
        }
        printf("\n");
    }
    for( int i= rows-1; i>=1; i--)
    {
         for(space=1 ; space<=rows-i ; space++)//If input is 5, then for the 1st line it's (5-1)=4; for 2nd line it's (5-2)=3
        {
            printf(" ");
        }
        for(columns=1; columns<= (2*i-1) ; columns++)//for pyramid colmuns are always (2n-1)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/tQQvy09/image.png" alt="image" border="0"></a>
</p>

----------


## **Experiment No : 02**

## **Experiment Name : Prinitng Pyramid**

## **Submission Date : 17 November 2024**

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
    int rows,space,columns;
    printf("Number of rows you want to print\t");
    scanf("%d",&rows);
    for( int i=1; i<=rows ; i++)
    {
        for(space=1 ; space<=rows-i ; space++)
        {
            printf(" ");
        }
        for(columns=1; columns<= (2*i-1) ; columns++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/KFj6CKJ/image.png" alt="image" border="0"></a>
</p>

--------------


## **Experiment No : 03**

## **Experiment Name : Prinitng Lower part of a diamond**

## **Submission Date : 17 November 2024**

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
    int rows,space,columns;
    printf("Number of rows you want to print\t");
    scanf("%d",&rows);
    for( int i=rows; i>=1 ; i--)
    {
        for(space=1 ; space<=rows-i ; space++)
        {
            printf(" ");
        }
        for(columns=1; columns<= (2*i-1) ; columns++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/k6GMf5h/image.png" alt="image" border="0"></a>
</p>
-----------------

## **Experiment No : 04**

## **Experiment Name : Prinitng Lower part of a diamond**

## **Submission Date : 17 November 2024**

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
    int rows,space,columns;
    printf("Number of rows you want to print\t");
    scanf("%d",&rows);
    for( int i=1; i<=rows ; i++)
    {
        for(columns=1; columns<=i ; columns++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/L03P6k7/image.png" alt="image" border="0"></a>
</p>

-------------------------------


## **Experiment No : 05**

## **Experiment Name : Prinitng Inverted Diamond**

## **Submission Date : 17 November 2024**

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
    int rows,space,columns;
    printf("Number of rows you want to print\t");
    scanf("%d",&rows);
    for( int i=rows; i>=1 ; i--)
    {
        for(space=1 ; space<=rows-i ; space++)
        {
            printf(" ");
        }
        for(columns=1; columns<= (2*i-1) ; columns++)
        {
            printf("*");
        }
        printf("\n");
    }
        for( int i=1; i<=rows ; i++)
    {
        for(space=1 ; space<=rows-i ; space++)
        {
            printf(" ");
        }
        for(columns=1; columns<= (2*i-1) ; columns++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/sFNKP2D/image.png" alt="image" border="0"></a>
</p>
----------------------------

## **Experiment No : 06**

## **Experiment Name : Prinitng a rombhus**

## **Submission Date : 17 November 2024**

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
    int rows,space,columns;
    printf("Number of rows you want to print\t");
    scanf("%d",&rows);
    for( int i=1; i<=rows ; i++)
    {
        for(space=1 ; space<=i ; space++)
        {
            printf(" ");
        }
        for(int j=1; j<=rows; j++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/KG4XxTB/image.png" alt="image" border="0"></a>
</p>
--------------------------------

## **Experiment No : 07**

## **Experiment Name : Prinitng Left Half Pyramid**

## **Submission Date : 17 November 2024**

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
    int rows;
    printf("Number of rows you want to print?\t");
    scanf("%d",&rows);
    for(int i=1; i<=rows; i++)
    {
        for(int space=1; space<=rows-i; space++)
        {
            printf(" ");
        }
        for(int stars=1; stars<=i; stars++)
        {
            printf("*");
        }
        printf("\n");
    }
     return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/GQhdnCW/image.png" alt="image" border="0"></a>
</p>
----------------------------

## **Experiment No : 08**

## **Experiment Name : Prinitng Inverted Left Half Pyramid**

## **Submission Date : 17 November 2024**

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
    int rows;
    printf("Number of rows you want to print?\t");
    scanf("%d",&rows);
    for(int i=1; i<=rows; i++)
    {
        for(int space=1; space<=i; space++)
        {
            printf(" ");
        }
        for(int stars=1; stars<=rows-i; stars++)
        {
            printf("*");
        }
        printf("\n");
    }
     return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/2vP4JH9/image.png" alt="image" border="0"></a>
</p>
----------------------

## **Experiment No : 07**

## **Experiment Name : Prinitng Inverted Right Half Pyramid**

## **Submission Date : 17 November 2024**

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
    int rows;
    printf("Number of rows you want to print?\t");
    scanf("%d",&rows);
    for(int i=1; i<=rows; i++)
    {
        for(int stars=1; stars<=rows-i; stars++)
        {
            printf("*");
        }
        printf("\n");
    }
     return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/N65K164/image.png" alt="image" border="0"></a>
</p>
