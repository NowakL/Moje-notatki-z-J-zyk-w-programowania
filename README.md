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


' 3. Wypisz kwadraty i szesciany liczb naturalnych od 1 do liczby podanej przez uzytkownika za pomoca petli for, while i do-while.

'

	#include <stdio.h>

	main() {
	int i, n, k, s;
	
	printf("Podaj liczbe naturalna: ");
	scanf("%d", &n);

	// pętla for
	for(i=1;i<=n;i++){
		k=i*i;
		s=i*i*i;
		printf("%d %d %d \n", i, k, s);
	
	}
	printf("\n");
	// pętla while
	i=1;
	 while(i<=n){
	 k=i*i;
		s=i*i*i;
		printf("%d %d %d \n", i, k, s);
		i++;
	 }
	 printf("\n");
	 //pętla do while
	 
	i=1;
		do{
		k=i*i;
		s=i*i*i;
		printf("%d %d %d \n", i, k, s);
		i++;
		}
		while(i<=n);
		
		
	return 0;
}

'4. Oblicz za pomoca petli for i while sume kwadratow liczb od 3 do 15.

'

	#include <stdio.h>


	main(){
	
	int i, n, k;
	n=0;
	
	for(i=3;i<=15;i++){
		k=i*i;
		n=n+k;
	
	}	
	printf("%d \n", n);
	
	printf("\n");
	printf("\n");
	
	i=3;
	n=0;
	while(i<=15){
		k=i*i;
		n=n+k;
		i++;
	}
	printf("%d \n", n);
	return 0;
}

'

# Zadania Warunkowe

 1. Napisz program liczacy pierwiastki trojmianu kwadratowego: a*x^2+b*x+c=0

'

	#include <stdio.h>
	#include <math.h>

	main(){

	double a ,b , c, x1, x2, x, delta;
	x1, x2 =0;
	
	puts("Podaj trzy liczby rozne od 0: ");
	scanf("%lf %lf %lf", &a , &b, &c); 
	delta=0;
	delta==b*b-4*a*c;
	
	printf("Delta jest rowna %lf\n", delta);
	
	if(delta>0){
		x1=(-b - sqrt(delta))/(2*a);
		x2=(-b + sqrt(delta))/(2*a);
		printf("zmienna x1 jest rowna %lf , a zmienna x2 jest rowna %lf.\n", x1 ,x2);
	}
	else if(delta==0){
		x=(-b)/(2*a);
		printf("X jest rowny %lf", x);
	}
			else printf("Brak rozwiazan.\n");
			}

'

 2. Znajdz liczby o tej wlasnosci, ze suma dzielnikow wlasciwych liczby jest rowna zadanej liczbie, np. 6=1+2+3. Sa to tak zwane liczby doskonale.

'

	# include <stdio.h>

	main(){
	int i, liczba, suma;
	puts("Podaj liczbe: \n");
	scanf("%d",&liczba);
	suma=0;
	
		for(i=2;i<10000;i++){
			
			for(liczba=1;liczba<i;liczba++)
			suma==i%liczba;
			printf("%d", suma);
		}
		
}

'
