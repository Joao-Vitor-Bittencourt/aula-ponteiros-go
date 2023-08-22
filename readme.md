# Golang Assíncrono - Introdução à ponteiros.

Video do canal [Huncoding](https://www.youtube.com/watch?v=FLIWsfS9gTg&list=PLm-xZWCprwYQz7Di62Z93zGHyLC-HkFpb)

### Introdução

O ponteiro é muito util em Go, e por isso é muito usado, sua função é, resumidamente, criar uma cópia de algum valor para que o original não seja alterado.

### O que é são ponteiros em go?

São variáveis usadas para armazenar o endereço na memória de outra variavel. Também são chamados de variáveis especiais. As variáveis são usadas para armazenar alguns dados em um endereço de memória específico no sistema. Esses endereços são sempre armazenados com no formato hexadecimal, começando com “0x” por exemplo, 0xFFAAF.

### Porque usar ponteiros?

Imagine a seguinte situação, você tem um banco com diferentes planos de investimento, e quer mostrar ao cliente quais alterações ele teria em seu saldo de acordo com cada plano, nessa situação você não desejaria alterar o saldo real, apenas utilizar o valor para realizar os cálculos de cada plano de investimento.

### Operadores * e &

Em go um ponteiro é representado usando o caractere * (asterisco) seguido pelo tipo de  valor armazenado.

*** Também é usado para “desreferenciar”** variáveis de ponteiro. Cancelar a referência de um ponterio nos dá acesso ao valor para o qual o ponteiro aponta quando escrevemos * xPTr = 0, estamos dizendo “armazene o int 0 no local de memória a que xPtr se refere”. Se tentarmos xPtr = 0, obteremos um erro do compilador porque xPtr não é um int, é um *int, que só pode receber outro *int.

Finalmente, ******************************************************************************************************************************usamos o operador & para encontrar o endereço de uma variável.****************************************************************************************************************************** & x retorna um * int (ponteiro para um int) porque x é um int. Isso é o que nos permite modificar a variável original. & x em principal e xPtr em zero referem-se ao mesmo local de memória.