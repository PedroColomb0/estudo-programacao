#### ele guarda valores dentro de propriedades, propriedades e valores

``` js

const person = {

    // ele guarda valores dentro de propriedades, propriedades e valores

    firstName : "Pedro",

    lastName : "Colombo",

    age : 21,

    hobbies : ['Assistir F1', 'Jogar Futebol', 'Ler']

}

  

const firstName = person.firstName

const lastName = person.lastName

const age = person.age

const hobbies = person.hobbies

  

// Acessar index da Array

const read = person.hobbies[2]

  

console.log(firstName)

console.log(lastName)

console.log(age)

console.log(hobbies)

  
  

console.log(read)

```

# Destructuring

``` js
const person = {
    firstName : "Pedro",
    lastName : "Colombo",
    age : 21,
    hobbies : ['Assistir F1', 'Jogar Futebol', 'Ler']
}

// const firstName = person.firstName
// const lastName = person.lastName
// const age = person.age
// const hobbies = person.hobbies

// mesma coisa do que fazer acima

const {age,firstName,lastName,hobbies} = person

// podemos renomear tambem com os :
const {age : idadenova ,firstName,lastName,hobbies} = person2

console.log(person)

```

# Adicionar Propriedade a um objeto

``` js
const person = {

    firstName : "Pedro",

    lastName : "Colombo",

    age : 21,

    hobbies : ['Assistir F1', 'Jogar Futebol', 'Ler'],

    dog2 : {

        name : "Simba",

        age : 4,

    },

}

  

const {age,firstName,lastName,hobbies} = person

  

// para Adicionarmos propriedade a um objeto (nesse caso a person)

person.dog = "Simba"

  

console.log(person)

  

console.log()

```

# Utilizando lista com objetos

``` js

// O que vamos mais ver no dia dia ~e uma lista contendo varios objetos

  

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

  

// acessar o index

console.log(todos[2])

  

// acessar propriedade especifica

console.log(todos[2].description)

```