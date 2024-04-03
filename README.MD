# Gerenciador de Tarefas

Este é um aplicativo para gerenciamento de tarefas desenvolvido em TypeScript com Express e MySQL.

## Funcionalidades

- Cadastro de usuários
- Criação, atualização, listagem e exclusão de tarefas
- Criação, atualização, listagem e exclusão de categorias
- Funcionalidades adicionais utilizando métodos de array

## Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/NathanLisandro/CRUDtypescript.git


## Uso

- Certifique-se de ter o servidor em execução após a instalação.
- Use uma ferramenta como Postman ou Insomnia para enviar requisições HTTP para as rotas fornecidas.

## Rotas

### Usuários

- **POST /api/users**: Cria um novo usuário.
- **GET /api/users/:id**: Retorna detalhes de um usuário específico.
- **PUT /api/users/:id**: Atualiza um usuário existente.
- **DELETE /api/users/:id**: Exclui um usuário.

### Tarefas

- **POST /api/tasks**: Cria uma nova tarefa.
- **GET /api/tasks/user/:userId**: Lista todas as tarefas de um usuário.
- **GET /api/tasks/:id**: Retorna detalhes de uma tarefa específica.
- **PUT /api/tasks/:id**: Atualiza uma tarefa existente.
- **DELETE /api/tasks/:id**: Exclui uma tarefa.

### Categorias

- **POST /api/categories**: Cria uma nova categoria.
- **GET /api/categories/user/:userId**: Lista todas as categorias de um usuário.
- **GET /api/categories/:id**: Retorna detalhes de uma categoria específica.
- **PUT /api/categories/:id**: Atualiza uma categoria existente.
- **DELETE /api/categories/:id**: Exclui uma categoria.

## Funcionalidades Adicionais

- **GET /api/tasks/category/:categoryId?userId=:userId**: Filtra tarefas por categoria.
- **GET /api/tasks/completed?userId=:userId**: Lista tarefas concluídas.
- **GET /api/tasks/pending?userId=:userId**: Lista tarefas pendentes.
- **GET /api/tasks/due/:startDate/:endDate?userId=:userId**: Lista tarefas que vencem em um determinado período.
- **GET /api/tasks/count/:userId**: Conta o número total de tarefas de um usuário.
- **GET /api/tasks/latest/:userId**: Retorna a tarefa mais recente de um usuário.
- **GET /api/tasks/average-completion?userId=:userId**: Calcula a média de conclusão das tarefas.
- **GET /api/tasks/longest-description?userId=:userId**: Retorna a tarefa com a descrição mais longa.
- **GET /api/tasks/grouped-by-category?userId=:userId**: Agrupa tarefas por categoria.
- **GET /api/tasks/oldest/:userId**: Retorna a tarefa mais antiga de um usuário.

## Tecnologias Utilizadas

- Node.js
- Express.js
- MySQL
- TypeScript



