

```
#include <stdio.h>
#include <time.h>

int main()
{
    time_t start, end; //time_t 는 unsigned long 
    start=time(NULL); //대입함수로 시작시간을 start에 대입하고
    printf("10초가 되면 아무 키나 누르세요\n"); //이 문장 출력
    while (1) //무한루프
    {
        if (getchar()) //사용자 키 입력받으면
        break; //탈출하고
    }
    printf("종료되었습니다.\n"); //이 문장 출력
    end=time(NULL); //키 입력 받을때의시간을 end에 대입
    printf("경과된 시간은 %ld 초입니다.\n", end-start); //시작시간부터 끝난시간의 시간차이를 계산 후, %ld에 long형식을 통해 대입
    return 0;
}
```

