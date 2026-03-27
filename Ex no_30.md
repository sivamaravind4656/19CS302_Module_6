# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.
## DATE:
## AIM:
To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm
   
1. Start.
2. Declare array size
3. Initialize array elements using malloc()
4. Update array size using realloc()
5. Print the result.
6. End.
   
## Program:
```
/*
C program to add two integer elements in an array using realloc() and that array already has three elements.

Developed by: ARAVINDHAN K A P
RegisterNumber: 212222063001
*/
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int *arr, i;

    arr = (int*)malloc(3 * sizeof(int));

    printf("Enter 3 integers:\n");
    for(i = 0; i < 3; i++)
    {
        scanf("%d", &arr[i]);
    }

    arr = (int*)realloc(arr, 4 * sizeof(int));

    printf("Enter the 4th integer:\n");
    scanf("%d", &arr[3]);

    int sum = 0;
    for(i = 0; i < 4; i++)
    {
        sum += arr[i];
    }

    printf("The sum of the array elements is: %d\n", sum);

    free(arr);

    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/2f889270-9e5d-469a-91e8-8c9ba4e4f3ba)



## Result:
Thus the program was executed and the output was verified successfully.
