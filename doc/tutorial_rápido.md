# Tutorial Rápdo

Planejar
Implementar
Entender o código
Testar


# Tarefa 1📘 Tutorial: Construindo um Front-end + API em Node.js (do zero)

## 🎯 Objetivo do projeto

Criar uma aplicação simples onde:

* O **Front-end (HTML)** possui um formulário com **nome e e-mail**
* O **Back-end (API Node.js)** gerencia usuários (CRUD)
* Tudo organizado seguindo uma **arquitetura clara e didática**

---

**Arquitetura**: 

## 🏗️ Arquitetura escolhida

### 👉 Arquitetura MVC (Model–View–Controller)

Mesmo sendo um projeto simples, vamos usar **MVC**, porque:

* Facilita o aprendizado
* Organiza responsabilidades
* É base para projetos profissionais

### 📦 Como fica o MVC aqui?

| Camada         | Responsabilidade                       |
| -------------- | -------------------------------------- |
| **View**       | HTML (index.html)                      |
| **Controller** | Regras da API (`userController.js`)    |
| **Model**      | Dados simulados (`data.js`)            |
| **Server**     | Configuração do servidor (`server.js`) |


Prompt 1: explique rapidamente a arquitetura escolhida (MVC) e mostre a estrutura de pastas do projeto. 

Estrutura final do projeto:

```
meu-projeto/
│
├── public/
│   └── index.html
│
├── controllers/
│   └── userController.js
│
├── data/
│   └── data.js
│
├── server.js
├── package.json
└── node_modules/
```

**Parte 1 – Front-end**: 

**Criar o front end**
Prompt 1(plan): Crie a pasta public e dentro da pasta public crie o arquivo `index.html`. 
Crie um formulário com **nome e email**

**Inicialize o repositorio git**
Prompt 2(plan):Inicialize o repositório git

**Conectar o formulário à API**
Prompt 3: crie o arquivo `script.js`. Capture o envio do formulário, use `fetch` com método POST para enviar `name` e `email` em JSON para a API e exiba uma mensagem de sucesso ou erro na tela. o servidor rodará na porta http://localhost:3000/api/users

**Conectar o formulário à API**
Prompt 4: No arquivo `index.html` e `script.js`. No script.js, liste os usuários da api, use `fetch` com método Get para listar `name` e `email` em JSON para a API e exiba a lista na tela no arquivo index.html. o servidor rodará na porta http://localhost:3000/api/users

dica: verificar futuramente qual a porta o servidor

**Parte 2 – Back-end (API Node.js)**: 

**Criar o servidor**
Prompt 1: Inicialize o package.json e instale as dependências `express` e `cors`. Configure o `package.json` com o script `"start": "node server.js"`. Configure ES Modules (ESM).Crie o arquivo .gitignore

**Arquivos do projeto**: 
Prompt 2: crie o arquivo `server.js` na raiz do projeto e crie a pasta src e dentro da pasta src crie os arquivos `controllers/userController.js` e `data/data.js`. Não crie o código dentro das pastas userController.js e data.js`

**Simular o banco de dados em memória**: 
Prompt 3: crie no arquivo `data.js` uma lista (array) de usuários (users) com os campos id, name e email. 

**server.js – configuração do servidor**: 
Prompt 3:crie o servidor express dentro do arquivo server.js. importe `express`, `cors`. Instancie o app. Defina `HOST` e `PORT`. Configure os middlewares `cors`, `express.json()` e `express.static('public')`.

dica: rode a aplicação no terminal: node server.js ou npm run start
para para a aplicação:: ctrl+c

**server.js – HTML**: 
Prompt 4 (opicional se não já criou): sirva o arquivo `index.html` usando `res.sendFile` e finalize iniciando o servidor com `app.listen`.

**server.js – rotas da API**: 

Prompt 5: crie a rota GET no arquivo server.js
GET `/api/users`.

**userController.js**: 
Prompt 6: implemente somente a função `getAllUsers` no arquivo userController.js

Prompt 7: No arquivo server.js, inport a a função `getAllUsers userController.js` e ajuste a rota GET `/api/users` para chama-lá.


Continuando:

**Crie as rotas da api**

Prompt :crie as rotas no arquivo server.js
GET `/api/users`,
GET `/api/users/:id`,
POST `/api/users`,
PUT `/api/users/:id`,
DELETE `/api/users/:id`,


**userController.js**: 
Prompt: implemente as funções `getAllUsers`, `getUserByID`, `createUser`, `updateUser` e `deleteUser`, com explicação simples do fluxo no arquivo userController.js


