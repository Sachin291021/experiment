#include <stdio.h>

int main() {
    // Declare variables to store marks of five subjects
    float marks[5], sum = 0.0, average;
    
    // Prompt the user to enter marks
    printf("Enter marks obtained in five subjects:\n");

    // Loop to get marks for all subjects
    for(int i = 0; i < 5; i++) {
        printf("Enter marks for subject %d: ", i + 1);
        scanf("%f", &marks[i]);
        sum += marks[i];  // Add the entered mark to sum
    }

    // Calculate the average
    average = sum / 5;

    // Display the total and average
    printf("\nTotal marks obtained: %.2f\n", sum);
    printf("Average marks: %.2f\n", average);

    return 0;
}
