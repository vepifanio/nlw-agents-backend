# NLW Agents

Este projeto foi desenvolvido durante o evento NLW da Rocketseat.

## Descrição

O NLW Agents é um servidor Node.js construído com TypeScript, utilizando Drizzle ORM para manipulação de banco de dados e Docker para facilitar o setup do ambiente.

## Principais Tecnologias e Bibliotecas

- **Node.js**
- **TypeScript**
- **Drizzle ORM**
- **Docker**
- **Zod** (validação de dados)
- **Fastify** (servidor HTTP)

## Padrões de Projeto

- Estrutura modular de pastas (`src/db`, `src/http/routes`, etc)
- Separação de responsabilidades (rotas, schema, conexão com banco)
- Uso de variáveis de ambiente para configuração

## Setup e Configuração

1. **Clone o repositório:**

   ```sh
   git clone <url-do-repo>
   cd server
   ```

2. **Copie o arquivo de variáveis de ambiente:**

   ```sh
   cp .env.example .env
   # Edite o .env conforme necessário
   ```

3. **Suba o banco de dados com Docker:**

   ```sh
   docker-compose up -d
   ```

4. **Instale as dependências:**

   ```sh
   npm install
   ```

5. **Rode as migrations e seeds:**

   ```sh
   npx drizzle-kit migrate
   npm run db:seed
   ```

6. **Inicie o servidor em desenvolvimento:**

   ```sh
   npm run dev
   ```

   **Ou em produção:**

   ```sh
   npm start
   ```

---

Projeto desenvolvido durante o NLW da Rocketseat.
