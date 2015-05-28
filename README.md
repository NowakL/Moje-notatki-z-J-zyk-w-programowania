## Notatki Jezyki programowania

# Zadania na Petle

1. Wypisz liczby calkowite od 0 do 23 za pomoca petli for, while i do-while.


'
	
	#include<stdio.h>
	main() {
	int i;
	i=0;

 	do {
	 printf("%d ", i);
	 i++;
				}

	while(i<=23);
	printf("\n");				

	i=0;

 	while(i<=23){
	
	printf("%d ", i);
	i++;
	}	
	printf("\n");
		
	for(i=0; i<=23; i++)
	printf("%d ", i);
	printf("\n");
	
	return 0;}
'

2. Wypisz liczbyod -3.5 do 7.5 z krokiem co 0.5 za pomoca petli for i while.

'

#include <stdio.h>

main(){
double i, step;
	
step=0.5;

		for(i=-3.5;i<=7.5;i++)
		{
		printf("%.1lf \n", i);
		i=i-step;
		
		}
		printf("\n");
		
		
	i=-3.5;
	step=0.5;
	
		while(i<=7.5){
		printf("%.1lf \n", i);
		i=i+step;
		}
	
	return 0;
	
}
'

