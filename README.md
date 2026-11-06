# C-in-work-
Tasks on C
/* Вводится номер дня, выдать название,
или "error" в случае неверного ввода */
/* Марнат */
/* Задания.
1. По номеру месяца - количество дней
2. По номеру месяца - время года */
#include <stdio.h>
/*Задание 1*/
int main() {
    int month;
    scanf("%d",&month);

    printf("Задание 1\n");
    switch (month) {
    case 1: case 3: case 5:    case 7: case 8: case 10: case 12:
        printf("31\n");
        break;
    case 2:
        printf("28 or 29\n");
        break;

    case 4:    case 6: case 9: case 11:
        printf("30\n");
        break;


    default:
        printf("Error\n");
        break;
    }
    return 0;
}
