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