# EX-11 - EMI Calculator  
## AIM:  
To write a program to prepare EMI calculator using function without return type and with arguments.

## PROGRAM:
```c
#include <stdio.h>
#include <math.h>
void emi(float p, float r, int t) {
    float amt, emi;
    r = r / (12 * 100);
    amt = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
    printf("EMI is: %.2f\n", amt);
}
int main() {
    float principal, rate;
    int months;
    scanf("%f%f%d", &principal, &rate, &months);
    emi(principal, rate, months);
    return 0;
}
```

## OUTPUT:
```
Input:
50000 10 12
Output:
EMI is: 4395.79
```

## RESULT:  
Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully.


# EX-12 - Fibonacci Series  
## AIM:  
To write a C program to generate the Fibonacci series for the value 6.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int n = 6, t1 = 0, t2 = 1, nextTerm, i;
    printf("%d %d ", t1, t2);
    for (i = 3; i <= n; i++) {
        nextTerm = t1 + t2;
        printf("%d ", nextTerm);
        t1 = t2;
        t2 = nextTerm;
    }
    printf("\n");
    return 0;
}
```

## OUTPUT:
```
Output:
0 1 1 2 3 5
```

## RESULT:  
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.


# EX-13 - One Dimensional Array  
## AIM:  
To write a C program to read n elements as input and print the last element of the array.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int n, i, arr[100];
    scanf("%d", &n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Last element: %d\n", arr[n-1]);
    return 0;
}
```

## OUTPUT:
```
Input:
5
10 20 30 40 50
Output:
Last element: 50
```

## RESULT:  
Thus the program to read n elements as input and print the last element of the array has been executed successfully.


# EX-14 - Positive Array Elements  
## AIM:  
To write a C Program to count total number of positive elements in an array.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int n, arr[100], i, count = 0;
    scanf("%d", &n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total positive elements: %d\n", count);
    return 0;
}
```

## OUTPUT:
```
Input:
6
-3 7 0 5 -1 8
Output:
Total positive elements: 3
```

## RESULT:  
Thus the program to count total number of positive elements in an array has been executed successfully.


# EX-15 - Replace All Even Elements With 'E' in One Dimensional Array  
## AIM:  
To write a C program to replace all even elements with 'E' in one dimensional array.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int n, i, arr[100];
    scanf("%d", &n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    printf("\n");
    return 0;
}
```

## OUTPUT:
```
Input:
5
2 5 8 7 10
Output:
E 5 E 7 E
```

## RESULT:  
Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.
