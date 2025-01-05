

----------
## **Experiment No : 01**

## **Experiment Name :  Fibonacci sequence.**

## **Submission Date : 9 December 2024**

----------

## **Code :**
```C
#include<stdio.h>

void check(int num);

int num1 = 0;
int num2 = 1;
int num3 = 0;

int main()
{
    int num;
    printf("Enter a number: ");
    scanf("%d",&num);
    printf("0 ");
    printf("1 ");
    check(num-2);
}

void check(int num)
{
    if (num == 0)
    {
        return;
    }
    num3 = num1 + num2;
    printf("%d ", num3);
    num1 = num2;
    num2 = num3;
    check(num-1);
}

```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/mCGyFX4"><img src="https://i.ibb.co.com/Rp964Bc/image.png" alt="image" border="0"></a>
</p>





----------
## **Experiment No : 02**

## **Experiment Name :  A number is prime or not.**

## **Submission Date : 4 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

void prime(int m);

int main()
{
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);

    prime(n);
    return 0;
}


void prime(int m)
{
    if (m <= 1)
    {
        printf("Not prime");
        return;
    }

    for(int i = 2; i < m; i++)
    {
        if (m%i == 0)
        {
            printf("Not prime\n");
            return;
        }
    }
    printf("prime\n");
}


```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/wRSKytR"><img src="https://i.ibb.co.com/g3SDyY3/image.png" alt="image" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'></a><br />
</p>




----------
## **Experiment No : 03**

## **Experiment Name :  Fibonacci sequence & summation.**

## **Submission Date : 4 January 2025**

----------

## **Code :**
```C
#include<stdio.h>

void check(int num);

int array[];

int num1 = 0;
int num2 = 1;
int num3 = 0;

int main(void)
{
    int num;
    printf("Enter a number: ");
    scanf("%d",&num);

    array[num];
    array[num-1] = 0;
    array[num-2] = 1;

    printf("0 ");
    printf("1 ");
    check(num-2);

    printf("\n");
    int sum =0;
    for (int i = 0; i < num; i++)
    {
        sum += array[i];
    }
    printf("\Summation: %d\n", sum);
}

void check(int num)
{
    if (num == 0)
    {
        return;
    }
    num3 = num1 + num2;
    printf("%d ", num3);

    int m = num;
    array[m-1] = num3;

    num1 = num2;
    num2 = num3;
    check(num-1);
}

```

## **Output :**
<p align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co.com/zX52HHL/image.png" alt="image" border="0"></a>
</p>




----------
## **Experiment No : 04**

## **Experiment Name :  Get power of a number using function.**

## **Submission Date : 4 January 2025**

----------

## **Code :**
```C
#include <stdio.h>

int powerf(int base, int power);

int main()
{
    int base, power;
    printf("Enter the base and power: ");
    scanf("%d %d", &base, &power);
    printf("Result: %d\n", powerf(base, power));
    return 0;
}

int powerf(int base, int power)
{
    if (power == 0)
    {
        return 1;
    }
    return base * powerf(base, power - 1);
}


```

## **Output :**
<p align="center">
<a href="https://ibb.co.com/BBZ2ZYJ"><img src="https://i.ibb.co.com/Tt8M8NG/image.png" alt="image" border="0"></a>
</p>
