# NLW Agents

Backend em Node.js desenvolvido durante o evento NLW da Rocketseat. Ele fornece uma API para gestão de salas e perguntas com suporte a transcrição de áudio e IA generativa.

## Tecnologias

- **Fastify** como framework HTTP
- **Zod** para validações de entrada
- **Drizzle ORM** com **PostgreSQL** e extensão **pgvector**
- **Google Gemini** para transcrição e geração de respostas
- **TypeScript** executado via Node 20

## Padrões

- Organização em módulos `src/http`, `src/db` e `src/services`
- Rotas escritas como plugins Fastify
- Serviços isolam integrações externas

## Configuração

1. Copie `.env.example` para `.env` e ajuste as variáveis
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Suba o banco com Docker:
   ```bash
   docker-compose up -d
   ```
4. Rode as migrações e (opcional) o seed:
   ```bash
   npm run db:migrate
   npm run db:seed
   ```
5. Inicie o servidor em modo desenvolvimento:
   ```bash
   npm run dev
   ```

A aplicação estará disponível em `http://localhost:3333`.

