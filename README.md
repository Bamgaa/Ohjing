#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h> //Preprocessor containing header files

statements defining int main() // functions
{
    specify int score[5]; //7 variables
    int sum=0;
    double ave=1;

    For (inti=0; i<5; i++) // a statement that specifies variable i as 0 and repeats by adding 1 if it is less than 5
    {
    printf ("%dth Student Score Input: ",i+1); // Add 1 to variable and output
    scanf ("%d", &score[i]); // type sentence
    If (score[i]<0 || score[i]>100) // If the variable is less than 0 or greater than 100, it will still output, or it will go to else.
    {
       printf("As if you typed it incorrectly, go back to ㄱ\n"");
       i--; // reduce the value of i at the end
    }
    else
    {
        sum += score[i]; // a sentence that continues to add values of 5 people
    }
}

Substituting ave=sum/5; //sum divided by 5 into ave

printf ("The average of five people is %).2f",ave);

return 0;

}
