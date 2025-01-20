
<a href="https://ibb.co.com/Rp6Dvnn"><img src="https://i.ibb.co.com/rGpw7PP/image.png" alt="image" border="0"></a>
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

## **Submission Date : 20 January 2025**

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

----------
## **Experiment No : 04**

## **Experiment Name : Write a program in C to count the total number of words in a string. **

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    int sum=1;
    char a[]="Blah Blah";
    for ( int i=0; i<sizeof(a); i++)
    {
        if(a[i]==" ")
        {
          sum++;
        }
    }
    printf("Number of words %d", sum+1);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/kBZTGfy/image.png" alt="image" border="0"></a>
</p>

----------
## **Experiment No : 05**

## **Experiment Name : Write a program in C to compare two strings without using string library functions. **

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    int sum=0;
    char a[80];
    char b[80];
    gets(a);
    gets(b);
    for ( int i=0; a[i]!='\0'; i++)
    {
        if (a[i]!=b[i])
        {
            printf("Not Equal");
            return;
        }
    }
    printf ("Equal");
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/MMBKGGn/image.png" alt="image" border="0"></a>
</p>


----------
## **Experiment No : 06**

## **Experiment Name : Write a program in C to count the total number of alphabets, digits and special characters in a string. **

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    int d=0,c=0,sp=0;
    char a[90];
    gets(a);
    //fgets(a,80,stdin);
    //strlwr(a);
    for( int i=0; a[i]!='\0'; i++)
    {
        if (a[i]>='0' &&  a[i]<='9')
        {
            d++;
        }
        else if (a[i]>='a' &&  a[i]<='z')
        {
            c++;
        }
        else
        {
            sp++;
        }
    } 
    printf("Digit: %d\n",d);
    printf("Character: %d\n",c);
    printf("Special Case: %d\n",d);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/yBZ36yS/image.png" alt="image" border="0"></a>
</p>




----------
## **Experiment No : 07**

## **Experiment Name : Write a program in C to copy one string to another string.**

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    int d=0,c=0,sp=0;
    char a[90];
    char b[90];
    gets(a);
    printf("The first string is: %s",a);
    strcpy(b,a);
    printf("\nThe second string is: %s",b);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/NSLBkTN/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>upload foto</a><br />
</p>


----------
## **Experiment No : 08**

## **Experiment Name :Write a program in C to count the total number of vowels or consonants in a string.**

## **Submission Date : 20 January 2025**

----------

## **Code :**
```C
#include<stdio.h>
#include<string.h>

int main()
{
    int v=0,c=0,n=0;
    char a[90];
    gets(a);
    for( int i=0; a[i]!='\0'; i++)
    {
        if (a[i]=='a'|| a[i]=='e'|| a[i]=='i'|| a[i]=='o' || a[i]=='u')
        {
            v++;
        }
    }
     for( int i=0; a[i]!='\0'; i++)
    {    
        if (a[i]>='a' &&  a[i]<='z')
        {
            c++;
        }
    }
    n=c-v;
    printf("Vowel: %d\n",v);
    printf("Consonant: %d\n",n);
    return 0;
}
```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/nCB3Hmx/image.png" alt="image" border="0"></a>
</p>



