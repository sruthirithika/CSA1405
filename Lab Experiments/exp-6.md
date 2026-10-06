#include <stdio.h>
#include <ctype.h>

int main()
{
    char id[50];
    int i, valid = 1;

    printf("Enter an identifier: ");
    scanf("%s", id);

    if (!isalpha(id[0]) && id[0] != '_')
        valid = 0;

    for (i = 1; id[i] != '\0'; i++)
    {
        if (!isalnum(id[i]) && id[i] != '_')
        {
            valid = 0;
            break;
        }
    }

    if (valid)
        printf("Valid Identifier");
    else
        printf("Invalid Identifier");

    return 0;
}
OUTPUT:
<img width="1518" height="918" alt="Screenshot 2026-10-06 102127" src="https://github.com/user-attachments/assets/dcd5e643-e311-4b91-b8ea-136d431c816e" />
