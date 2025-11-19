# leap-year
#include<stdio.h>
int main() {
    int year, month, feb_days;

    printf("Enter a year: ");
    scanf("%d", &year);
    printf("Enter month number (1-12): ");
    scanf("%d", &month);

    if (month == 12) {
        while (1) {
            printf("Infinite Loop Running... December detected!\n");
        }
    } else {
        
        if ((year % 400 == 0) || (year % 4 == 0 && year % 100 != 0))
            feb_days = 29;
        else
            feb_days = 28;
        printf("\nDays in first 6 months: ");
        printf("January=31  February=%d  March=31  April=30  May=31  June=30", feb_days);
       
        if (feb_days == 29)
            printf("Leap Year");
        else
            printf("Not a Leap Year");

          if (month == 10) {
            printf("\nDiwali Vacation Holidays: ");
            printf("holidays date 18 19 20 21 22 23 24 25 26");
        }
    }

    return 0;
}

