
Quando estamos transitando dados entre um frontend e um backend, nao conseguimos enviar uma lista ou um objeto em javascript, mas enviamos sim um json o que é esse json

### Converter Array para Json

``` js

const todos = [

    {
        id: 1,
        description: "Estudar programação",
        isCompleted : false
    },
    {

        id: 2,
        description: "Ler",
        isCompleted : true
    },
    {
        id: 3,
        description: "Treinar'",
        isCompleted : true
    },

  

]

  

// para enviarmos para uma api(servidor), temos que converter esse cara para json

const todosJson = JSON.stringify(todos)
console.log(todosJson)


// Ele nao é mais uma lista e sim um Json e sim uma string num formato json

```

### Converter Json para Array

``` js

const todos = [

    {

        id: 1,

        description: "Estudar programação",

        isCompleted : false

    },

    {

        id: 2,

        description: "Ler",

        isCompleted : true

    },

    {

        id: 3,

        description: "Treinar'",

        isCompleted : true

    },

  

]

  

const todosJson = JSON.stringify(todos)

  

// aqui

const todoList = JSON.parse(todosJson)

console.log(todoList)

```