#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <ctype.h>

int main() {
    char input[100], op, t[3];
    int i, j, len, k = 1;
    
    printf("Enter an arithmetic expression: ");
    scanf("%s", input);
    
    len = strlen(input);
    
    printf("Three address code representation:\n");
    
    for (i = 0; i < len; i++) {
        if (isdigit(input[i])) {
            // If the current character is a digit, print the corresponding TAC code
            printf("t%d = %c\n", k, input[i]);
            t[0] = 't';
            t[1] = k + '0';
            t[2] = '\0';
            k++;
        } else if (input[i] == '+' || input[i] == '-' || input[i] == '*' || input[i] == '/') {
            // If the current character is an operator, print the corresponding TAC code
            op = input[i];
            printf("%c %c %c %c\n", t[0], t[1], op, input[i+1]);
        }
    }
    
    return 0;
}
