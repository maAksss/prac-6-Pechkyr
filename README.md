# Практична 6 
Виконав: Печкур Максим
# Опис
Тема: довжина вектора

Визначити довжину вектора за його координатами. 

Вхідні дані: чотири цілі числа х1, у1, х2, у2 - кордина ти початку та кінця вектора відповідно

Вихідні дані: одне число - довжина вектора з точністю до шести знаків після коми

# Код
```
#include <stdio.h>
#include <math.h>

int main() {
    int x1, y1, x2, y2;
    double length;

    printf("Введіть координати початку вектора (x1, y1): ");
    scanf("%d %d", &x1, &y1);

    printf("Введіть координати кінця вектора (x2, y2): ");
    scanf("%d %d", &x2, &y2);

    int dx = x2 - x1;
    int dy = y2 - y1;
    length = sqrt(dx * dx + dy * dy);

    printf("Довжина вектора: %.6f\n", length);

    return 0;
}
```
