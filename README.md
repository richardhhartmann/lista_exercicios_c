## Lista de exercícios Estrutura de Dados 1

##### **Abstract.** This project aims to answer a list of exercises in the question Structures of Data I, through the knowledge acquired in the classroom, and creativity and imagination in solving problems. With the help of the complementary material provided by Professor Juliano Ratusznei, it is possible to understand the requirements of the exercise, divide it into parts and arrive at a logical result that satisfies the problem.


##### **Resumo.** Este trabalho visa responder a uma lista de exercícios na questão Estruturas de Dados I, através do conhecimento adquirido em sala de aula, e criatividade e imaginação na resolução de problemas. Com a ajuda do material complementar fornecido peloprofessor Juliano Ratusznei, é possível entender os requisitos do exercício, dividi-lo em partes e chegar a um resultado lógico que satisfaça o problema.


## Descrição do exercício 1 a ser solucionado:
### Escreva um programa para escrever quando inicializado “Olá aluno hoje é sexta-feira”

## Resolução do exercício - Codificação:

```
#include <stdio.h>
#include <stdlib.h>
#include <locale.h>
int main(void)
{
 setlocale(LC_ALL, "Portuguese");
// aqui o programa irá imprimir a frase. 
 printf("Olá aluno hoje é sexta-feira"); 
 system("pause");
 return 0;
}
```

## Execução do exercício - Resolução
##### Figura 1: tela da solução do exercício 1.
<img src="/src/img1.png"><br/><br/>

## Descrição da aprendizagem obtida através da problemática:
### Através do exercício, é compreendido o funcionamento da função “printf” como ferramenta de impressão ou exibição na tela do terminal uma lista formatada de números, caracteres, strings e entre outros.

## Descrição do exercício 2 a ser solucionado:
###Dado a entrada via teclado do nome de usuário (seu nome) escrever na tela “Bem-vindo nome de usuário”

## Resolução do exercício - Codificação:

```
#include <stdio.h>
#include <stdlib.h>
#include <locale.h>
int main(void){
 setlocale(LC_ALL, "Portuguese");
 int i = 1; // criação da variável i para o primeiro loop de repetição do programa
 int sair;
 while (i == 1) { // primeiro loop de repetição do programa
 char nome[99];
 printf("Digite o seu nome: ");
 scanf("%s", &nome); // aqui o usuário dará entrada no nome
 printf("Bem-vindo, %s\n\n", nome); // aqui o programa ira printar o nome do usuário
 i = 0;
 int aux = 1; // criação da variável auxiliar para o segundo loop de repetição do 
programa
 while (aux == 1) { // segundo loop de repetição do programa
 printf("Deseja executar o programa novamente? Digite 1 para sim e 0 para não: \n");
 scanf("%d", &sair);
 aux = 0;
 if (sair == 1) {
 i = 1;
 } else if (sair == 0) {
 i = 0;
 break;
 } else {
 printf("O valor digitado é inválido! Tente novamente. \n\n");
 aux = 1;
 }
 i = 1;
 }
 }
 system("pause");
 return 0;
}
```

## Execução do exercício - Resolução
##### Figura 2: tela da solução do exercício 2.
<img src="/src/img2.png"><br/><br/>

