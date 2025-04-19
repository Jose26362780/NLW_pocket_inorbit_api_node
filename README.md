
# 📊 NLW Pocket JS API |  in Orbit | 

Uma API de controle de metas semanais desenvolvido durante um evento de programação da rocketseat, construída com **Node.js**, **Fastify**, **Drizzle ORM** e **PostgreSQL**. Ideal para acompanhar a criação, conclusão e progresso de metas ao longo das semanas.

## 🚀 Tecnologias Utilizadas
 
 - ![Zod](https://img.shields.io/badge/zod-000643?style=for-the-badge&logo=zod&logoColor=white)
 - ![Biome](https://img.shields.io/badge/Biome-000320?style=for-the-badge&logo=Biome&logoColor=blue)
 - ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
 - ![Fastify](https://img.shields.io/badge/fastify-345?style=for-the-badge&logo=Fastify&logoColor=white)
 - ![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
 - ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
 - ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
 - ![Drizzle ORM](https://img.shields.io/badge/Drizzle_ORM-123?style=for-the-badge&logo=drizzle&logoColor=green)


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
git clone https://github.com/Jose26362780/NLW_pocket_inorbit_api_node
cd seu-repo
```

2. **Instale as dependências:**

```bash
npm install
```

3. **Configure o banco de dados:**

Crie um arquivo `.env` com as variáveis necessárias:

```
DATABASE_URL="postgresql://docker:docker@localhost:5432/inorbit"
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


## 🔗 Deploy 

![github](https://img.shields.io/badge/github-000000?style=for-the-badge&logo=github&logoColor=white)
![netlify](https://img.shields.io/badge/vercel-023?style=for-the-badge&logo=vercel&logoColor=white)



## 💻 Sobre mim 😄
 Entusiasta da programação e estudante de Engenharia de Software com foco em        desenvolvimento front-end rumo ao full stack. Dedicado a criar experiências digitais inovadoras que impactam o mundo através da tecnologia.

## 🔗 Contato 

[![linkedin](https://img.shields.io/badge/Linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jose-martinez-352032222/)
[![gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](https://mailto:juniorjose1925@gmail.com)
[![portfolio](https://img.shields.io/badge/Jose.Dev-0A0A03?style=for-the-badge&logo=react&logoColor=whit)](https://my-portfolio-jose-martinez.netlify.app/)


## 📄 Licença

Este projeto está sob a licença MIT.






