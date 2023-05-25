

```
#include <stdio.h>

int main() {
  int x = 20, y = 20;
  int *p;

  p = &x;
  printf("p=%p\n", p);
  printf("*p=%u\n\n", *p);

  p = &y;
  printf("p=%p\n", p);
  printf("p=%u\n", *p);

  return 0;
}
```


