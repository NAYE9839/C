

```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int main() {
  int x;

  scanf("%d", &x);

  for (int i = 1; i <= x; i++) {
    for (int j = 1; j <= x - i; j++) {
      printf("");
    }
    for (int k = 1; k <= i; k++) {
      printf("*");
    }
    printf("\n");
  }
  return 0;
}

```

```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int get_integer()
{
    int value;
    printf("정수를 입력하시오: ");
    scanf("%d", &value);
    return value;
}

int add(int x, int y)
{
    return x+y;
}
int main()
{
    int x=get_integer();
    int y=get_integer();

    int sum=add(x,y);
    printf("두수의 합은 %d입니다. \n", sum);
    return 0;
}

```
