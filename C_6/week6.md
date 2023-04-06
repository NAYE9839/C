# 6주차 코드



```

#include <stdio.h>

int main()
{
    int n,sum=0, i=1;
    printf("정수를 입력하시오: ");
    scanf("%d", &n);

    while(i<=n)
    {
        sum+=i;
        i++;
    }

    printf("1부터 %d까지의 합은 %d입니다", n, sum);
}
   
```







