#include <stdio.h>
#include <ctype.h>
#include <string.h>

int main()
{
    char str[100], token[20];
    int i = 0, j;

    printf("Enter an expression: ");
    fgets(str, sizeof(str), stdin);

    while (str[i] != '\0')
    {
        if (isspace(str[i]))
        {
            i++;
        }
        else if (isalpha(str[i]) || str[i] == '_')
        {
            j = 0;
            while (isalnum(str[i]) || str[i] == '_')
                token[j++] = str[i++];
            token[j] = '\0';
            printf("Identifier: %s\n", token);
        }
        else if (isdigit(str[i]))
        {
            j = 0;
            while (isdigit(str[i]))
                token[j++] = str[i++];
            token[j] = '\0';
            printf("Constant: %s\n", token);
        }
        else if (strchr("+-*/=%", str[i]))
        {
            printf("Operator: %c\n", str[i]);
            i++;
        }
        else
            i++;
    }

    return 0;
}
OUTPUT:
<img width="1897" height="957" alt="Screenshot 2026-10-05 185018" src="https://github.com/user-attachments/assets/64fbd768-037d-4ce5-ae58-d27740be9223" />
