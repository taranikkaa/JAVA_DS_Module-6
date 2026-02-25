# EX3 Write a program to count the number of digits in an integer.
## DATE:25.02.2026
## AIM:
To write a program to count the number of digits in an integer

## Algorithm
1. Start
2. Read an integer number
3. Initialize count = 0
4. If number == 0, set count = 1
5. If number < 0, convert it to positive
6. While number != 0
7. Divide number by 10
8. Increase count by 1
9. Display count
10. Stop

## Program:
```
/*
Program to count the number of digits in an integer

Developed by: TARANIKKA A
Register Number: 212223220115
*/

import java.util.Scanner;

public class CountDigits {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int num, count = 0;

        System.out.print("Enter an integer: ");
        num = sc.nextInt();

        if (num == 0) {
            count = 1;
        } else {
            if (num < 0) {
                num = -num;  // Handle negative numbers
            }

            while (num != 0) {
                num = num / 10;
                count++;
            }
        }

        System.out.println("Number of digits = " + count);

        sc.close();
    }
}

```

## Output:

<img width="372" height="199" alt="Screenshot 2026-02-19 222406" src="https://github.com/user-attachments/assets/92945852-ec64-4481-ad4a-eebd7f78eb03" />


## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
