#include <stdio.h>

int main() {
    char operator;
    double num1, num2, result;

    printf("Enter an operator (+, -, *):\n");
    scanf(" %c", &operator); // Added a space before %c to consume any newline character
    printf("Enter first number:\n");
    scanf("%lf", &num1); // Corrected format specifier to %lf
    printf("Enter second number:\n");
    scanf("%lf", &num2); // Corrected format specifier to %lf

    switch (operator) {
        case '+':
            result = num1 + num2;
            printf("%.2f + %.2f = %.2f\n", num1, num2, result);
            break;
        case '-':
            result = num1 - num2;
            printf("%.2f - %.2f = %.2f\n", num1, num2, result);
            break;
        case '*':
            result = num1 * num2;
            printf("%.2f * %.2f = %.2f\n", num1, num2, result);
            break;
        default:
            printf("Invalid operator.\n");
    }

    return 0;
}
