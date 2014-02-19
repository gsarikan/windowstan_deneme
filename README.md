windowstan_deneme
=================

//girilen sayinin faktoriyelini hesaplayan C kodu

#include <stdio.h>
#include <stdlib.h>

long faktoriyel(long N){
     if(N==0){
        return 1;
        } else {
           return N*faktoriyel(N-1);
           }
}

int main(int argc, char *argv[])
{
  
  long sayi;
  
  printf("faktoriyelini hesaplamak istediginiz sayiyi giriniz: \n");
  scanf("%ld",&sayi);
  
  printf("%ld!= %ld\n",sayi,faktoriyel(sayi));
  
  system("PAUSE");	
  return 0;
}


