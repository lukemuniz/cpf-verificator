# cpf-verificator
verificador de CPF por 2 etapas



#include<stdio.h>
#include<conio.h>
#include<locale.h>
#include <stdlib.h>
#include <windows.h>



main(){


int a,b,c,d,e, f,g,h,i,j,k, soma, resto;
float oper, oper2;

setlocale(LC_ALL,"");

printf("Digite os 9 primeiros dígitos do CPF para validação \n");

printf("\n \n");

	
	scanf("%i", &a);
	scanf("\n %i", &b);
	scanf("\n %i", &c);
	scanf("\n %i", &d);
	scanf("\n %i", &e);
	scanf("\n %i", &f);
	scanf("\n %i", &g);
	scanf("\n %i", &h);
	scanf("\n %i", &i);
printf("\n Obrigado, verificando. Aguarde por favor");
	
Sleep (1000);
system ("cls");
	
					
					oper = ((a*10) + (b*9) + (c*8) + (d*7) + (e*6) + (f*5) + (g*4) + (h*3) + (i*2)) % 11 ;
					
					if(oper<=1){
						j=0;
					}
					else{
						j=11-oper;
					}
					
					oper2 = ((a*11) + (b*10) + (c*9) + (d*8) + (e*7) + (f*6) + (g*5) + (h*4) + (i*3) + (j*2)) % 11 ;
					
					if(oper2<=1){
						k=0;
					}
					else{
						k=11-oper2;
					}
					
printf("\n \n O dígito verificador é = %i%i",j,k);
Sleep (1000);
printf("\n\n");
printf("\n Mais um instante");
Sleep (1000);

					
soma = ((a+b+c+d+e+f+g+h+i+j+k) % 11);
//printf("\n soma do cpf igual a : %i", soma);

if(soma<1){
	printf("\n O CPF é válido");
	
}

Sleep(1000);

printf("\n Pressione qualquer tecla para sair");
getch();

					




}



	
	
	

	


	
	



