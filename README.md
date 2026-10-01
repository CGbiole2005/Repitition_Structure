#include <stdio.h>

int main() {
    int i, j, k;

    // === Challenge 1.1: Single Row ===
    printf("--- Challenge 1.1 - Single Row ---\n");
    i = 0;
    while (i < 8) {
        printf("*");
        i++;
    }
    printf("\n\n");


    // === Challenge 1.2: Vertical Column ===
    printf("--- Challenge 1.2 - Vertical Column ---\n");
    i = 0;
    while (i < 5) {
        printf("*\n");
        i++;
    }
    printf("\n");


    // === Challenge 2.1: Square ===
    printf("--- Challenge 2.1 - Square ---\n");
    i = 0;
    while (i < 4) {
        j = 0;
        while (j < 4) {
            printf("*");
            j++;
        }
        printf("\n");
        i++;
    }
    printf("\n");


    // === Challenge 2.2: Rectangle ===
    printf("--- Challenge 2.2 - Rectangle ---\n");
    i = 0;
    while (i < 3) {
        j = 0;
        while (j < 6) {
            printf("*");
            j++;
        }
        printf("\n");
        i++;
    }
    printf("\n");


    // === Challenge 3.1: Right Triangle ===
    printf("--- Challenge 3.1 - Right Triangle ---\n");
    i = 1;
    while (i <= 5) {
        j = 1;
        while (j <= i) {
            printf("*");
            j++;
        }
        printf("\n");
        i++;
    }
    printf("\n");


    // === Challenge 3.2: Inverted Triangle ===
    printf("--- Challenge 3.2 - Inverted Triangle ---\n");
    i = 5;
    while (i >= 1) {
        j = 1;
        while (j <= i) {
            printf("*");
            j++;
        }
        printf("\n");
        i--;
    }
    printf("\n");


    // === Challenge 3.3: Diamond ===
    printf("--- Challenge 3.3 - Diamond ---\n");
    int n = 3; // Top half row count

    // Top half of diamond
    i = 1;
    while (i <= n) {
        // Spaces
        j = 1;
        while (j <= n - i) {
            printf(" ");
            j++;
        }
        // Stars
        k = 1;
        while (k <= (2 * i - 1)) {
            printf("*");
            k++;
        }
        printf("\n");
        i++;
    }

    // Bottom half of diamond
    i = n - 1;
    while (i >= 1) {
        // Spaces
        j = 1;
        while (j <= n - i) {
            printf(" ");
            j++;
        }
        // Stars
        k = 1;
        while (k <= (2 * i - 1)) {
            printf("*");
            k++;
        }
        printf("\n");
        i--;
    }

    return 0;
}
