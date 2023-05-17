

```
#include <stdlib.h>
#include <stdio.h>
#include <unistd.h> //windows.h 헤더파일은 window운영체제에서만 동작하고 conio.h 헤더파일은 비표준 헤더파일이기에 unistd.h 헤더파일을 사용한다.
#include <time.h>

void disp_car(int car_number, int distance) //26,27줄 disp_car 차 번호, 거리 받고 출력
{
    int i;
    printf("CAR #%d:", car_number); //자동차 번호 출력
    for(i=0; i<distance/10; i++)
    {
        printf("*"); //주행거리에 따라 별 출력
    }
    printf("\n");
}

int main()
{ 
    int i;
    int car1_dist=0, car2_dist=0;
    srand((unsigned)time(NULL));
    for(i=0; i<6; i++) //주행시간 6까지 증가
    {
        car1_dist+=rand()%100; //0-99까지 제한
        car2_dist+=rand()%100; //0-99까지 제한
        disp_car(1, car1_dist); //1번 자동차 번호,거리 출력
        disp_car(2, car2_dist); //2번 자동차 번호,거리 출력
        getchar(); //사용자 키 입력을 대기, 주행시간 6만큼 6회 반복 가능, 실제로 주행시간으로 설정해둔 6만큼 출력후 탭키 5번을 치면 처음 출력값과 함께 총 6번까지 반복 실행된다._getch(); dms conio.h 헤더파일에 포함된 비표준 함수이기에 unistd.h 헤더파일에 속한 getchar()합수를 사용

    }
    return 0;
}
```

