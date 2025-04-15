# Aprenda JoilsonGol
O que é JoilsonGol, basicamente é um apelido para o a linguagem de algorítmos que o grande Joilson usa em suas aulas de algoritmos.

## Por que devemos aprender JoilsonGol?
A Resposta mais direta é: Porque sim! 



# Começando!
## 1. Estrutura
A estrutura no JoilsonGol é algo bastante forte e nela contempla algumas "Obrigações" como"
### 1.1 Escopos
Escopos são "áreas" onde as instruções são escritas, por exemplo todo o algoritmo de um programa deve estar dentro de um escopo principal que irá dizer para o computador onde começa e termina o pograma.

No JoilsonGol é utilizado um padrão de escopo em forma de blocos, ou seja, tem uma instrução que define o inicio e o fim de um escopo.

> _(Para quem já é familiarizado com o mundo da programação, ele parece muito com o sistema de blocs/escopos do Ruby)_

Para determinarmos início de um escopo utilizamos a palavra/termo `inicio` e para determinar o fechamendo to escopo usamos o `fim.`

Utilizando em um exemplo ficará assim:
```
inicio
    bla bla bla;
    ble ble ble;
    blu blu blu;
fim.
```

> Explicação do exemplo: O Escopo irá compreender as instruçõe bla bla, ble ble e blublu e determina onde começa e termina, pois algoritmos são passos finitos para resolver um problema.

### 1.2 Instruções
Instruções é tudo aquilo que determina uma ação que será executada pelo computador. E todas devem conter um `;` que irá dizer para o computador que a instrução acabou. 

> Exemplos de instruções:
```
escreva();
leia();
VarX <- 10 + 1;
``` 

### 1.3 Identação
Uma coisa que não pode faltar no JoilsonGol é a identação, pois com ela o nosso programa fica mais organizado e legível.

> _Para quem estiver começando agora, cuidado o Joilson/Betinha tira pontos se pecar nessa parte_

A identação é algo bastante simples e fácil de entender, iremos pensar nela como se fosse a relação de **pai** e **filho**, o filho é subordinado ao pai. Trazendo para o algorítmo podemos pensar que o escopo principal é o pai de todo o programa e as instruções posteriores estará subordinadas a ele, como um filho.

> Exemplo:
```
inicio
    escreva("Joilson é o melhor professor");
fim.
```

Você percebeu que a instrução `escreva` ela está recuada para dentro? Então, isso é a identação, em outras palavras, é um recuo dentro do código.

## 2. Variáveis
Este é um ponto que é bastante cobrado, pois ele é a base que é usada em todas as linguágens de programação.

### 2.1 O que é uma variável?
Podemos pensar em uma variável como se fosse uma gaveta em que podemos guardar objetos, e podemos modificar e acessar esse objeto empre que precisarmos.

### 2.2 Tipos de variáveis
Uma pergunta, já tentou guardar algo maior que a gaveta dentro dela? É impossível.

É a mesma coisa com as variáveis, existem **gavetas** específica para cada tipo de objeto.

Em algaritmos, esses tipos de gavetas são os tipos das variáveis.

Esses tipos são:
- **inteiros**: esse tipo de variável suporta apenas números inteiros positivos e negaativos, ex: 1, 2, 4, 5;
- **reais**: armazena números decimais (números com vírgula), ex: 1.05, 0.005, 10.2;
- **logico**: armazena apenas a informação **verdadeira** ou **falsa**;
- **caractere**: armazena caracteres (letras), ex: nome de uma pessoa; 

### 2.4 Declaração de Variáveis
Antes de usarmos uma variável em nosso programa devemos dizer para o computador para "criar" uma gaveta do tipo que precisamos na memória do computador.

Para fazermos isso é muito simples, basta escrever o tipo da variável e o nome que queremos atribuir para ela.

> Exemplo: 
```
inicio
    real: NomeVariavelReal;
    inteiro: NomeVariavelInteira;
    logica: NomeVariavelLogica;
    caractere: NomeCaractere;
fim.
```

Outro assunto que é muito cobrado é as regras de determinação do nome da variável.

São elas:
- **PascalCase**: O nome da variável deve ser escrita na convenção do PascalCase, então toda letra inicial de uma palavra deve ser maiúscula, ex: IdadeLimite, Idade, QuantidadeLitros.
_(Se for composta, ficará em maiúsculo a inicial de cada palavra)_;
- **APENAS letras na primeira letra**: A primeira letra do nome da variável nunca poderá ser um número;
- **PROIBIDO simbolos**: Simbolos como: _, @, #, $, %, etc. Não é aceito no JoilsonGol.
- **Seja claro**: Não use nomes genéricos, pois dificulta o entendimento do código.

### 2.5 Manipulação de variáveis
As variáveis são algo muito importante, pois com elas podemos "brincar" com as informações que são guardadas nelas.

#### 2.5.1 Determinação do valor
Utilizamos o sinal `<-` _(setinha)_ para atribuir um valor para a variável.

> Exemplo:
```
inicio
    caractere: NomePessoa;

    NomePessoa <- "Joilson";
fim.
```

Nesse exemplo estamos atribuindo para a variável `NomePessoa` o valor `Joilson` e toda vez que referirmos a variável `NomePessoa` será retornado o valor `Joilson`



