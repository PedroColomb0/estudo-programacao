
# Classes

As classes em JavaScript são basicamente impressoras de objetos.
conseguimos definir uma entidade pessoa e imprimir um objeto dessa entidade.

``` js
class Person {

// O constructor é sempre executado como instaciamos nossa classe, seria meio que tudo que está nele seria meio que parametros obrigatorios

    constructor(firstName, lastName, age) {
        this.firstName = firstName;
        this.lastName = lastName;
        this.age = age;
    }
}
  
// Para instanciar
const person = new Person("Pedro", "Colombo", 23)

console.log(person)

```

# Métodos

Podemos criar metodos para essa classe

``` js

class Person {

    constructor(firstName, lastName, age) {
        this.firstName = firstName;
        this.lastName = lastName;
        this.age = age;
    }
  

    // Para criarmos os metodos ( funcoes da classe)
    getFullName() {
        console.log(`${this.firstName} ${this.lastName}`)
    }

    speak() {
        console.log("Bom dia")
    }

}

// Para instanciar
const person = new Person("Pedro", "Colombo", 23)

// Criamos entao o metodo que junta o first name e o last name

person.getFullName()
person.speak()
console.log(person)

```

# Criando Métodos Estáticos

São metodos que não necessitam que as classes seja instanciada para ser executados exemplo 

``` js

    speak() {

        console.log("Bom dia")

    }

```

pode ser estatico, porque ele não usa nenhum dado da pessoa, diferente desse que usa o firstName e o lastName e ai a classe vai precisar ser instanciada.

``` js

    getFullName() {
        console.log(`${this.firstName} ${this.lastName}`)
    }

```

para transformamos em estatico

``` js

class Person {

  

    constructor(firstName, lastName, age) {

        this.firstName = firstName;

        this.lastName = lastName;

        this.age = age;

    }

  

    static speak() {

        console.log("Bom dia")

    }

}

  

Person.speak()

  

// como é estatico nao acessamos os dados da Classe Person, porque é estatico

```

# Heranças

Conseguimos herdar determinada classe em uma nova classe

``` js

class Animal {

  

    constructor(name){

        this.name = name

    }

  

    speak(){

        console.log(`${this.name} made som noise!`)

    }

}

  
  

// Queremos agora deixar isso mais especifico, vamos criar uma nova classe que extenda esse animal, porque todo dog é um animal, todos podem herdar

// dessa classe

  

class Dog extends Animal {

    constructor(name){

        // fazemos esse super para chamar o constructor de quem estamos extendendo que seria da classe animal

        super(name)

    }

}

  
  

const animal = new Animal('Simba');

const dog = new Dog('Bobby');

  

animal.speak()

dog.speak

```

porque quando extendemos uma classe, a classe que extende tem acesso a todos os metodos que a classe pai tem, o dog tem acesso a tudo que o animal tem.

e podemos sobrescrever ou seja sobrescevr o metodo da classe pai no filho entendeu tipo

``` js

class Animal {

  

    constructor(name){

        this.name = name

    }

  

    speak(){

        console.log(`${this.name} made som noise!`)

    }

}

  
  

// Queremos agora deixar isso mais especifico, vamos criar uma nova classe que extenda esse animal, porque todo dog é um animal, todos podem herdar

// dessa classe

  

class Dog extends Animal {

    constructor(name){

        // fazemos esse super para chamar o constructor de quem estamos extendendo que seria da classe animal

        super(name)

    }

  

    barked() {

        console.log(`Dog ${this.name} barked!`)

    }

}

  
  

const animal = new Animal('Simba');

const dog = new Dog('Bobby');

  

animal.speak()

dog.speak() -> entao aqui vai ser na vrdade o barked e nao o speak entendeu o resultado final

```