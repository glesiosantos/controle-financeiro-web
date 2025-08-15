💰 Gerenciador de Finanças Pessoais

Um sistema fullstack para controle de finanças pessoais, desenvolvido com NestJS + GraphQL no backend e Vue 3 + Apollo Client no frontend.
Ideal para acompanhar receitas, despesas, saldo e gerar relatórios mensais de forma simples e visual.

✨ Funcionalidades
Funcionalidade	Descrição
👤 Criar Conta	Cadastro de usuários com autenticação via JWT
💵 Criar Lançamentos	Adicionar receitas ou despesas
🏦 Gerenciar Contas	Conta corrente, cartão de crédito, etc
🗂 Categorias	Classificação de lançamentos
📅 Listagem do Mês	Exibir movimentações do período
🔍 Filtros	Pesquisa por tipo, categoria ou conta
💲 Saldo Diário e Mensal	Resumo rápido da situação financeira
📊 Relatórios Gráficos	Análise visual das finanças
🛠 Tecnologias Utilizadas
Backend

NestJS

GraphQL

TypeORM

PostgreSQL

JWT (Autenticação)

BCrypt (Criptografia de senhas)

Moment.js (Manipulação de datas)

Frontend

Vue.js 3

Apollo Client (Integração GraphQL)

Tailwind CSS

Vite

Pinia (Gerenciamento de estado)

📐 Arquitetura do Projeto
flowchart LR
    subgraph Frontend [Frontend - Vue 3 + Tailwind + Apollo]
        UI[Interface de Usuário]
        Pinia[Gerenciamento de Estado]
        Apollo[Apollo Client]
    end

    subgraph Backend [Backend - NestJS + GraphQL]
        Auth[JWT Auth Service]
        Services[Services]
        TypeORM[TypeORM Models]
        DB[(PostgreSQL)]
    end

    UI --> Pinia
    Pinia --> Apollo
    Apollo --> Backend
    Backend --> Auth
    Backend --> Services
    Services --> TypeORM
    TypeORM --> DB

📡 Exemplo de Queries & Mutations (GraphQL)
Criar usuário
mutation {
  createUser(input: {
    name: "João Silva",
    email: "joao@email.com",
    password: "123456"
  }) {
    id
    name
    email
  }
}

Criar lançamento
mutation {
  createLancamento(input: {
    tipo: "DESPESA",
    valor: 150.75,
    descricao: "Supermercado",
    contaId: 1,
    categoriaId: 2
  }) {
    id
    descricao
    valor
    data
  }
}

Listar lançamentos do mês
query {
  lancamentosDoMes(mes: 8, ano: 2025) {
    descricao
    valor
    tipo
    data
  }
}

📦 Como Executar o Projeto
Pré-requisitos

Node.js instalado

PostgreSQL configurado

Yarn ou NPM

<details> <summary>📜 Backend</summary>
# Clone o repositório
git clone https://github.com/seuusuario/gerenciador-financas.git

# Acesse o backend
cd gerenciador-financas/backend

# Instale as dependências
yarn install

# Configure as variáveis de ambiente
cp .env.example .env

# Execute as migrations
yarn typeorm migration:run

# Inicie o servidor
yarn start:dev

</details> <details> <summary>💻 Frontend</summary>
# Acesse o frontend
cd ../frontend

# Instale as dependências
yarn install

# Inicie o projeto
yarn dev

</details>
📸 Screenshots

(adicione imagens reais da aplicação aqui)

📜 Licença

Este projeto está licenciado sob a licença MIT.