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

9.
#include <stdio.h>

int main(){

    int volume = 0, altura = 0, largura =0, comprimento = 0;

    printf("Entre com o comprimento:\n");
    scanf("%d",&comprimento);
    printf("Entre com a largura:\n");
    scanf("%d",&largura);
    printf("Entre com a altura:\n");
    scanf("%d",&altura);

    volume = comprimento*largura*altura;

    printf("O valor do volume da caixa é:%d\n",volume);
    
}

10.
#include <stdio.h>

float real = 0, dolar = 0, cotacao = 0; 

int main(){ 
    printf("Qual a cotação do dolar?:\n"); 
    scanf("%f",&cotacao); 
    printf("Qual o valor em real para câmbio?\n"); 
    scanf("%f",&real);
 
    printf("O valor em dolar é:%.2f\n",real*cotacao); 
}  

11.
#include <stdio.h>

int main(){

    int num1 = 0, num2 = 0;
    int soma = 0, produto = 0, diferenca = 0 ,quociente = 0, resto =0; 

    printf("Entre com o primeiro número:\n");
    scanf("%d",&num1);
    printf("Entre com o segundo número:\n");
    scanf("%d",&num2);

    soma = num1 + num2;
    produto = num1 * num2;
    diferenca = num1 - num2;
    quociente = num1 / num2;
    resto = num1 % num2;

    printf("Os resultados são:\n-Soma = %d\n-Produto = %d\n-Diferença = %d\n-Quociente = %d\n-Resto = %d\n",soma,produto,diferenca,quociente,resto);
}

12.
#include <stdio.h>

int main(){

    int a = 0, b = 0;

    printf("Entre com o valor de A:\n");
    scanf("%d",&a);
    printf("Entre com o valor de B:\n");
    scanf("%d",&b);

    a ^= b;
    b ^= a;
    a ^= b;

    printf("O valor de A é:%d\nO valor de B é:%d\n",a,b);
}

13.
#include <stdio.h>

int main(){

    float c = 0, f = 0;

    printf("Entre com a temperatura em graus celcius:\n");
    scanf("%f",&c);

    f = (9 * c + 160) / 5;

    printf("A temperatura em Fahrenheit é:%.1f\n",f);
}

14.
#include <stdio.h>

int main(){

   int dias_trabalhados = 0;
   float salario = 0, diaria = 50.25;

   printf("Entre com a quantidade de dias trabalhados:\n");
   scanf("%d",&dias_trabalhados);

   salario = (float)dias_trabalhados * diaria;

   if(dias_trabalhados >= 10 && dias_trabalhados <= 20){
       salario = salario * 1.2;
   } 
   if(dias_trabalhados > 20){
       salario = salario * 1.3;
   }

   salario = salario * 0.9;

   printf("O salario total é:%.2f\n",salario);
}

15.
#include <stdio.h>

int main(){

    float valor_hora = 0, horas_trab = 0, inss = 0, salario_br = 0, salario_liq = 0;

    printf("Entre com o valor da hora trabalhada:\n");
    scanf("%f",&valor_hora);
    printf("Entre com o número de horas trabalhadas:\n");
    scanf("%f",&horas_trab);
    printf("Entre com o valor do desconto do INSS em %%:\n");
    scanf("%f",&inss);

    salario_br = valor_hora * horas_trab;
    salario_liq = salario_br - (inss*0.01 * salario_br);

    printf("Valor do salário bruto:%.2f\nValor do salário liquido:%.2f\n",salario_br,salario_liq);
}

16.
#include <stdio.h>

int main(){

    int numero = 0, valor_abs = 0;

    printf("Entre com o número:\n");
    scanf("%d",&numero);

    valor_abs = (numero < 0) * -numero + (numero >= 0) * numero;

    printf("Valor absoluto:%d\n",valor_abs);    
}

17.
#include <stdio.h>

int main(){

    float pi = 3.14159, raio = 0, diametro = 0, circunferencia = 0, area = 0;

    printf("Entre com o valor do Raio:\n");
    scanf("%f",&raio);
    printf("Diametro:%.4f\nCircunferência:%.4f\nÁrea:%4.f\n",2.0*raio,(2.0*pi)*raio,pi*(raio*raio));
    
}

