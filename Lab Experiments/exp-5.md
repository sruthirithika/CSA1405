#include <stdio.h>

int main()
{
    char str[200];
    int spaces = 0, newlines = 0, i;

    printf("Enter text (use ~ to end):\n");
    scanf("%[^~]", str);

    for(i = 0; str[i] != '\0'; i++)
    {
        if(str[i] == ' ' || str[i] == '\t')
            spaces++;

        if(str[i] == '\n')
            newlines++;
    }

    printf("Total number of white spaces: %d\n", spaces);
    printf("Total number of newline characters: %d\n", newlines);

    return 0;
}
OUTPUT:
<img width="1881" height="930" alt="Screenshot 2026-10-05 191435" src="https://github.com/user-attachments/assets/b9ebcb28-e327-47bb-85c8-05972f098b6c" />
