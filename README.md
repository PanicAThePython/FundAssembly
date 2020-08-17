# FundAssembly
  Exercícios de Arquitetura de Computadores e sintaxe do ASSEMBLY.
  
  * Os números devem ser escritos em hexadecimal e com dois dígitos. Exemplo: ao invés de A, escreva 0A.
  * Para fazer operações, primeiro copie o valor para A(registrador) e, depois de fazer a operação, guarde em algum outro registrador para não perder o valor.

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
    
* **SUB:** subtrai um valor de A e guarda em um registrador da preferência do programador
    * Exemplo: SUB 03, A;
    
* **ADD:** soma valores ao de A e guarde em um registrador da preferência do programador
    * Exemplo: ADD 03, A;

* **INC:** soma 01 no valor de um resgistrador;
    * Exemplo: INC B;
    
* **JMP:** pula para um pedaço do código
    * Exemplo: JMP INICIO; //pula para o rótulo INICIO
    
* **JMPZ:** pula para um rótulo quando a resposta da subtração for ZERO!
    * Exemplo:
              MOV 01, A; //copia 01 pra A
              SUB 01, A; //subtrai 01 de A e guarda em A
              JMPZ FIM; //se a resposta for zero, pula pra FIM

* **JMPC:** pula para um rótulo quando a resposta da subtração for NEGATIVA! EXEMPLO: A tem 03 e subtraio 04, vai acender o FLAG C!!

* **CALL:** chama uma função (TODA FUNÇÃO TERMINA COM UM RET)
    * Exemplo: CALL IMPRIMIRFRASE; //chama a função de tal nome
    
* **RET:** faz a função, quando terminar de executar, voltar para a linha onde foi chamada
