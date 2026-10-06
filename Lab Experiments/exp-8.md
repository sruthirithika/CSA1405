#include <stdio.h>

int main()
{
    char ch;

    printf("Grammar:\n");
    printf("S -> AaAb | BbBa\n");
    printf("A -> ε\n");
    printf("B -> ε\n\n");

    printf("Enter production value to find FOLLOW: ");
    scanf(" %c", &ch);

    if (ch == 'S')
        printf("FOLLOW(S) = { $ }\n");

    else if (ch == 'A')
        printf("FOLLOW(A) = { a b }\n");

    else if (ch == 'B')
        printf("FOLLOW(B) = { b a }\n");

    else
        printf("Invalid Non-Terminal\n");

    return 0;
}
OUTPUT:
<img width="1667" height="790" alt="Screenshot 2026-10-06 102853" src="https://github.com/user-attachments/assets/194a3725-f5f4-41e1-a095-d087430d3d2e" />
