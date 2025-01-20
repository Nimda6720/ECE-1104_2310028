----------
## **Experiment No : 01**

## **Experiment Name : Write a program in C to find the length of a string without using library functions. **

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    int sum=0;
    char a[]="Blah Blah";
    for ( int i=0; i<sizeof(a); i++)
    {
        sum++;
    }
    printf("%d", sum);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/pJ240V1"><img src="https://i.ibb.co.com/ZWdcL4f/image.png" alt="image" border="0"></a>
</p>

----------
## **Experiment No : 02**

## **Experiment Name :Write a program in C to separate individual characters from a string. **

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    char a[]="Blah Blah";
    for ( int i=0; i<sizeof(a); i++)
    {
        printf("%c\t",a[i]);
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/V9Wq2Rg"><img src="https://i.ibb.co.com/PjZ6wKc/image.png" alt="image" border="0"></a>
</p>

----------
## **Experiment No : 03**

## **Experiment Name : Write a program in C to print individual characters of a string in reverse order. **

## **Submission Date : 13 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    char a[]="Blah Blah";
    for ( int i=sizeof(a); i>=0; i--)
    {
        printf("%c",a[i]);
    }
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/3Rm2n6S"><img src="https://i.ibb.co.com/2Z3xTVc/image.png" alt="image" border="0"></a>
</p>
