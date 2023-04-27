

```
#include <stdio.h>

int main()

{
    int x;
    int y;
    int sum, diff, mul, div;

    x=20;
    y=10;

    sum= x+y;
    diff=x-y;
    mul=x*y;
    div=x/y;

    printf("두수의 합: %d\n", sum);
    printf("두수의 차: %d\n", diff);
    printf("두수의 곱: %d\n", mul);
    printf("두수의 몫: %d\n", div);

    return 0; 
}

```


```
#define _CRT_SECURE_NO_WARNINGS

#include <stdio.h>
int main()
{
    int x;
    int y;
    int sum;

    printf("첫번째 숫자를 입력하시오:");
    scanf("%d", &x);

    printf("두번째 숫자를 입력하시오:");
    scanf("%d", &y);

    sum=x+y;
    printf("두수의 합:%d\n", sum);
    
    return 0;
}

```


```

#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int main()
{
    float radius;
    float area;

    printf("반지름을 입력하시오: ");
    scanf("%f", &radius);

    area=3.14 * radius *radius;

    printf("원의 면적: %f\n", area);

    return 0;
}

```

```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int main()
{
    double rate;
    double usd;
    int krw;

    printf("환율을 입력하시오: ");
    scanf("%lf", &rate);

    printf("원하 금액을 입력하시오: ");
    scanf("%d", &krw);

    usd=krw/rate;

    printf("원하는 %d원은 %lf달러입니다.\n", krw, usd);

    return 0;
}
```


```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int main()
{
    double num1, num2, num3;
    double sum, avg;

    printf("3개의 실수를 입력하시오: ");
    scsanf("%lf %lf %lf, &num1, &num2, &num3");

    sum=num1+num2+num3;
    avg=sum/3.0;

    printf("합계=%.2lf\n", sum);
    printf("평균=%.2lf\n", avg);

    return 0;
    
}
```

#include <stdio.h>

int main()
{
    double w, h, area, perimeter;

    w=10.0;
    h=5.0;
    area=w*h;
    perimeter=2*(w+h);

    printf("사각형의 넓이: %lf\n", area);
    printf("사각형의 둘레: %lf\n", perimeter);
    return 0;
}

```

```
#include <stdio.h>

int main()
{
    int x;

    printf("변수x의 크기: %d\n", sizeof(x));

    printf("char형의 크기: %d\n", sizeof(char));
    printf("int형의 크기: %d\n", sizeof(int));
    printf("short형의 크기: %d\n", sizeof(short));
    printf("long형의 크기: %d\n", sizeof(long));
    printf("float형의 크기: %d\n", sizeof(float));
    printf("double형의 크기: %d\n", sizeof(double));
    
    return 0;
}

```


```

#include <stdio.h>

int main()
{
    int x= 10;
    int y= 010;
    int z= 0*10;

    printf("x=%d", x);
    printf("y=%d", y);
    printf("z=%d", z);

    return 0;
}

```

#include <stdio.h>
int main()
{
    float x= 1.234567890123456789;
    double y= 1.234567890123456789;

    printf("float의 크기=%d\n", sizeof(float));
    printf("double의 크기=%d\n", sizeof(double));

    printf("x=%30.25f\n", x);
    printf("y=%30.25f\n", y);
    return 0;

}

```

```

#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int main()
{
    int i=0;
    do
    {
        printf("1---새로만들기\n");
        printf("2---파일열기\n");
        printf("3---파일닫기\n");
        printf("하나를 선택하시오.\n");
        scanf("%d", &i);/* code */
    } while (i<1||i>3);
    
    printf("선택된 매뉴=%d\n", i);
    return 0;
    
}

```

```

#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

    int main()
    { 
        int i, n;

        scanf("%d", &n);

        printf("====================\n");
        printf("====================\n");
        for(i=1; i<=n; i++)
        printf("%5d %5d\n", i, i*i*i);
        return 0;

    }
    
    ```
    
    
    ```
    
    #define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

int max(int x, int y);
{
    (x > y)? return x : return y;
}
int main()
{
    int x,y,larger;

    printf("정수 2개를 입력하시오: ");
    scanf("%d %d", &x, &y);

    larger = max(x,y);

    printf("더 큰 값은 %입니다. \n", larger);
    return 0;
}

```

```

#include <stdio.h>
    
    int main()
    {
        int a=2, b=2, c=2, d=2;

        a&=1;
        b^=1;
        c>>=1;
        d|=1;

        printf("a=%d b=%d c=%d d=%d\n", a, b, c, d);
        return 0;
    }
    
    ```
