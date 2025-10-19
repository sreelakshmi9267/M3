# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function with return type and without arguments.

## ALGORITHM

1. Start the program.
2. Define a function with return type and without arguments.
3. Inside the function, read principal amount, rate of interest, and number of months.
4. Calculate EMI using the formula:
5. return the calculated emi value to the main function.
6. In the main function, receive the returned EMI value and display the result.
7. Stop the program.

## PROGRAM
```
#include <stdio.h>
#include<math.h>
void emi(void);
int main()
{
    emi();
    return 0;
}
void emi()
{
    float p,r,t,emi;
    scanf("%f%f%f",&p,&r,&t);
    r=r/(12*100);
    t=t*12;
    emi=(p*r*pow(1+r,t))/(pow(1+r,t)-1);
    printf("Monthly EMI is= %.3f",emi);
}
```

## OUTPUT
![alt text](<output 1.png>)


## RESULT

Thus the program to prepare EMI calculator using function with return type without arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n = 6;
    int first = 0, second = 1, next, i;

    printf("Fibonacci series for %d terms:\n", n);

    for(i = 1; i <= n; i++) {
        printf("%d ", first);
        next = first + second;
        first = second;
        second = next;
    }

    return 0;
}

```

## OUTPUT
![alt text](<output 2.png>)


## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Last element: %d\n", arr[n - 1]);

    return 0;
}
```
## OUTPUT
![alt text](<output 3.png>)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, count = 0;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for(int i = 0; i < n; i++) {
        if(arr[i] > 0) {
            count++;
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```
## OUTPUT
![alt text](<output 4.png>)

## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.



# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    char result[n];

    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for(int i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            result[i] = 'E';
        } else {
            result[i] = arr[i]; 
        }
    }

    printf("Modified array:\n");
    for(int i = 0; i < n; i++) {
        if(result[i] == 'E') {
            printf("%c ", result[i]);
        } else {
            printf("%d ", result[i]);
        }
    }

    return 0;
}
```
## Output:
 
![alt text](<output 5.png>)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



