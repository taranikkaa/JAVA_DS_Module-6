# Ex2 Count how many times a number appears in an array recursively.
## DATE:25.02.2026

## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1. Start the program and read the array elements.

2. Read the number whose occurrences must be counted.

3. Define a recursive function countOccurrences(arr, n, target) to count matches in the first n elements.

4. If n == 0, return 0; otherwise check if the last element equals the target and add it to the recursive result.

5. Call the recursive function with full array length and print the total count.

## Program:
```
/*
Program Count how many times a number appears in an array recursively.
Developed by: TARANIKKA A
RegisterNumber:  212223220115
*/

import java.util.*;

public class CountOccurrencesRecursive {

    // Recursive method to count occurrences
    static int countOccurrences(int[] arr, int n, int target) {
        if (n == 0)
            return 0;

        int count = (arr[n - 1] == target) ? 1 : 0;
        return count + countOccurrences(arr, n - 1, target);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int[] arr = new int[n];
        System.out.println("Enter the elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        System.out.print("Enter the number to count: ");
        int target = sc.nextInt();

        int result = countOccurrences(arr, n, target);
        System.out.println("The number " + target + " appears " + result + " times.");
    }
}


```

## Output:

<img width="1919" height="615" alt="Screenshot 2025-11-15 101236" src="https://github.com/user-attachments/assets/6d623ccd-cc3f-42a4-a0e6-8bbd846e1e0e" />


## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
