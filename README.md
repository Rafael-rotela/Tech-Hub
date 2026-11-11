# Tech-Hub

> Um e-commerce completo de produtos de tecnologia, construído com **React + Vite** no front-end, **Next.js** no back-end e **MySQL + Prisma** na camada de dados.

---

## 💻 Sobre o Projeto

O **Tech-Hub** é uma plataforma de e-commerce moderna criada para simular a experiência real de compra e venda de eletrônicos e produtos de tecnologia. O projeto tem como objetivo consolidar conhecimentos em desenvolvimento full stack com JavaScript/TypeScript, abordando desde a construção de interfaces reativas até a modelagem de banco de dados e a criação de APIs.

### 🌟 Funcionalidades Principais

- 🛒 **Carrinho de Compras:** adicionar, remover e atualizar a quantidade de produtos em tempo real.
- 🔍 **Filtro de Produtos:** busca por categorias, preços e especificações técnicas.
- 👤 **Autenticação de Usuários:** cadastro, login e área do cliente.
- 📦 **Gestão de Produtos e Pedidos:** catálogo, estoque e histórico de pedidos persistidos no banco.
- 💳 **Simulação de Checkout:** fluxo completo de finalização de pedido de ponta a ponta.
- 📱 **Design Responsivo:** interface otimizada para computadores, tablets e celulares.

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia |
| --- | --- |
| **Front-end** | [React](https://react.dev) + [Vite](https://vite.dev) |
| **Back-end / API** | [Next.js](https://nextjs.org) (Route Handlers) |
| **Banco de Dados** | [MySQL](https://www.mysql.com) |
| **ORM** | [Prisma](https://www.prisma.io) |
| **Ambiente / Ferramentas** | [Node.js](https://nodejs.org), npm, Git |

## 📁 Estrutura do Projeto

```
Tech-Hub/
├── frontend/          # Aplicação React + Vite (interface da loja)
│   ├── src/
│   └── package.json
├── backend/           # Aplicação Next.js (API do e-commerce)
│   ├── app/api/       # Rotas da API
│   ├── prisma/
│   │   └── schema.prisma
│   └── package.json
└── README.md
```

## ⚙️ Como Rodar o Projeto

### 📋 Pré-requisitos

Antes de começar, você vai precisar ter instalado:

- [Git](https://git-scm.com)
- [Node.js](https://nodejs.org) (versão 20 ou superior) e npm
- [MySQL](https://dev.mysql.com/downloads/) (versão 8 ou superior) rodando localmente ou em um servidor acessível

### 🚀 Passos para Execução

```bash
# 1. Clone este repositório
git clone https://github.com/Rafael-rotela/Tech-Hub.git

# 2. Acesse a pasta do projeto
cd Tech-Hub
```

#### 🗄️ Back-end (Next.js + Prisma)

```bash
# 3. Acesse a pasta do back-end e instale as dependências
cd backend
npm install

# 4. Crie o arquivo de variáveis de ambiente
cp .env.example .env
```

Configure a conexão com o MySQL no arquivo `.env`:

```env
DATABASE_URL="mysql://USUARIO:SENHA@localhost:3306/techhub"
```

```bash
# 5. Gere o Prisma Client e aplique as migrations no banco
npx prisma generate
npx prisma migrate dev

# 6. Inicie o servidor do back-end (http://localhost:3000)
npm run dev
```

#### 🎨 Front-end (React + Vite)

Em outro terminal:

```bash
# 7. Acesse a pasta do front-end e instale as dependências
cd frontend
npm install

# 8. Crie o arquivo de variáveis de ambiente
cp .env.example .env
```

Configure a URL da API no arquivo `.env`:

```env
VITE_API_URL="http://localhost:3000/api"
```

```bash
# 9. Inicie o front-end (http://localhost:5173)
npm run dev
```

### 🧰 Comandos Úteis do Prisma

```bash
npx prisma studio            # Interface visual para explorar o banco
npx prisma migrate dev       # Cria e aplica uma nova migration
npx prisma db seed           # Popula o banco com dados iniciais (se configurado)
```

## 🧑‍💻 Autores

**Rafael**
- **LinkedIn:** [Rafael Rotela](https://www.linkedin.com/in/rafael-rotela-0986b1356/)
- **E-mail:** [rjvrafael22@gmail.com](mailto:rjvrafael22@gmail.com)
- **GitHub:** [@Rafael-rotela](https://github.com/Rafael-rotela)

**Gih**
- **LinkedIn:** [Acesse meu perfil](https://linkedin.com)
- **E-mail:** [seu.email@exemplo.com](mailto:seu.email@exemplo.com)
- **GitHub:** [@seu-usuario](https://github.com)

## 📄 Licença

Este projeto está sob a licença descrita no arquivo [LICENSE](LICENSE).
