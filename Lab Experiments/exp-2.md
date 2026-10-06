#include <stdio.h>
#include <string.h>

int main()
{
    char str[100];

    printf("Enter a line: ");
    fgets(str, sizeof(str), stdin);

    if (str[0] == '/' && str[1] == '/')
        printf("It is a single-line comment.\n");
    else if (str[0] == '/' && str[1] == '*')
        printf("It is a multi-line comment.\n");
    else
        printf("It is not a comment.\n");

    return 0;
}
OUTPUT:
<img width="1878" height="925" alt="Screenshot 2026-10-05 185252" src="https://github.com/user-attachments/assets/993bcfdf-88fd-4b41-a5fd-a625059167a5" />
