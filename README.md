### Cadastro de Usuários com GraphQl e MongoDB

#### Listando os Usuários

```
query {
  users {
  	id
    name
    email
	}
}
```


#### Buscando um único usuário

```
query {
  user(id:"5d3bbbf5f947a52e2ac14c3c") {
    name
    email
  }
}
```

#### Criando Um usuário

```
mutation {
  createUser(name:"João Neto", email: "joao.neto@dev.com") {
    id
  }
}
```


#### Rodando o projeto - localhost:4000

```
npm install
node src/server.js
```