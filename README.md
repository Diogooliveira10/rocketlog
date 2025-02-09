# API de Entregas 📦

Uma API desenvolvida em Node.js para gerenciar pedidos e entregas, permitindo que vendedores enviem pedidos para clientes e acompanhem o status das entregas.

## 📌 Funcionalidades

- Cadastro e autenticação de usuários com diferentes perfis: `sale` (vendedor) e `customer` (cliente).
- Gerenciamento de pedidos, vinculando cada entrega a um usuário.
- Controle de status das entregas: `processing`, `shipped` e `delivered`.
- Registro de movimentações de entrega (exemplo: "Produto saiu para entrega").
- Validação de dados para maior segurança e consistência.
- Testes automatizados para garantir confiabilidade da API.

## 🚀 Tecnologias Utilizadas

- **Node.js**
- **Express** - Framework minimalista para criação de APIs.
- **TypeScript** - Tipagem estática para maior segurança no desenvolvimento.
- **Docker** - Containerização do ambiente.
- **PostgreSQL** - Banco de dados relacional.
- **Prisma** - ORM moderno para facilitar manipulação do banco de dados.
- **Zod** - Validação de dados.
- **bcrypt** - Criptografia de senhas.
- **Jest & Supertest** - Testes automatizados para endpoints.
- **Insomnia** - Testes manuais da API.
- **Beekeeper Studio** - Gerenciamento do banco de dados.

## 🛠️ Como Executar o Projeto

### Pré-requisitos
Antes de começar, você precisará ter instalado em sua máquina:
- **Docker**
- **Node.js**
- **npm** ou **yarn**

### Passos para rodar o projeto

1. Clone o repositório:
   ```sh
   git clone https://github.com/Diogooliveira10/rocketlog.git
   ```
2. Acesse a pasta do projeto:
   ```sh
   cd nome-do-projeto
   ```
3. Instale as dependências:
   ```sh
   npm install  # ou yarn install
   ```
4. Suba os containers Docker:
   ```sh
   docker-compose up -d
   ```
5. Rode as migrações do banco de dados:
   ```sh
   npx prisma migrate dev
   ```
6. Inicie o servidor:
   ```sh
   npm run dev  # ou yarn dev
   ```

## 🧪 Rodando os Testes

Para rodar os testes automatizados, utilize o seguinte comando:
```sh
npm run test:dev
```
