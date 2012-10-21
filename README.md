first-coding
============

Program Description: Calculate how long Carbon-14 decay has been on-going (in years) with the given remaining amount of the radio active Carbon-14 material.

#include<math.h>
#include<stdio.h>

int main(void)
{
  float target;
  float Prem; //percentage of C-14 remaining
  float agsam; // age of sample
  float rd; //rate of decay


  printf("\nEnter the percentage of carbon-14 remaining: ");
  scanf("%f", &target);

  Prem = target / 100;
  rd = 0.00012097; 

  agsam = -(1 / rd) * log(Prem);
  printf("\nPercentage of C-14 remaining: %.2f", target);


  printf("\nThe age of the sample:       %.5f years\n", agsam);

  return(0);
}

