

```
#include <stdio.h>
#include <math.h>
#define PI 3.141592 //#define 전처리기를 통해 상수값 3.141592를 문자 PI로 치환

double rad(double degree) //각도를 라디안으로 변환
{
    return PI*degree/180.0;
}
void drawbar(int height) //밑에 출력할 *을 막대그래프형태로
{
    for (int i=0; i<height; i++) //밑에서 계산되어 주어질 height 만큼 
    printf("*"); //*출력
    printf("\n");
}
int main()
{
    int degree, x, y;
    for (degree=10; degree<=170; degree+=20) //degree를 10부터 170까지 20씩 증가하는걸 반복
    {
        y = (int)(60*sin(rad((double)degree))+0.5); //sin(rad((double)degree)) 계산후 60 곱하고, 0.5 더해서 반올림해주고, y에 대입
        drawbar(y); //y값을 9줄 void drawbar(int height)에 전달
    }
    return 0;
}
```

