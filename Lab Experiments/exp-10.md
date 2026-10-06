#include <stdio.h>

int main()
{
    printf("Given Grammar:\n");
    printf("S -> iEtS | iEtSeS | a\n");
    printf("E -> b\n");

    printf("\nGrammar after Left Factoring:\n");
    printf("S -> iEtSX | a\n");
    printf("X -> eS | E\n");

    return 0;
}
OUTPUT:
<img width="1760" height="602" alt="Screenshot 2026-10-06 103533" src="https://github.com/user-attachments/assets/6d641447-82dd-4d54-a7e0-a18e221b801b" />
