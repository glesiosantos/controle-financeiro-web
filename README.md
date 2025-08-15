## 💰  Gerenciador de Finanças Pessoais

Um sistema completo para controle financeiro pessoal, permitindo registrar receitas e despesas, organizar contas e categorias, além de visualizar relatórios e gráficos para melhor gestão do seu dinheiro.
Este projeto foi desenvolvido para estudos e composição de portfólio, utilizando tecnologias modernas no backend e frontend.

## 🚀 Funcionalidades - Core

- 👤 Criar Conta – Registro de usuários com autenticação segura.
- 💵 Criar Lançamentos – Adicione receitas ou despesas.
- 🏦 Criar Contas – Ex.: Cartão de Crédito, Cartão de Débito, Conta Corrente.
- 🗂 Criar Categorias – Classifique seus lançamentos.
- 📅 Listar Lançamentos do Mês – Visualize todas as movimentações do período.
- 🔍 Filtrar Lançamentos – Pesquisa por categoria, conta ou tipo.
- 📊 Relatórios Mensais – Exibição de gráficos para melhor análise.
- 💲 Saldo Diário e Mensal – Veja rapidamente como está a sua situação financeira.

## 🛠 Tecnologias Utilizadas - Backend

- NestJS – Framework Node.js para construção de APIs.
- GraphQL – Consulta e manipulação de dados.
- TypeORM – ORM para integração com banco de dados.
- PostgreSQL – Banco de dados relacional.
- JWT – Autenticação baseada em tokens.
- BCrypt – Criptografia de senhas.
- Moment.js – Manipulação de datas.

# Frontend
- Vue.js – Framework JavaScript progressivo.
- Apollo Client – Integração GraphQL no frontend.
- Tailwind CSS – Estilização moderna e responsiva.
- Vite – Build tool rápida e leve.
- Pinia – Gerenciamento de estado.

## 📦 Como Executar o Projeto
Pré-requisitos

Node.js instalado

PostgreSQL configurado

Yarn ou NPM

## Instalando o Backend
```
    # Clone o repositório
    git clone https://github.com/seuusuario/gerenciador-financas.git

    # Acesse a pasta do backend
    cd gerenciador-financas/backend

    # Instale as dependências
    yarn install

    # Configure as variáveis de ambiente (.env)
    cp .env.example .env

    # Execute as migrations
    yarn typeorm migration:run

    # Inicie o servidor
    yarn start:dev
```
## Instalando o Frontend
```
    # Acesse a pasta do frontend
    cd ../frontend

    # Instale as dependências
    yarn install

    # Inicie o projeto
    yarn dev
```
📸 Screenshots (opcional)

Adicione imagens do sistema para deixar o README mais atrativo.

📌 Objetivo do Projeto

Este sistema foi criado com foco em aprendizado e demonstração de habilidades para portfólio, explorando boas práticas de arquitetura, autenticação e integração entre backend e frontend