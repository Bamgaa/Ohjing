#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>   //헤더 파일을 포함시키는 전처리기

int main()   //함수를 정의하는 문장
{
    int score[5];   //7개의 변수를 지정
    int sum=0;
    double ave=1;

    for (int i=0; i<5; i++)   //변수 i를 0으로 지정하고 5보다 낮으면 1씩 더하면서 반복시키는 문장
    {
    printf("%d번째 학생 점수 입력: ",i+1);   //변수에 1을 더한 후 출력
    scanf("%d",&score[i]);   //입력하는 문장
    if (score[i]<0 || score[i]>100)   //변수가 0보다 작거나 100보다 크면 그래도 출력하고 아니면 else로 넘어가는 조건문
    {
       printf("잘못 입력한듯 다시 ㄱㄱ\n");
       i--;  //마지막에 i의 값을 감소
    }
    else
    {
        sum += score[i];   //5명의 값을 계속 더하는 문장
    }
}

ave=sum/5;   //sum을 5로 나눈값을 ave에 대입

printf("5명의 평균은 %.2f",ave);

return 0;

}
