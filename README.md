# DiceGame
# DiceGame
#include<stdlib.h>
#include<time.h>

int GetRandom(int min,int max);

int main(){

int d1,d2;
srand((unsigned int)time(NULL));
d1=GetRandom(1,6);
d2=GetRandom(1,6);
printf("Rolling the dice...\n");
printf("Die 1: %d\n",d1);
printf("Die 2: %d\n",d2);
printf("Total value: %d\n",d1+d2);
return 0;
}

int GetRandom(int min,int max){

return min+(int)(rand()*(max-min+1.0)/(1.0+RAND_MAX));
}
