# Catálogo de Pokemons
                              
Esse é um projeto FullStack (backend e frontend) onde acessamos APIs públicas de [Pokemon](https://pokeapi.co/) e também do [GitHub](https://docs.github.com/pt/rest/overview/resources-in-the-rest-api). 

## Preview do Projeto
![Recording 2022-11-09 at 14 16 50](https://user-images.githubusercontent.com/106412675/200897047-d0f6a81b-926d-47aa-b733-d9416e418435.gif)

## Tecnologias
### Frontend
 - HTML
 - Javascript
 - XMLHttpRequest
 - CSS
 - Integração com APIs
 
### Backend C#
 - .Net
 - H2
 
### Backend Java
 - Spring
 - H2
 - Swagger Open API
 - JPA
 - Feign Client

## C# Backend Tasks
### 1 - Busca pokemons páginados
- GET /api/v1/pokemons?page=1
- Response - 200 OK
```
{
  qtd: 1154,
  pagina: 1,
  temProx: true,
  pokemons: [
    {
      name: "Nome do Pokemon",
      img: "https://pokeapi.co/api/v2/linkdafotodopokemon/"
    }
  ]
}
```

### 2 - Busca pokemon por nome
- GET /api/v1/pokemons/nome/{nomeDoPokemon}
- Response - 200 OK
```
{
  name: "Nome do Pokemon",
  img: "https://pokeapi.co/api/v2/linkdafotodopokemon/"
}
```
- Response - 404 NOT FOUND

### 3 - Salva Pokemon
- POST /api/v1/pokemons
```
{
  name: "Nome do Pokemon",
  img: "https://pokeapi.co/api/v2/linkdafotodopokemon/"
}
```
- Response - 201 CREATED
- Response - 400 BAD REQUEST

## Java Backend Tasks
### 1 - Busca usuários cadastrados
- GET /api/v1/usuarios
- Response - 200 OK
```
 [
  {
    name: "Nome do Usuario",
    img: "https://pokeapi.co/api/v2/linkdafotodopokemon/",
    nickname: "Ladgelson",
    email: "email@gmail.com",
    pokemonsQueEleGosta: [
      "PIKACHU",
      "DITTO"
    ]
  }
]
```
