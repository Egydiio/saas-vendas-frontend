# SaaS Frontend

Aplicação frontend SPA construída com **Vue 3** e **Vite**, integrada a uma API **Laravel** para gerenciamento de lojas online. O sistema permite que usuários criem e personalizem sua própria loja virtual, adicionem produtos e acompanhem pedidos de forma simples e eficiente.

## Funcionalidades

- **Cadastro e Personalização de Lojas**: Usuários podem criar e customizar suas lojas virtuais.
- **Gerenciamento de Produtos**: Adição, edição e exclusão de produtos físicos ou digitais.
- **Acompanhamento de Pedidos**: Visualização e gestão dos pedidos realizados nas lojas.
- **Interface Responsiva**: Layout adaptável a qualquer dispositivo, proporcionando ótima experiência do usuário.
- **Integração Segura**: Comunicação com a API Laravel utilizando autenticação JWT para garantir segurança nas operações.

## Tecnologias Utilizadas

- [Vue 3](https://vuejs.org/) (framework frontend)
- [Vite](https://vitejs.dev/) (ferramenta de build e desenvolvimento)
- [Vue Router](https://router.vuejs.org/) (roteamento SPA)
- [Pinia](https://pinia.vuejs.org/) (gerenciamento de estado)
- [Axios](https://axios-http.com/) (requisições HTTP)
- [Tailwind CSS](https://tailwindcss.com/) (estilização)
- [API Laravel](https://laravel.com/) (backend)

## Requisitos

- Node.js >= 18.x
- npm ou yarn

## Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/Egydiio/saas-vendas-frontend.git
   cd saas-vendas-frontend
   ```

2. Instale as dependências:
   ```bash
   npm install
   # ou
   yarn install
   ```

3. Copie o arquivo de exemplo de ambiente e configure as variáveis:
   ```bash
   cp .env.example .env
   # Edite o .env com a URL da sua API Laravel e outras configurações
   ```

4. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   # ou
   yarn dev
   ```

5. Acesse a aplicação em [http://localhost:5173](http://localhost:5173)

## Autenticação

A autenticação é realizada via JWT fornecido pela API Laravel. Ao efetuar login, a aplicação armazena o token e o utiliza para autenticar as próximas requisições.

### Exemplo de login

```js
// Exemplo de payload para login
{
  email: 'usuario@exemplo.com',
  password: 'senha'
}
```

A resposta conterá o token JWT a ser utilizado nas requisições autenticadas.

## Estrutura das Principais Telas

- **Login/Cadastro**: Autenticação do usuário.
- **Dashboard**: Visão geral das lojas e pedidos.
- **Gerenciamento de Lojas**: Listagem e edição de lojas virtuais.
- **Gerenciamento de Produtos**: Cadastro e listagem de produtos.
- **Pedidos**: Acompanhamento e detalhes dos pedidos recebidos.

##

Projeto desenvolvido por [João Egydio](https://github.com/Egydiio)
