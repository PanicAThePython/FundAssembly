# FundAssembly
  
  * Os números devem ser escritos em hexadecimal e com dois dígitos. Exemplo: ao invés de A, escreva 0A.
  * Para fazer operações, primeiro copie o valor para A e, depois, guarde em algum outro repositório para não perder o valor.

## Comandos da linguagem ASSEMBLY
* **MOV:** copia o valor para um registrador da M++(A, B, C, D ou E)
    * Exemplos: 
      * MOV 01, A; //copia o valor 1 para A
      * MOV #00, A; //copia o valor guardado na primeira posição da memória RAM para A
      * MOV A, B; //copia o valor de A para B
* **PUSH:** copia o valor e manda para a memória de pilha
    * Exemplo: PUSH B; //faz backup do valor de B

* **POP:** recupera o valor presenta na pilha (o valor deve ser pego de volta na ordem que foi posto. Exemplo: se guardei o valor de A, e depois B, devo primeiro recuperar B e depois A)
    * Exemplo: POP B; //recupera o valor de B
    
* **JMP:** pula para um pedaço do código
    * Exemplo: JMP INICIO; //pula para o rótulo INICIO

* **CALL:** chama uma função (TODA FUNÇÃO TERMINA COM UM RET)
    * Exemplo: CALL IMPRIMIRFRASE; //chama a função de tal nome
    
* **RET:** faz a função, quando terminar de executar, voltar para a linha onde foi chamada
