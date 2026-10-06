#include <stdio.h>

int main()
{
    char grammar[10][20];
    int n, i;

    printf("Enter number of productions: ");
    scanf("%d", &n);

    printf("Enter productions:\n");
    for(i = 0; i < n; i++)
        scanf("%s", grammar[i]);

    printf("\nFIRST sets:\n");

    for(i = 0; i < n; i++)
    {
        printf("FIRST(%c) = { %c }\n",
               grammar[i][0], grammar[i][3]);
    }

    return 0;
}
OUTPUT:
<img width="1683" height="922" alt="Screenshot 2026-10-06 102447" src="https://github.com/user-attachments/assets/d037a8b9-3f0e-49a3-bfdb-30e2655a18ef" />
