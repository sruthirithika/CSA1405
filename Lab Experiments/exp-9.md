#include <stdio.h>

int main()
{
    char nt, alpha, beta;

    printf("Enter grammar:\n");
    printf("S -> (L) | a\n");
    printf("L -> L,S | S\n\n");

    nt = 'L';
    alpha = ',';
    beta = 'S';

    printf("Left recursive production: L -> L,S | S\n");

    printf("\nGrammar without left recursion:\n");
    printf("L -> SL'\n");
    printf("L' -> ,L' | E\n");

    return 0;
}
OUTPUT:
<img width="1805" height="910" alt="Screenshot 2026-10-06 103145" src="https://github.com/user-attachments/assets/44b13866-46de-466c-aa65-9282297c32e0" />