18.
#include <stdio.h>

int main(){
   printf("\n********       ***         *              *");
   printf("\n*      *     *     *      ***           *   *");
   printf("\n*      *   *         *   *****        *       *");
   printf("\n*      *   *         *     *        *           *");
   printf("\n*      *   *         *     *      *               *");
   printf("\n*      *   *         *     *        *            *");
   printf("\n*      *   *         *     *          *        *");
   printf("\n*      *    *       *      *            *    *");
   printf("\n********       ***         *              *");
}

19.
#include <stdio.h>

int main(){
   
    int numero = 0;
    char* resultado;

    printf("Entre com o núemro:\n");
    scanf("%d",&numero);

    resultado = (numero % 2 == 0) ? "par" : "ímpar";

    printf("O número %d é %s\n",numero,resultado);
}

20.
#include <stdio.h>

int main(){
   
    int num1 = 0, num2 = 0;
    char* resultado;

    printf("Entre com o primeiro número:\n");
    scanf("%d",&num1);
    printf("Entre com o segundo número:\n");
    scanf("%d",&num2);

    resultado = ((num1 % num2 == 0 && num2 != 0) || num2 % num1 == 0 && num2 !=0 ) ? "Multiplo" : "Não multiplo";

    printf("O número %d é %s de %d\n",num1 ,resultado, num2);
}

21.
#include <stdio.h>

int main() {
    printf("Conjunto:\nA    %d\nB    %d\nC    %d\na    %d\nb    %d\nc    %d\n0    %d\n1    %d\n2    %d\n$    %d\n*    %d\n+    %d\n/    %d\n     %d\n",'A','B','C','a','b','c','0','1','2','$','*','+','/',' ');
}

22.
#include <stdio.h>

int main() {
    int numero = 0, centena = 0, dezena = 0, unidade = 0, inverso = 0;

    printf("Entre com um número de 3 digitos:\n");
    scanf("%d",&numero);

    centena = numero / 100;
    dezena = (numero % 100) / 10;
    unidade = numero % 10;

    inverso = (unidade * 100) + (dezena * 10) + centena;

    printf("O número invertido é igual:%d\n",inverso);
}

23.
#include <stdio.h>

int main() {
    int x, n, resultado;

    printf("Entre com o valor x:\n");
    scanf("%d",&x);
    printf("Entre com o valor n:\n");
    scanf("%d",&n);

    resultado = x << n;

    printf("%d",resultado);
}

24.
#include <stdio.h>

int main() {
    int total_seg = 0, horas = 0, minutos = 0, segundos = 0;

    printf("Entre com a quantidade total de segundos:\n");
    scanf("%d",&total_seg);

    horas = total_seg / 3600;
    minutos = (total_seg % 3600) / 60;
    segundos = total_seg % 60;

    printf("São %d horas, %d minutos, %d segundos.\n",horas,minutos,segundos);
}

25.
#include <stdio.h>
#include <math.h>

int main() {
    float x1 = 0, x2 = 0, y1 = 0, y2 = 0, distancia = 0;

    printf("Entre com o valor de X1:\n");
    scanf("%f",&x1);
    printf("Entre com o valor de X2:\n");
    scanf("%f",&x2);
    printf("Entre com o valor de Y1\n");
    scanf("%f",&y1);
    printf("Entre com o valor de Y2:\n");
    scanf("%f",&y2);

    distancia = sqrt(pow(x2-x1,2)+pow(y2-y1,2));

    printf("A distância entre os pontos é:%.2f",distancia);
}

26.
#include <stdio.h>
#include <math.h>

int main() {
    float num1 = 0, num2 = 0, num3 = 0, med_aritmetica = 0, med_geometrica = 0;

    printf("Entre com o primeiro número:\n");
    scanf("%f",&num1);
    printf("Entre com o segundo número:\n");
    scanf("%f",&num2);
    printf("Entre com o terceiro número:\n");
    scanf("%f",&num3);

    med_aritmetica = (num1 + num2 + num3) / 3;
    med_geometrica = pow(num1 * num2 * num3, 1.0 / 3.0);

    printf("Média aritmética:%.2f\nMédia Geométrica:%.2f",med_aritmetica,med_geometrica);
}
