# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>


void calculateEMI(float principal, float rate, int time) {
    float emi;
    float monthlyRate = rate / (12 * 100); 
    int months = time * 12;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);

    printf("\nThe EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int time;

    
    scanf("%f", &principal);

   
    scanf("%f", &rate);

    
    scanf("%d", &time);

 
    calculateEMI(principal, rate, time);

    return 0;
}
```

## OUTPUT


![437750122-decc10cb-261c-4e95-9c8b-767a53acd002](https://github.com/user-attachments/assets/0b2702c3-897c-4089-ae27-8bef858a9251)



## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


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
    int n = 6; // Number of terms
    int first = 0, second = 1, next, i;

    printf("Fibonacci Series up to %d terms:\n", n);

    for (i = 0; i < n; i++) {
        if (i <= 1)
            next = i;
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }

    return 0;
}
```

## OUTPUT


![437750157-371ee0a5-0b36-471f-8f73-95b03e54f54c](https://github.com/user-attachments/assets/8d3385ed-f9bb-4c7d-b119-21d6a5b6647d)






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
    int n, i;
;
    scanf("%d", &n);

    int arr[n]; 

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }


    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
```
## OUTPUT




![437750225-c195c5a9-a824-4463-b5be-7f8e552f26f8](https://github.com/user-attachments/assets/12d0a2b6-1f00-473a-a2c4-96c5a6f6374b)





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
    int n, i, count = 0;


    scanf("%d", &n);

    int arr[n]; 

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        if (arr[i] > 0) {
            count++; 
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```


## OUTPUT


![437750245-8e326c57-dd42-4e62-93b5-3ad8ee278b99](https://github.com/user-attachments/assets/745824f2-1d6e-4d92-af12-6a356e9a8e4a)



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
    int n, i;

    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Array after replacing even elements with 'E':\n");
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    return 0;
}
```
## Output:
 
![437751071-ec5273f5-81e1-40d0-820d-23fdfe7f3ae4](https://github.com/user-attachments/assets/5a4b5e97-97c3-416f-b87f-1da0d048557e)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



