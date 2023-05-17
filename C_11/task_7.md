

```
#define _CRT_SECURE_NO_WARNINGS
#include <math.h>
#include <stdio.h>

int main()
{
    double height, distance, tree_height, degrees, radians;
    printf("나무와의 길이(단위는 미터):"); //문장 출력하고
    scanf("%lf", &distance); //사용자에게 나무와의 거리 입력받기, 입력받은건 distance에 저장
    printf("측정자의 키(단위는 미터):"); //문장 출력하고
    scanf("%lf", &height); //사용자에게 측정자의 키 입력받기, 입력받은건 height에 저장
    printf("각도(단위는 도):"); //문장 출력하고
    scanf("%lf", &degrees); //사용자에게 각도 입력받기, 입력받은건 degrees에 저장
    radians=degrees*(3.141592/180.0); //입력받은 각도를 대입해서 계산후 radians에 대입
    tree_height=tan(radians)*distance+height; //위의 값을 이용해 계산후, tree_height에 대입
    printf("나무의 높이(단위는 미터): %lf\n", tree_height); //위의 tree_height 값을 %lf에 대입 후 문장 출력
    return 0;
}
```

