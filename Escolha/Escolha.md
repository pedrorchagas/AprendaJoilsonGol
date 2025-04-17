# 3 Escolha
**O que é o escolha?** O escolha é uma instrução que utilizamos quando precisamos fazer diversas verificações sobre uma variável.

> Exemplo: Um sistema que define a a linguagem de um programa, fazendo com o Se e Senão fica assim:
```
inicio
    caractere: Linguagem, OpcaoUsuario;

    escreva("Qual que será usado pelo programa?);
    leia(OpcaoUsuario);

    se(OpcaoUsuario = "Inglês")
        então
            Linguagem <- "US";
        senão
            se(OpcaoUsuario = "Alemão")
                então
                    Linguagem <- "DE";
                senão
                    se(OpcaoUsuario = "Akazam")
                        então
                            Linguagem <- "AK";
                        senão
                            se(OpcaoUsuario = "Português")
                                então
                                    Linguagem <- "PT-BR";
                                senão
                                    Liguagem <- "Desconhecida
                            fimse.
                    fimse.
            fimse.
    fimse.

    escreva("Linguagem escolhida foi: ", Linguagem);
fim 
```
Podemos ver que fica muito complicado e difícil entender esse código desse tamanho e quebrado.

> Com o escolha podemos fazer assim:
```
inicio
    caractere: Linguagem, OpcaoUsuario;

    escreva("Qual que será usado pelo programa?);
    leia(OpcaoUsuario);

    escolha(OpcaoUsario)
        caso "Inglês": Linguagem <- "US";
        caso "Alemão": Linguagem <- "DE";
        caso "Akazam": Linguagem <- "AK";
        caso "Português": Linguagem <- "PT-BR";
        caso contrário: Linguagem <- "Linguagem desconhecida";
    fimescolha.

    escreva("Linguagem escolhida foi: ", Linguagem);
fim.
```
> Podemos ver que o código ficou bem mais menor e fácil de entender.

Uma coisa que podemos fazer com o escolha é criar uma `Bloco` para quando for preciso fazer mais de uma instrução.

> Exemplo de um menu interativo:
```
inicio
    inteiro: OpcaoUsuario;
    caractere: UF

    escreva("ESCOLHA O SEU ESTADO");
    escreva("1     GOIAS");
    escreva("2     RIO DE JANEIRO");
    escreva("3     RIO GRANDE DO SUL");
    escreva("4     CEARÁ");
    escreva("5     SÃO PAULO");
    leia(OpcaoUsuario);

    escolha(OpcaoUsuario)
        caso 1: 
            inicio
                escreva("Você mora no melhor estado do Brasil!!! <3 ");
                UF <- "GO";
            fim;
        caso 2: UF <- "RJ";
        caso 3: UF <- "RS";
        caso 4: UF <- "CE";
        caso 5: UF <- "SP";
        caso contrário: UF <- "UF DESCONHECIDO";
    fimescolha.
fim.
```
Podemos ver que no caso `1` colocamos marcamos um bloco de instruções com `inicio` em `fim` e dentro dele colocamos as instruções.

**OBS:** Isso já caiu em APAs. Preste atencão!