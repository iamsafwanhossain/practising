#include<stdio.h>
#include<stdlib.h>
#include<time.h>

int main(){

srand(time(0));

int randomNumber = (rand() % 100)+1;
int number_of_guesses = 0;
int guessess;



do
{
  printf("guess the number");
scanf("%d" ,&guessess);

if (guessess<randomNumber)
{
  printf("guess higher number ");
}else if(guessess>randomNumber){
printf("guess low number");
}

number_of_guesses++;
} while (guessess!= randomNumber);

printf("you guessed the number in %d process",number_of_guesses);
return 0;
}
