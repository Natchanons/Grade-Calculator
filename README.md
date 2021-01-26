# Grade-Calculator

#include<stdio.h>
#define MAX_SIZE 100
int main()
{
    float subj[MAX_SIZE],sum=0,credit[MAX_SIZE],result=0,c=0;
    int i,length;

    printf("How many subject you want to calculate = ");
    scanf("%d",&length);
    
    for(i=0;i<length;i++)
    {
        printf("Subject [%d] = ",i);
        scanf("%f",&subj[i]);
        printf("How much credit for Subject [%d] = ",i);
        scanf("%f",&credit[i]);
        sum += subj[i]*credit[i]; 
        c += credit[i];
    }
    result = sum/c;
    printf("Your result is = %f",result);

    return 0;
}
