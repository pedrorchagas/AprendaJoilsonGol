## 2. Variáveis
Este é um ponto que é bastante cobrado, pois ele é a base que é usada em todas as linguágens de programação.

### 2.1 O que é uma variável?
Podemos pensar em uma variável como se fosse uma gaveta em que podemos guardar objetos, e podemos modificar e acessar esse objeto empre que precisarmos.

### 2.2 Tipos de dados
Uma pergunta, já tentou guardar algo maior que a gaveta dentro dela? É impossível.

É a mesma coisa com as variáveis, existem **gavetas** específica para cada tipo de objeto.

Em algaritmos, esses tipos de gavetas são os tipos das variáveis.

Os tipos primitivos são:
- **inteiros**: esse tipo de variável suporta apenas números inteiros positivos e negaativos, ex: 1, 2, 4, 5;
- **reais**: armazena números decimais (números com vírgula), ex: 1.05, 0.005, 10.2;
- **logico**: armazena apenas a informação **verdadeira** ou **falsa**;
- **caractere**: armazena caracteres (letras), ex: nome de uma pessoa.

### 2.3 Declaração de Variáveis
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
- **PROIBIDO simbolos**: Simbolos como: _, @, #, $, %, etc. Não é aceito no JoilsonGol;
- **Seja claro**: Não use nomes genéricos, pois dificulta o entendimento do código;
- **Nome único**: O nome da variável deve ser unico para evitar conflitos.

### 2.4 Manipulação de variáveis
As variáveis são algo muito importante, pois com elas podemos "brincar" com as informações que são guardadas nelas.

#### 2.4.1 Determinação do valor
Utilizamos o sinal `<-` _(setinha)_ para atribuir um valor para a variável.

> Exemplo:
```
inicio
    caractere: NomePessoa;

    NomePessoa <- "Joilson";
fim.
```

Nesse exemplo estamos atribuindo para a variável `NomePessoa` o valor `Joilson` e toda vez que referirmos a variável `NomePessoa` será retornado o valor `Joilson`

> Outro exemplo:
```
inicio
    inteiro: AnoAtual;
    AnoAtual <- 2025;
    escreva(AnoAtual)
fim.
```
> Neste exemplo, estamos definindo o o valor `2025` para a variável `AnoAtual`

#### 2.4.2 Moficação de valor da variável
Durante a execução do programa podemos alterar o valor da variável quantas vezes quisermos.

> Exemplo:
```
inicio
    real: SaldoBancario;

    SaldoBancario <- 10.50;
    SaldoBancario <- 20.00;
    SaldoBancario <- 30.00;
    SaldoBancario <- 99080.01;
    
    escreva(SaldoBancario);
fim.
```
> Neste exemplo definimos a variável `SaldoBancario` e alteramos o valor dentro da _"gaveta"_ dessa variável toda vez que utilizamos o operador de definição `<-`. portanto, ao usar a funcão `escreva(SaldoBancario)` o programa irá escrever o valor `99080.01` que é o mesmo valor definido por ultimo.

#### 2.4.3 Operações com variáveis
Assim como na matemática podemos usar as variáveis dentro de formulas, como funções do primeiro grau. E com essa funcionalidade podemos criar programas que processam diversos dados de entrada para mostrar na saida.

Para demonstrar essa funcionalidade iremos criar um programa que multiplica qualquer entrada por 2.

_Esse caso iremos usar operadores matemáticos, caso tenha dúvida, temos um tópico separado sobre eles._

> Pensamento matemático:
```
y = X.2
```
Utilizando esse conceito no programa ele irá ficar assim:


> Código:
```
inicio
    real: ValorEntrada, ValorSaida;

    leia(ValorEntrada);

    ValorSaida <- ValorEntrada * 2;

    escreva(ValorSaida);
fim.
```
> Analisando o código, podemos ver que, basicamente, as letras `x` e `y` foram substituidas por `ValorEntrada` e `ValorSaida`.E o restante da lógica matemática continua igual.

Com isso podemos fazer programas mais complexos, e para demostrar isso iremos criar um programa que calcule a velocidade média de um carro.

> Pensamento matemático/fisica:
```
vm = ΔS/ΔT ≈ vm = (Sf - Si)/(Tf - Ti) ≈ vm = Sf/Tf
```

> Código:
```
inicio
    real: VelocidadeMedia, Tempo, Espaco;

    //Entrada de dados
    escreva("Informe o tempo e o espaço percorrido");
    leia(Tempo);
    leia(Espaco);

    //Processamento
    VelocidadeMedia <- Espaco/Tempo;

    //Saida
    escreva("A velocidade média foi: ", VelocidadeMedia);
fim.
```
> Com isso podemos perceber que as variáveis tem um funcionamento semelhante ao da matemática.

> OBS: A funcão `leia()` é o comando que permite que o usuário insira dados.


> Outro exemplo mais complexo:

Logica matemática: Para encontrar a idade de uma pessoa basta subtrair o ano atual pelo ano de nascença.
```
inicio
    // Definição das variáveis
    inteiro: AnoNascimento, IdadeAtual, AnoAtual;
    AnoAtual <- 2025; //Isso é uma constante, pois tem um valor fixo.

    // Entrada de dados
    AnoNascimento <- 2006;

    // Processamentos dos dados
    IdadeAtual <- AnoAtual - AnoNascimento;

    // Saida de dados
    escreva(IdadeAtual);
fim.
```
> Neste exemplo mais complexo podemos ver que declaramos duas variáveis ao mesmo tempo, `AnoNascimento` e `IdadeAtual`, podemos fazer isso para quantas variáveis do mesmo tipo.