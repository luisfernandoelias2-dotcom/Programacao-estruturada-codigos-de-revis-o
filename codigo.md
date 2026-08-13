#include <stdio.h>
int soma(int a, int b);
int eh_par(int n);
int maior(int a, int b);
int potencia(int base, int expoente);
int fatorial(int n);
/* ============================================================
PROGRAMA PRINCIPAL
============================================================ /
int main(void) {
int a = 4, b = 6, r;
/ TODO: chamar a fun o soma e armazenar o resultado em r */
r = soma (a, b);
printf("Soma: %d\n", r);

/* TODO: chamar a fun o eh_par */
printf("Par: %d\n", eh_par(a));

/* TODO: chamar a fun o maior */
printf("Maior: %d\n", maior(a, b));

/* TODO: chamar a fun o potencia */
printf("Potencia: %d\n", potencia(a, b));

/* TODO: chamar a fun o fatorial /
printf("Fatorial: %d\n", fatorial(a));
return 0;
}
/ ============================================================
EXERC CIO 1 Soma de dois numeros
============================================================ /
int soma(int a, int b) {
/ TODO: retornar a soma de a e b /
return a+b;
}
/ ============================================================
EXERC CIO 2 Verificar numero par
============================================================ /
int eh_par(int n) {
/ TODO: retornar 1 se n for par, 0 caso contrario /
if (n%2== 0){
return 1;
}
else {
return 0;
}
}
/ ============================================================
EXERC CIO 3 Maior de dois numeros
============================================================ /
int maior(int a, int b) {
/ TODO: retornar o maior valor entre a e b /
if (a>b){
return a;
}
else {
return b;
}
}
/ ============================================================
EXERC CIO 4 Potencia
============================================================ /
int potencia(int base, int expoente) {
/ TODO: calcular base^expoente sem usar pow */
int resultado = 1;
for (int i = 0; i < expoente; i++) {
resultado = resultado * base;
}

return resultado;
}
/* ============================================================
EXERC CIO 5 Fatorial
============================================================ /
int fatorial(int n) {
/ TODO: calcular e retornar o fatorial de n */
int resultado = 1;
for (int i = n; i>0; i--){
resultado = resultado * n;
}

return resultado;
}
/*Outra forma de fazer:
while (n > 0) {
resultado = resultado * n;
n--;
}

return resultado;
}
*/
