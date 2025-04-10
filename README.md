# Projeto Full Stack Week 💻

Este é o repositório oficial do e-commerce desenvolvido durante a Full Stack Week, um evento diferente de tudo que você já viu, com 4 lives de muito conteúdo. Nosso objetivo principal é criar um projeto altamente relevante, utilizando as tecnologias mais modernas e demandadas pelo mercado, a fim de adicionar autoridade ao currículo de desenvolvedor.

## Tecnologias Utilizadas 🚀

- **React**: Uma biblioteca JavaScript popular para construir interfaces de usuário interativas.

- **Next.js 13**: Um framework React que oferece renderização do lado do servidor (SSR), geração estática (SSG), entre muitos outros recursos.

- **Next Auth**: Biblioteca para autenticação de usuários com OAuth.

- **Postgres**: Um sistema de gerenciamento de banco de dados relacional.

- **Prisma**: Um ORM (Object-Relational Mapping) para Node.js e TypeScript.

- **shadcn/ui**: Uma biblioteca de componentes de IU reutilizáveis e estilizáveis.

- **Tailwind CSS**: Um framework CSS que oferece várias classes para utilização já pré-estilizadas.

- **API do Stripe**: Uma API de pagamento popular para processar pagamentos online de forma segura.

## Funcionalidades 📦

- **Login com o Google**: Permitimos que os usuários façam login usando suas contas do Google para uma experiência de autenticação simplificada.

- **Navegação por Categorias**: Os usuários podem explorar produtos por categorias, facilitando a busca e a compra.

- **Descontos em Produtos**: Alguns produtos podem ter descontos especiais, permitindo aos usuários economizar em suas compras.

- **Gerenciamento do Carrinho de Compras**: Os usuários podem adicionar produtos ao seu carrinho de compras, remover produtos e também modificar a quantidade de um produto no carrinho de compras conforme necessário.

- **Pagamento do Pedido com a API do Stripe**: Oferecemos uma experiência segura de pagamento online com a integração da API do Stripe, incluindo o uso de webhooks para processar eventos relacionados ao pagamento. Os usuários podem concluir seus pedidos com facilidade e segurança.

## Protótipo no Figma 🎨

Você pode visualizar o protótipo do nosso projeto no Figma. Ele oferece uma prévia visual de como a interface do usuário é projetada e como as diferentes funcionalidades são organizadas. Confira o protótipo [aqui](https://www.figma.com/proto/8VmwuO1vnKChtYwgOrOeHQ/File-System-Web-Store?node-id=344-100&p=f&t=Buo4xHi9yFvISpw1-0&scaling=min-zoom&content-scaling=fixed&page-id=344%3A99).

Fique à vontade para explorar e compartilhar suas opiniões sobre o design do projeto!

## Como Rodar o Projeto Localmente 🖥️

Siga os passos abaixo para configurar e executar o projeto em sua máquina local:

### Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas:

- **Node.js** (versão 18 ou superior)
- **npm** ou **yarn**
- **Docker** e **Docker Compose** (opcional, mas recomendado para rodar o banco de dados)
- **PostgreSQL** (caso não utilize Docker)

### Passo a Passo

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/viniciusmilk/fsw-store.git
   cd fsw-store
   ```

2. **Copie o arquivo de exemplo de variáveis de ambiente:**

   ```bash
   cp .env.example .env
   ```

3. **Instale as dependências:**

   ```bash
   npm install
   ```

4. **Suba os containers do Docker:**

   ```bash
   docker compose up -d
   ```

5. **Execute as migrações do Prisma:**
    #### Certifique-se de que a variável de ambiente DATABASE_URL no arquivo .env tenha o seguinte valor DATABASE_URL="postgresql://postgres:password@localhost:5432/app"

   ```bash
   npx prisma migrate dev
   ```

6. **Execute o seed do banco de dados:**

   ```bash
   npx prisma db seed
   ```

7. **Inicie o servidor de desenvolvimento:**

   ```bash
   npm run dev
   ```


## Contribuições e Colaborações 🤝

Este projeto está totalmente aberto a contribuições. Se você deseja colaborar, fique à vontade para criar pull requests, corrigir bugs, adicionar novos recursos ou aprimorar a documentação. Sua contribuição é valiosa e ajuda a melhorar ainda mais este projeto!

### Como Contribuir

1. Faça um fork deste repositório.

2. Crie uma branch para sua contribuição:

```bash
    git checkout -b minha-contribuicao
```

3. Faça suas alterações e adicione commits descritivos (seguindo o Conventional Commits, preferencialmente).

4. Crie um pull request para a branch `main` deste repositório.

5. Envie suas alterações para o seu repositório forkado:

```bash
    git push origin minha-contribuicao
```
