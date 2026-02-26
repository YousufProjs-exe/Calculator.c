

#Calculator.c source code :

//easy copy and paste 

#include <stdio.h>
int main() 
{ 
    int a, b, opt, res; 
	// declaring variables

    printf("Welcome To Switch Case Calculator\n"); 
	// Welcome command / Message
    printf("Enter first number: ");
    scanf("%d", &a); 
	// asking user for first number (first Input)
    printf("Enter second number: ");
    scanf("%d", &b); 
	// asking user for second number (Second Input)

    printf("Arithmetic Operations: \n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    printf("5. Modulus Division\n"); 
	// Setting options
	
    printf("Enter your choice: ");
    scanf("%d", &opt);

    switch(opt)
	{ 
        case 1:
            res = a + b;
            printf("Addition: %d\n", res);
            break;
            
        case 2:
            res = a - b;
            printf("Subtraction: %d\n", res);
            break;
            
        case 3:
            res = a * b;
            printf("Multiplication: %d\n", res);
            break;
            
        case 4:
            if(b != 0) {
                res = a / b;
                printf("Division: %d\n", res);
            } else {
                printf("Error: Division by zero!\n");
            }
            break;
            
        case 5:
            if(b != 0) {
                res = a % b;
                printf("Modulus Division: %d\n", res);
            } else {
                printf("Error: Division by zero!\n");
            }
            break;
            
        default:
            printf("Invalid Option Selected\n");
			// default Case for Invalid attempts
    }

    return 0;
}
