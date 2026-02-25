# Ex5 Count Inversions in an Array
## DATE: 25-02-2026
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm
1. Start
2. Read the number of elements (n)
3. Input the array elements
4. Initialize inversionCount = 0
5. For i from 0 to n-1
6. For j from i+1 to n-1
7. If arr[i] > arr[j], increase inversionCount by 1
8. Display inversionCount
9. Stop

## Program:
``` java 
/*
Program to Count the number of inversions in an array 
where inversion is defined as: arr[i] > arr[j] and i < j

Developed by: TARANIKKA A
Register Number: 212223220115

*/

import java.util.Scanner;

public class CountInversions {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int arr[] = new int[n];

        System.out.println("Enter array elements:");
        for(int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int inversionCount = 0;

        for(int i = 0; i < n; i++) {
            for(int j = i + 1; j < n; j++) {
                if(arr[i] > arr[j]) {
                    inversionCount++;
                }
            }
        }

        System.out.println("Number of inversions: " + inversionCount);

        sc.close();
    }
}
```

## Output:

<img width="473" height="296" alt="Screenshot 2026-02-19 223209" src="https://github.com/user-attachments/assets/e23b5df9-3195-4348-81ae-5f1532b4dfb7" />


## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
