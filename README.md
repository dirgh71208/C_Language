# C_Language
#include <stdio.h>

int main() {
    float w, h, bmi;

    // Get weight from user
    printf("Enter the weight in kg: ");
    scanf("%f", &w);

    // Get height from user
    printf("Enter height in meters: ");
    scanf("%f", &h);

    // Calculate BMI: weight / (height * height)
    bmi = w / (h * h);
    
    printf("Calculated BMI: %.2f\n", bmi);

    // Evaluate BMI category
    if (bmi < 18.5) {
        printf("Person is underweight\n");
    } 
    else if (bmi >= 18.5 && bmi < 25.0) {
        printf("Person is normal weight\n");
    } 
    else if (bmi >= 25.0 && bmi < 30.0) {
        printf("Person is overweight\n");
    } 
    else {
        printf("Person is obese\n");
    }

    return 0;
}
