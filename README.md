/*The temperature in Chennai exists somewhere between 280C to 330C in a particular
week. The temperature in Delhi is 80C lesser than in Chennai. Likewise, the
temperature in Haveri is 50C more than that of Chennai. Write a C program to find the
temperature of Gangtok for a particular week, which is the temperature difference
between Delhi and Haveri. Get the temperature of Chennai (0C) as input for the week
of 7 days and the temperature of Gangtok (0C) as output for the week of 7 days.
Implement the program using arrays and validate the rules.*/
#include<stdio.h>
int main(){
  int c,d,h,g;
  int arrc[7],arrd[7],arrh[7],arrg[7];
  for(int x=0;x<7;x++){
    scanf("%d",&c);
    arrc[x]=c;
    arrd[x]=c-80;
    arrh[x]=c+50;
    arrg[x]=arrd[x]-arrh[x];
  }
  for(int x=0;x<7;x++){
    printf("%d\n",arrg[x]);
  }
}
