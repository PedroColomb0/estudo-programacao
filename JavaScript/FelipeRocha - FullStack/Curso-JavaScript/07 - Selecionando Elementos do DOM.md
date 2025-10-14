
Seleção de elementos do DOM

# Dom 
Basicamente é nosso site.

Html, Body, Dentro do Body temos as tags, ai conseguimos selecionar tudo dentro do Dom

Podemos Selecionar pelo ID

exemplo

``` html
	<h1 id="add-user">Add User</h1>
```

e no JavaScript

``` js

 const addUserText = document.getElementById('add-user')
 console.log(addUserText)
 
```

ai vai retornar no console

``` html
	<h1 id="add-user">Add User</h1>
```


podemos alterar ele o elemento.


``` js
	addUserText.innerText = "Adicionar o usuário"
```


# QuerySelector

Podemos utilizar ele também para selecionar, podemoser selecionar tanto classe como id

para id colocamos #add-user o jogo da velha.

