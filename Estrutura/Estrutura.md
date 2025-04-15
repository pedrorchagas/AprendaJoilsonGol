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