# URI-1168-c
/*Entrada  A entrada contém um inteiro N, (1 ≤ N ≤ 1000) correspondente ao número de casos de teste, 
seguido de N linhas, cada linha contendo um número (1 ≤ V ≤ 10100) correspondente ao valor que João quer montar com os leds. 
Saída  Para cada caso de teste, imprima uma linha contendo o número de leds que João precisa para montar o valor desejado, 
seguido da palavra "leds".*/

#include <stdio.h>

int main(){
    int n, s, l[10] = {6, 2, 5, 5, 4, 5, 6, 3, 7, 6};
    char d;
    scanf("%d", &n);
    getchar();
    while(n--){
        s = 0;
        while((d = getchar()) != '\n'){
            s += l[d - '0'];
        }
        printf("%d leds\n", s);
    }
    return 0;
}

