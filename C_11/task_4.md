

```
#include <math.h> //수학적 함수 ex)sin,cos 를 쓰기위한 헤더파일
#include <stdio.h>

int main()
{ 
    double pi=3.1415926535; //원주율 값 저장
    double x,y;
    x = pi/2; //대입함수로 pi/2을 x에 대입
    y = sin(x); //사인 x값 y에 대입
    printf("sin(%f)=%f\n", x, y); //위의 x와 y값을 sin(%f)=%f 식에 대입, %f이기에 소수점 6자리까지만 출력
    y = cos(x); //코사인 x값 y에 대입
    printf("cos(%f)=%f\n", x, y); //위의 x와 y값을 cos(%f)=%f 식에 대입, %f이기에 소수점 6자리까지만 출력
    return 0;
} 
```


