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
- **Render** - Plataforma de deploy para back-end e banco de dados.
- **Tsup** - Biblioteca para conversão de TypeScript para JavaScript.

## 🛠️ Como Executar o Projeto

### Pré-requisitos
Antes de começar, você precisará ter instalado em sua máquina:
- **Docker**
- **Node.js**
- **npm** ou **yarn**

### Passos para rodar o projeto localmente

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

## 🚀 Deploy da Aplicação

A aplicação está configurada para ser implantada utilizando **Render**, uma plataforma de deploy que permite hospedar tanto aplicações back-end quanto bancos de dados.

### Deploy no Render

1. **Build Command**: O Render executa o seguinte comando para compilar a aplicação antes de cada deploy:
   ```sh
   npm install && npm run build && npx prisma migrate deploy
   ```
2. **Start Command**: O Render inicia a aplicação com o seguinte comando:
   ```sh
   npm start
   ```

## 🧪 Rodando os Testes

Para rodar os testes automatizados, utilize o seguinte comando:
```sh
npm run test:dev
```

## 📦 Build da Aplicação

O projeto utiliza **Tsup** para converter TypeScript para JavaScript. O comando de build é:
```sh
npm run build
```
Isso gera a versão final da aplicação pronta para execução em produção.

## 🚀 Executando a Aplicação

Para rodar a aplicação em produção, utilize o comando:
```sh
npm start
```
Isso inicia o servidor para aceitar requisições.

---
