# CRIANDO UMA CLASSE 



## Parte 1: Criar Função
Prompt 1: Crie um arquivo usuario.js e dentro dele crie uma função(listarUsuarios) que contenha uma lista de usuários com id, nome. Exporte esta função.
Prompt 2: Crie um arquivo index.js e dentro dele importe a função listarUsuarios e exiba a lista de usuário no console.
Execute no terminal:node index.js

Prompt 3: Toque o o module.exports para a sintaxe de export do ES6/ESM (import/export). 

Também preciso atualizar o index.js para usar import em vez de require

## Parte 2: Criar Classe

Prompt 1: Crie um arquivo User.js e dentro dele crie no construtor uma lista de usuários com id, nome e o método(listarUsuarios) para retornar os usuários Exporte esta classe.

Prompt 2: No arquivo index.js e dentro dele importe a classe User, instancie e exiba a lista de usuário no console.
Execute no terminal:node index.js


# Estudo:

### 🔹 Função

* Executa **uma ação específica**
* **Não mantém estado**
* Simples, rápida e fácil de entender
* Ideal para **helpers, utilitários e lógicas pequenas**

👉 *Use quando não precisa guardar dados nem regras complexas.*

---

### 🔹 Classe

* Representa um **conceito com dados + comportamento**
* **Mantém estado interno**
* Organiza regras de negócio
* Escala melhor em sistemas grandes

👉 *Use quando o código cresce e precisa de organização.*

---

### 🧠 Regra de ouro

> **Sem estado → função**
> **Com estado → classe**


Defina:
CommonJS OU ES Modules
Claro, bem direto 👇

### 🔹 CommonJS

* Usa `require` / `module.exports`
* Padrão antigo do Node.js
* Simples e muito usado em projetos legados
* Não precisa configurar `package.json`

👉 **Bom para projetos simples ou antigos**

---

### 🔹 ES Modules (ESM)

* Usa `import` / `export`
* Padrão moderno do JavaScript
* Precisa `"type": "module"` no `package.json`
* Melhor compatibilidade com o futuro

👉 **Bom para projetos novos**


