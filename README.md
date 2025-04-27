# 🍕 pizza.shop API

Aplicativo de entrega de comida (similar ao iFood/Uber Eats) back-end construído com TypeScript, Drizzle e ElysiaJS.

> 🔥 Este projeto tem como objetivo ser agnóstico em relação ao runtime, o que significa que ele deve funcionar no Bun, Node, Cloudflare Workers ou qualquer runtime compatível com a API padrão da Web.

## Executando

Este projeto depende do Docker para configurar o banco de dados. Com o Docker instalado, clone o projeto, instale as dependências, configure os containers do Docker e execute a aplicação.

> Você também deve executar as migrações para criar as tabelas do banco de dados e rodar o seed para popular o banco de dados com dados fictícios.

```sh
bun i
docker compose up -d
bun migrate
bun seed
bun dev
```

## Funcionalidades

> O **resumo** das funcionalidades está listado abaixo. Todas as funcionalidades possuem testes E2E.

- Deve ser possível registrar um novo restaurante
- Deve ser possível fazer login como gerente de restaurante
- Deve ser possível registrar-se como um novo cliente
- Deve ser possível criar um pedido para o restaurante
- Deve ser possível gerenciar o menu do restaurante
- Deve ser possível gerenciar as avaliações do restaurante
- Deve ser possível deixar uma avaliação
- Deve ser possível gerenciar os pedidos do restaurante
- Deve ser possível atualizar o perfil público do restaurante
- Deve ser possível abrir/fechar o restaurante
- Deve ser possível listar métricas do restaurante