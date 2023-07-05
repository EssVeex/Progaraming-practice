#include <stdio.h>

int countNumbers(int r) {
    if (r <= 0) {
        return 0;
    }

    if (r == 1) {
        return 2; // 5 та 9
    }

    int count = 0;
    int prevCount = 1; // Кількість чисел для розряду 1

    for (int i = 2; i <= r; i++) {
        count = prevCount * 2; // Помножити на 2, оскільки є по дві можливості (5 або 9) для кожного розряду
        prevCount = count;
    }

    return count;
}

int main() {
    int r;
    printf("Введіть кількість розрядів (р): ");
    scanf("%d", &r);

    int result = countNumbers(r);
    printf("Кількість чисел із %d розрядів: %d\n", r, result);

    return 0;
}
