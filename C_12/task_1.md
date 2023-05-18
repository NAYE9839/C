


```
구구단
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int main() {
  int s, e;

  while (1) {
    scanf("%d %d", &s, &e);
    if ((2 < s || 9 > s) || (2 < e || 9 > e)) {
      printf("INPUT ERROR!\n");
      break;
    }
  }
  if (s < e) {
    for (int i = 1; i <= 9; i++) {
      for (int j = s; j <= e; j++) {
        printf("%d * %d = %2d", j, i, i * j);
      }
      printf("\n");
    }
  } else {
    for (int i = 1; i <= 9; i++) {
      for (int j = s; j >= e; j--) {
        printf("%d * %d = %2d", j, i, i * j);
      }
      printf("\n");
    }
  }
  ```
  
  
