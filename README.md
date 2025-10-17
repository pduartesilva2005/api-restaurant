# API Restaurant

Uma API RESTful para gerenciamento de pedidos em restaurantes desenvolvida com Node.js, Express e SQLite.

## 📋 Funcionalidades

- Cadastro e gerenciamento de produtos
- Controle de mesas
- Abertura e fechamento de sessões de mesa
- Registro de pedidos
- Cálculo do total da conta

## 🛠️ Tecnologias

- [Node.js](https://nodejs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/)
- [Knex.js](https://knexjs.org/)
- [SQLite](https://www.sqlite.org/)
- [Zod](https://zod.dev/)

## 📦 Instalação

```bash
# Clone o repositório
git clone <https://github.com/pduartesilva2005/api-restaurant.git>

# Acesse a pasta do projeto
cd api-restaurant

# Instale as dependências
npm install

# Execute as migrations
npm run knex migrate:latest

# Execute os seeds
npm run knex seed:run

# Inicie o servidor
npm run dev

```

## 🚀 Rotas da API

### Produtos

- `GET /products` - Lista todos os produtos
- `POST /products` - Cadastra um novo produto
- `PUT /products/:id` - Atualiza um produto
- `DELETE /products/:id` - Remove um produto

### Mesas

- `GET /tables` - Lista todas as mesas

### Sessões de Mesa

- `GET /tables-sessions` - Lista todas as sessões
- `POST /tables-sessions` - Abre uma nova sessão
- `PATCH /tables-sessions/:id` - Fecha uma sessão

### Pedidos

- `POST /orders` - Registra um novo pedido
- `GET /orders/table-session/:table_session_id` - Lista pedidos de uma sessão
- `GET /orders/table-session/:table_session_id/total` - Mostra o total da conta

## ✍️ Autor

Pedro Duarte
