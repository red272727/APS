# APS
CÓDIGO DA APS
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <locale.h>

int main(){
    setlocale(LC_ALL, "portuguese");

    system("color 09");
	srand(time(NULL));
	int sorteado, digitado, contador=0;
	int s=1;
	int n=0;
	sorteado = 1 + rand()%50;
	printf("      #        ######     ##   #         #   ##   ##     #   #    #   #####\n");
    printf("     # #       #     #          #       #         # #    #   #    #   #\n");
    printf("    #   #      #      #   ##     #     #     ##   #  #   #   #    #   #\n");
    printf("   #     #     #     #    ##      #   #      ##   #   #  #   ######   #####\n");
    printf("  #########    #    #     ##       # #       ##   #    # #   #    #   #\n");
    printf(" #         #   #####      ##        #        ##   #     ##   #    #   #####\n");
    printf("                                                                           \n");
    printf("                              # # # #\n");
    printf("                             #       #\n");
    printf("                             #       #\n");
    printf("                             #       #\n");
    printf("                             #       #\n");
    printf("                              # # # # \n");
    printf("                                                                           \n");
    printf("      ##     #     ##    ##   ##      ##   #####   #####      # # # #\n");
    printf("      # #    #     ##    ##   # #    # #   #       #    #    #       #\n");
    printf("      #  #   #     ##    ##   #  #  #  #   #       #   #     #       #\n");
    printf("      #   #  #     ##    ##   #   ##   #   #####   ####      #       #\n");
    printf("      #    # #     ##    ##   #        #   #       #   #     #       #\n");
    printf("      #     ##     ########   #        #   #####   #    #     # # # #\n");
	printf("O número sorteado está entre: 1 E 50\n");

	do{
		contador++;
		printf("Chute um número: \n");
		scanf("%d",&digitado);

		if(digitado == sorteado){
			printf("Boaa, só conquitar o mundo humano!!! \n");
			printf("Acertou em %d tentativas.\n", contador);
		}else if (sorteado < digitado){
			printf("Chute um número menor: \n");
		}else{
			printf("Tente um número maior: \n");
		}

	}
	while(sorteado != digitado);

	printf("\n                Créditos: \n");
    printf("Gustavo De Campos Araujo Caramelo RA: 21308545 \n");
    printf("Higor Mantas De Oliveira Lins     RA: 21245760 \n");
    printf("Isabella Fagundes Barao           RA: 21268610");
	return 0;
}
