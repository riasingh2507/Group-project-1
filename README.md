Menu driven program using switch case statement in C to check whether a number is: 
(i) Even number or Odd number, 
(ii) Two digit positive number or not,
(iii) Multiple of 5 or not.

//Ishu: Implements the main loop and menu display.
//Ria: Checking whether given number is even or odd using switch case.
//Spandan: Checking whether given number is a two-digit positive number or not using switch case.
//Rohit: Checking whether given number is a multiple of 5 or not using switch case.  
//Ayush: Exiting the program and printing the default statement.

````
#include <stdio.h>

int main() {
    int choice, num;

    printf("Menu:\n");
    printf("1. Check if a number is even or odd\n");
    printf("2. Check if a number is a two-digit positive number\n");
    printf("3. Check if a number is a multiple of 5\n");
    printf("4. Exit\n");

    printf("Enter your choice (1-4): ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:
            printf("Enter a number: ");
            scanf("%d", &num);
            if (num % 2 == 0) {
                printf("%d is an even number.\n", num);
            } else {
                printf("%d is an odd number.\n", num);
            }
            break;

        case 2:
            printf("Enter a number: ");
            scanf("%d", &num);
            if (num >= 10 && num <= 99) {
                printf("%d is a two-digit positive number.\n", num);
            } else {
                printf("%d is not a two-digit positive number.\n", num);
            }
            break;

        case 3:
            printf("Enter a number: ");
            scanf("%d", &num);
            if (num % 5 == 0) {
                printf("%d is a multiple of 5.\n", num);
            } else {
                printf("%d is not a multiple of 5.\n", num);
            }
            break;

        case 4:
            printf("Exiting the program.\n");
            break;

        default:
            printf("Invalid choice. Please select a number between 1 and 4.\n");
            break;
    }

    return 0;
}
````
