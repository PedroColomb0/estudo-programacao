# Map

``` js
const numbers = [1,2,3,4,5]

// Temos o problema que seria multiplicar todos os numeros por 2 dessa lista, para isso podemos usar o map, ele o map vai executar uma determinada funcao em cada item

// e vai retornar uma nova lista com essa funcao executada em todos os itens

const numbersMultipliedByTwo = numbers.map((itemAtual) =>
   // como vai ser em todos os itens, nosso props seria item por item, porque seria tipo index por index
   // agora vamos  retornar o que queremos executar em cada number
    itemAtual * 2

)

  

console.log(numbersMultipliedByTwo)

// Todos os numeros estao multiplicados por 2,essa funcao foi executada em cada 1 dos numeros daqui. Meio que ele vai fazer um loop,

// perrcorendo em todos os itens da lista e fazendo a alteracao nesse index por index.
````


# Filter

``` js

// Temos a missao de pegar só as idades que são pares dentro dessa lista, seria algo como de fato filtrar dentro da lista baseado na condicao que queremos

// entao vamos filtrar uma lista e vamos retornar uma lista nova baseando o filtro que passamos.

  

const ages = [8,13,27,30,22,40]

  

const evenAges = ages.filter((itemAtual) =>

    // Resto da Divisao

     itemAtual % 2 === 0

)

  

console.log(evenAges)

  

// resposta [ 8, 30, 22, 40 ]
 
```

# Reduce

``` js

// Reduce, ele é util quando queremos reduzir todos os valores da nossa lista para um só.

  

const ages = [8,13,27,30,22,40]

  

// Exemplo vamos supor que nossa misão agora é pegar a soma de todas as idades, somar todos os valor, entao voce concorda que queremos somar tudo

// entao queremos reduzir esse valor da lista para um valor só que no caso é a soma dele

  

const sumOfAges = ages.reduce((age, accumulator) => {

    // esse accumulator seria basicamente o valor atual da acomulacao de todas as edicoes dessa funcao aqui

}, 0)

```

