

EXP NO:21 C PROGRAM TO CREATE A FUNCTION TO FIND THE GREATEST NUMBER
Aim:
To write a C program to create a function to find the greatest number

Algorithm:
1.	Include the necessary header #include <stdio.h>.
2.	Use a series of if and else if statements to compare the values and return the maximum among them.
3.	Declare variables n1, n2, n3, n4, and greater to store user input and the result.
4.	Use scanf to take four integers as input.
5.	Call the max_of_four function with the input integers and store the result in the greater variable
 
Program:

```c
#include <stdio.h>

// Function to find the greatest number
int greatest(int a, int b)
{
    if (a > b)
        return a;
    else
        return b;
}

int main()
{
    int num1, num2, result;

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);

    result = greatest(num1, num2);

    printf("Greatest number = %d", result);

    return 0;
}
```

Output:
```
Enter two numbers: 25 40
Greatest number = 40
```

Result:
Thus, the program  that create a function to find the greatest number is verified successfully.


 
EXP NO:22 C PROGRAM TO PRINT THE MAXIMUM VALUES FOR THE AND, OR AND  XOR COMPARISONS
Aim:
To write a C program to print the maximum values for the AND, OR and XOR comparisons

Algorithm:
1.	Define a function calculate_the_max that takes two integers n and k as parameters.
2.	Declare variables a, o, and x to store the maximum values for AND, OR, and XOR operations, respectively.
3.	Use nested loops to iterate through pairs of integers (i, j) from 1 to n.
4.	Within the loops, check conditions for AND, OR, and XOR operations and update the corresponding maximum values (a, o, x).
5.	Declare variables n and k to store user input.
6.	Use scanf to take two integers as input.
7.	Call the calculate_the_max function with input values.
 
Program:

```c
#include <stdio.h>

int main()
{
    int a, b;
    int and_val, or_val, xor_val, max;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    and_val = a & b;
    or_val = a | b;
    xor_val = a ^ b;

    printf("AND value = %d\n", and_val);
    printf("OR value = %d\n", or_val);
    printf("XOR value = %d\n", xor_val);

    max = and_val;

    if (or_val > max)
        max = or_val;

    if (xor_val > max)
        max = xor_val;

    printf("Maximum value = %d", max);

    return 0;
}
```

Output:
```
Enter two numbers: 5 3
AND value = 1
OR value = 7
XOR value = 6
Maximum value = 7
```
Result:
Thus, the program to print the maximum values for the AND, OR and XOR comparisons
is verified successfully.


 
EXP NO:23 C PROGRAM TO WRITE THE LOGIC FOR THE REQUESTS
Aim:
To write a C program to write the logic for the requests

Algorithm:
1.	Declare variables noshel and noque to store the number of shelves and the number of queries, respectively.
2.	Use scanf to take two integers as input for the number of shelves and queries.
3.	Declare a 2D array shelarr to represent shelves and books, and an array nobookarr to store the number of books on each shelf.
4.	Declare variables k and c to keep track of the book index and the total number of books.
5.	Use a for loop to iterate over the queries.
 
Program:

```c
#include <stdio.h>

int main()
{
    int request;

    printf("Enter your request number: ");
    scanf("%d", &request);

    if (request == 1)
    {
        printf("Request 1 is processed");
    }
    else if (request == 2)
    {
        printf("Request 2 is processed");
    }
    else if (request == 3)
    {
        printf("Request 3 is processed");
    }
    else
    {
        printf("Invalid request");
    }

    return 0;
}
```

Output:
```
Enter your request number: 2
Request 2 is processed
```


Result:
Thus, the program to write the logic for the requests is verified successfully.


 
EXP NO:24 C PROGRAM PRINT THE SUM OF THE INTEGERS IN THE ARRAY.
Aim:
To write a C program print the sum of the integers in the array.

Algorithm:
1.	Declare a variable n to store the number of integers.
2.	Use scanf to take an integer n as input.
3.	Declare an array a of size n to store the integers.
4.	Declare a variable sum and initialize it to zero.
5.	Use a for loop to iterate n times:
6.	Use scanf to input each integer and add it to the sum.
7.	Print the final sum using printf.



Program:

```c
#include <stdio.h>

int main()
{
    int arr[100], n, i, sum = 0;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter the array elements:\n");

    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
        sum = sum + arr[i];
    }

    printf("Sum of array elements = %d", sum);

    return 0;
}
```

Output:
```
Enter the number of elements: 5
Enter the array elements:
10
20
30
40
50
Sum of array elements = 150
```

 


Result:
Thus, the program prints the sum of the integers in the array is verified successfully.


 
EXP NO 25: C PROGRAM TO COUNT THE NUMBER OF WORDS IN A      SENTENCE



Aim:

To write a C program that counts the number of words in a given sentence.

Algorithm:

1.	Input the sentence: Take a sentence from the user.
2.	Initialize a counter variable: This will keep track of the number of words.
3.	Process each character of the sentence:
o	Iterate through the sentence, checking each character.
o	If a character is not a space, it may belong to a word. If it's the first non-space character after a space or at the start, increment the word count.
4.	Handle spaces and punctuation: Skip over spaces, punctuation marks, and consider each word as a sequence of characters separated by spaces.
5.	Display the result: After processing the sentence, output the total word count.



Program:

```c
#include <stdio.h>
#include <string.h>

int main()
{
    char sentence[100];
    int i, count = 1;

    printf("Enter a sentence: ");
    fgets(sentence, sizeof(sentence), stdin);

    for(i = 0; sentence[i] != '\0'; i++)
    {
        if(sentence[i] == ' ')
        {
            count++;
        }
    }

    printf("Number of words = %d", count);

    return 0;
}
```

Output:
```
Enter a sentence: C programming is easy
Number of words = 4
```



Result:

Thus, the program that counts the number of words in a given sentence is verified 
successfully.
