# NLW Agents

Este projeto é um backend desenvolvido durante o evento NLW da Rocketseat.

## Tecnologias e Bibliotecas Utilizadas
- **Node.js** com **TypeScript**
- **Fastify**: Framework web para Node.js, focado em performance
- **fastify-type-provider-zod**: Integração de validação de tipos com Zod
- **@fastify/cors**: Middleware para habilitar CORS
- **Drizzle ORM**: ORM para manipulação de banco de dados
- **Docker**: Para orquestração de containers e ambiente de banco de dados

## Padrões de Projeto
- Estrutura modular de rotas (cada rota em um arquivo separado)
- Separação de responsabilidades (rotas, banco de dados, configuração de ambiente)
- Uso de validação de dados com Zod

## Setup e Configuração

1. **Clone o repositório:**
   ```bash
   git clone <url-do-repo>
   cd server
   ```

2. **Instale as dependências:**
   ```bash
   npm install
   ```

3. **Configure as variáveis de ambiente:**
   - Edite o arquivo `.env` conforme necessário (veja o exemplo em `src/env.ts`).

4. **Suba o banco de dados com Docker:**
   ```bash
   docker-compose up -d
   ```

5. **Execute as migrations e seeds:**
   ```bash
   npm run db:migrate
   npm run db:seed
   ```

6. **Inicie o servidor:**
   ```bash
   npm run dev
   ```

O servidor estará disponível em `http://localhost:<PORTA>`.

---

Projeto desenvolvido durante o evento NLW da Rocketseat.
