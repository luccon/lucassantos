1.
#include <stdio.h>

int num = 0;

int main(){   

    printf("Entre com o número para ser convertido!\n");
    scanf("%d",&num);
    
    printf("%x\n",num);
    printf("%o\n",num);
    return 0;
}

2.
#include <stdio.h>

float num = 0;

int main(){   

    printf("Entre com o número real!\n");
    scanf("%f",&num);
    
    printf("O valor é:%.1f\n",num);
}

3.
#include <stdio.h>

int x = 0;

int main(){   
    printf("Entre com o valor de X:\n");
    scanf("%d",&x);
    
    printf("O valor triplo de x:%d\nSeu quadrado:%d\nSeu meio: %d\n",x*3,x*x,x/2);   
}

4.
#include <stdio.h>

float x = 0;

int main(){   
    printf("Entre com o valor da conta:\n");
    scanf("%f",&x);

    printf("O valor total da conta é:%.2f\n",x*1.1);
}

5.
#include <stdio.h>

float x = 0;
char sexo;

int main(){   
    printf("Entre com a altura:\n");
    scanf("%f",&x);
    printf("Entre com o sexo(F/M):");
    scanf(" %c",&sexo);

    if(sexo != 'F' && sexo != 'M'){
        printf("Sexo inválido!");
    }
    switch (sexo){
        case 'F':
        printf("O seu peso ideal é:%.2f\n",(62.1*x)-44.7);
        break;

        case 'M':
        printf("O seu peso ideal é:%.2f\n",(72.7*x)-58);
        break;
    }  
}

6.
#include <stdio.h>

int x = 0, y = 0, z = 0;
int horas = 0, minutos = 0, segundos = 0;

int main(){   
    printf("Entre com a quantidade de horas:\n");
    scanf("%d",&x);
    printf("Entre com a quantidade de minutos:\n");
    scanf("%d",&y);
    printf("Entre com a quantidade de segundos:\n");
    scanf("%d",&z);

    horas = x * 60 * 60;
    minutos = y * 60;
    segundos = horas + minutos + z;

    printf("%d Horas, %d minutos e %d segundos é igual %d segundos.",x,y,z,segundos);    
}

7.
#include <stdio.h>

int x = 0;
    

int main(){   
    printf("Entre com o número:\n");
    scanf("%d",&x);
    printf("%d\n",x*x);
}

8.
#include <stdio.h>

int x = 0;
    
int main(){   
    printf("Entre com o número:\n");
    scanf("%d",&x);
    printf("Antecessor:%d\nSucessor:%d\n",x-1,x+1);
}

9.#include <stdio.h>

float real = 0, dolar = 0, cotacao = 0; 

int main(){ 
    printf("Qual a cotação do dolar?:\n"); 
    scanf("%f",&cotacao); 
    printf("Qual o valor em real para câmbio?\n"); 
    scanf("%f",&real);
 
    printf("O valor em dolar é:%.2f\n",real*cotacao); 
}  

