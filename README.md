# EXERCICIO-DO-WHILE

    
    #include <stdio.h>
    #include <stdlib.h>
    #include <time.h>


    int main(){
        system ("clear");
        srand((unsigned)time(NULL));
        int numeroSorteado = rand() % 11;
        int num;
        
        do{
            printf("\nAdvinhe o número aleatório! \n");
            printf("Número: ");
            scanf("%d", &num);
        
            if(numeroSorteado > num){
                printf("Número sorteado é maior! \n");
            }
            else if(numeroSorteado < num){
                printf("Número sorteado é menor! \n");
            }
        }while(numeroSorteado != num);
        
        printf("Você acertou o número %d");
        
        
    
        return 0;
    }
