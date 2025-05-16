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
void calculateEMI(float principal, float annualRate, float years) {
    float monthlyRate = annualRate / (12 * 100); 
    int months = (int)(years * 12);             

    float emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) /
                (pow(1 + monthlyRate, months) - 1);

    printf("Monthly EMI is= %.3f\n", emi);
}

int main()
{
    float principal = 775000;
    float annualRate = 8.75;
    float years = 10.6;
    calculateEMI(principal, annualRate, years);
    return 0;
}

```

## OUTPUT

![image](https://github.com/user-attachments/assets/adb7480c-5b1c-4978-975a-5369e9420c7d)




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
    int n = 6;  // Number of terms
    int first = 0, second = 1, next;

    printf("Fibonacci series for %d terms:\n", n);

    for (int i = 1; i <= n; i++) {
        printf("%d ", first);
        next = first + second;
        first = second;
        second = next;
    }

    printf("\n");

    return 0;  // Indicate successful execution
}


```

## OUTPUT

![image](https://github.com/user-attachments/assets/c8f1a287-fcc8-49b4-b6d8-ed470a2c8b86)







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

int main()
{
    int n, i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i < n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;i++) 
    {
        printf("%d ",a[i]);
    }

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/40758c23-9f4b-490e-a14b-f98569302421)









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
#include<stdio.h>
int main()
{
    int n,p=0;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++){
        scanf("%d",&a[i]);
        if(a[i]>0)
            p++;
    }
    printf("count  of positive numbers  in array: %d",p);
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/2fd5fa75-fe05-4e0e-9896-1e14293e1349)




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
    int arr[100], n;
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E'; 
        }
    }
    printf("Updated array:\n");
    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    return 0;
}

```
## Output:
 ![image](https://github.com/user-attachments/assets/1aba585f-01bf-4eeb-8946-39bf04aa614c)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



