#include <stdio.h>

int main()
{
    char op;

    printf("Enter any operator: ");
    scanf("%c", &op);

    switch(op)
    {
        case '+':
            printf("Addition");
            break;

        case '-':
            printf("Subtraction");
            break;

        case '*':
            printf("Multiplication");
            break;

        case '/':
            printf("Division");
            break;

        default:
            printf("Not an operator");
    }

    return 0;
}
  OUTPUT:
  <img width="1888" height="928" alt="Screenshot 2026-10-05 190659" src="https://github.com/user-attachments/assets/f079650f-c45f-4fe8-9923-db31c8774f0f" />
