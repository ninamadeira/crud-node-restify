# API Restful com Node.js

API Restful que controla operações crud de contatos.

### Criar uma pasta para projeto
```
Ex.: mkdir node-restify
```

### Entrar na pasta node-nestify
```
cd node-restify
```

### Instalar o nodemon
```
npm install --save-dev nodemon
```
  
### Criar o package.json
```
npm init
```
### Instalar módulos restify, restify-errors, knex e postgres
```
npm i --save restify restify-errors knex pg
```

### Criar o banco de dados db e a tabela contato no postgres
```
CREATE DATABASE db;

CREATE TABLE contato (
	id SERIAL PRIMARY KEY,
	name VARCHAR(256) NOT NULL,
	email VARCHAR(256) NOT NULL
);
O id é do tipo auto-incremento.
```

### Executar aplicação e reiniciar automaticamente a cada mudança
```
nodemon index.js
```

### Testar as rotas e seus respectivo verbos http
```
Insomnia ou Postman

POST: http://localhost:8080/create
{
	"name": "Mara Santos",
	"email": "mara@empresa.com
}

DELETE: http://localhost:8080/delete/1
```
