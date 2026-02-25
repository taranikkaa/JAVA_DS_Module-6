# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE: 25-02-2026
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
1. Start
2. Read number of rows and columns
3. Input elements of Matrix A
4. Input elements of Matrix B
5. Add corresponding elements of Matrix A and Matrix B
6. Store result in Matrix C
7. Check whether each element of Matrix C is even or odd
8. If all elements are odd, print "Resultant matrix is Odd"
9. Else if all elements are even, print "Resultant matrix is Even"
10. Otherwise print "Resultant matrix is Mixed"
11. Stop   

## Program:
``` java
/*
Program to find the nature of resultant matrix.

Developed by:TARANIKKA A
Register Number: 212223220115
Date: 25-02-2026
*/

import java.util.Scanner;

public class MatrixNature {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of rows: ");
        int r = sc.nextInt();

        System.out.print("Enter number of columns: ");
        int c = sc.nextInt();

        int A[][] = new int[r][c];
        int B[][] = new int[r][c];
        int C[][] = new int[r][c];

        System.out.println("Enter elements of Matrix A:");
        for(int i = 0; i < r; i++) {
            for(int j = 0; j < c; j++) {
                A[i][j] = sc.nextInt();
            }
        }

        System.out.println("Enter elements of Matrix B:");
        for(int i = 0; i < r; i++) {
            for(int j = 0; j < c; j++) {
                B[i][j] = sc.nextInt();
            }
        }

        boolean allEven = true;
        boolean allOdd = true;

        // Matrix Addition
        for(int i = 0; i < r; i++) {
            for(int j = 0; j < c; j++) {
                C[i][j] = A[i][j] + B[i][j];

                if(C[i][j] % 2 == 0)
                    allOdd = false;
                else
                    allEven = false;
            }
        }

        if(allOdd)
            System.out.println("Resultant matrix is Odd");
        else if(allEven)
            System.out.println("Resultant matrix is Even");
        else
            System.out.println("Resultant matrix is Mixed");

        sc.close();
    }
}

```

## Output:

<img width="405" height="404" alt="Screenshot 2026-02-19 222934" src="https://github.com/user-attachments/assets/b0386c8a-ecde-4beb-b682-4d6ae98c4a0c" />


## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
