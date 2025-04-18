# 📊 Goal Tracker API

Uma API de controle de metas semanais, construída com **Node.js**, **Fastify**, **Drizzle ORM** e **PostgreSQL**. Ideal para acompanhar a criação, conclusão e progresso de metas ao longo das semanas.

---

## 🚀 Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)
- [Fastify](https://fastify.dev/)
- [Drizzle ORM](https://orm.drizzle.team/)
- [PostgreSQL](https://www.postgresql.org/)
- [Zod](https://zod.dev/) – validação de dados
- [Docker Compose](https://docs.docker.com/compose/) – ambiente de desenvolvimento
- [Biome](https://biomejs.dev/) – formatação e lint de código
- [TypeScript](https://www.typescriptlang.org/)

---

## 🧱 Arquitetura do Projeto

O projeto segue uma arquitetura modular baseada em separação de responsabilidades:

```
src/
├── db/           # Schema e conexão com o banco (Drizzle ORM)
│   ├── index.ts
│   ├── schema.ts
│   └── seed.ts
├── functions/    # Lógica de negócio (use-cases)
│   ├── create-goal.ts
│   ├── create-goal-completion.ts
│   ├── get-week-pending-goals.ts
│   └── get-week-summary.ts
├── http/         # Camada HTTP (rotas e servidor Fastify)
│   ├── routes/
│   ├── server.ts
│   └── env.ts
```

> 📌 Inspirado em **Clean Architecture** simplificada, esse padrão favorece:
> - Escalabilidade
> - Manutenibilidade
> - Testabilidade

---

## 🔧 Como rodar localmente

1. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

2. **Instale as dependências:**

```bash
npm install
```

3. **Configure o banco de dados:**

Crie um arquivo `.env` com as variáveis necessárias:

```
DATABASE_URL=postgres://user:password@localhost:5432/dbname
```

4. **Suba o banco com Docker:**

```bash
docker-compose up -d
```

5. **Rode as migrações e seed (se necessário):**

```bash
npm run db:migrate
npm run db:seed
```

6. **Inicie a aplicação:**

```bash
npm run dev
```

---

## 🛠️ Scripts disponíveis

| Comando             | Descrição                         |
|---------------------|-----------------------------------|
| `npm run dev`       | Inicia o servidor em modo dev     |
| `npm run format`    | Formata o código com Biome        |
| `npm run db:migrate`| Roda as migrações com Drizzle     |
| `npm run db:seed`   | Popula o banco com dados de seed  |

---

## 📫 Contato

Desenvolvido por [Seu Nome].  
Entre em contato via [LinkedIn](https://linkedin.com/in/seu-perfil) ou [seuemail@exemplo.com](mailto:seuemail@exemplo.com)

---

## 📄 Licença

Este projeto está sob a licença MIT.
