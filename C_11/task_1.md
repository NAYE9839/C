

```
#include <stdlib.h> //난수 함수를 불러오는 헤더파일
#include <stdio.h>
#include <time.h>

int coin_toss(); //23줄 int coin_toss() 함수 호출, 동전 던지기 함수 선언
int main()
{
    int toss; //던진 횟수
    int heads=0; //앞면 개수
    int tails=0; //뒷면 개수
    srand((unsigned)time(NULL)); 
    for (toss=0; toss<100; toss++) //100번까지 증가하며 반복
    { 
        if(coin_toss()==1) //던지기 함수가 1이면
        heads++; //앞면 증가
        else //아니면
        tails++; //뒷면 증가
    }
    printf("동전의 앞면: %d\n", heads); //앞면 개수 출력
    printf("동전의 뒷면: %d\n", tails); //뒷면 개수 출력
    return 0;
}
int coin_toss()
{
    int head=rand()%2; //0 아니면 1(랜덤)
    return head; //선택 값 반환
}
```

