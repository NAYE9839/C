

```
#include <stdio.h>
#include <math.h>

int menu() //밑에 있는 메뉴들 출력, 선택된 번호 반환
{
    int n;
    printf("1.팩토리얼\n");
    printf("2.싸인\n");
    printf("3.로그(base 10)\n");
    printf("4.제곱근\n");
    printf("5.순열(nPr)\n");
    printf("6.조합(nCr)\n");
    printf("7.종료\n");
    printf("선택해주세요:");
    scanf("%d", &n);
    return n;
}
void factorial() //팩토리얼 계산
{
    long long n, result=1, i;
    printf("정수를 입력하시오:"); //문장 출력 후
    scanf("%lld", &n); //사용자한테 정수n 받고
    for (i = 1; i <= n; i++) // 1부터 n까지 증가하며 반복
    result = result * i; //계산 후
    printf("결과=%lld\n\n", result); // result값 %lld에 longlong형식으로 대입
}
void sine() //싸인 계산
{
    double a, result;
    printf("각도를 입력하시오:"); //문장 출력 후
    scanf("%lf", &a); //사용자한테 정수a 받고
    result = sin(a); //a의sin값을 계산 후 result에 대입
    printf("결과=%lf\n\n", result); //result값 %lf에 double형식으로 대입
}
void logBase10() //로그 계산
{
    double a, result;
    printf("실수값을 입력하시오:"); //문장 출력 후
    scanf("%lf", &a); //사용자한테 정수a값 받고
    if (a<=0.0) // a가 0이하면
    printf("오류\n"); //오류 출력
    else //a가 0보다 크면
    {
        result = log10(a); //a 대입해서 계산 후 result에 대입
        printf("결과=%lf\n\n", result); //result값 %lf에 double형식으로 대입
    }
    return 0;
}
int main()
{
    while (1) //무한반복
    {
        switch (menu()) //메뉴에서
        {
            case 1: //1을 입력하면
            factorial(); //팩토리얼 계산으로
            break; //탈출
            case 2: //2을 입력하면
            sine(); //싸인 계산으로
            break; //탈출
            case 3: //3을 입력하면
            logBase10(); //로그 계산으로
            break; //탈출
            case 7: //7을 입력하면
            printf("종료합니다.\n"); //이 문장 출력하고
            return 0; //종료
            default: //일치하는 값 없으면
            printf("잘못된 선택입니다.\n"); //이 문장 출력하고
            break; //탈출
        }
    }
}
```


