# N2_Lingugem_programação_3_JS

Atividade avaliativa da disciplina de Linguagem de programação 3.
Para essa atividade utilizei como banco de dados MongoDB Atlas e o envio das requisições foi feito via Postman.
 
### O ambiente:
* Na configuração foi preciso utilizar o link da cluster usuario e senha (arquivo .env do projeto).
* A inicialização do código, é preciso realizar o download, executar a pasta via VS Code e dentro do VS Code abrir o terminal e digitar "npm install", comando utilizado na instalação de todas as dependencias (nodemon, dotenv, express, mongoose).
* Após a instalação utilize "npm start" para iniciar a execução do app.js.
 
Tendo o servidor rodando, utilize o Postman para fazer as requisições para a API utilizando a URL http://localhost:3000/

### Requisições: 
#### Usuario:
http://localhost:3000/users


* Listar usuário - GET - http://localhost:3000/users 
* para procurar um usuario por nome - GET - http://localhost:3000/users/<nome>
* criação de usuario - POST - http://localhost:3000/users 
* deletar usuario via id - DELETE - http://localhost:3000/users/<id>

#### Sala:
http://localhost:3000/rooms

* Listar salas - GET - http://localhost:3000/rooms
* para procurar sala via ID  - GET - http://localhost:3000/rooms/<id>
* para criar uma nova sala - POST - http://localhost:3000/rooms
* para alterar uma sala existente por id - PATCH - http://localhost:3000/rooms/<id>

Para criação ou modificação das classes, tem que colocar as informações da classe no corpo da requisição como arquivo JSON segue os exemplos a baixo:
 
 {
 
    "nome" : "Nome",
    "sobrenome" : "sobrenome"
 
}
 
 {
 
    "nome" : "sala102",
    "lotacao" : 200
 
}
