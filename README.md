<div align="center">

# 📝 Blog Pessoal

### Uma aplicação moderna de blog desenvolvida com React, TypeScript e Vite.

[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-6-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vite.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/Licença-Educacional-8B5CF6?style=for-the-badge)](#)

<br />

[![Acessar Projeto](https://img.shields.io/badge/Acessar%20Projeto-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://blogpessoal-react-jcrf.vercel.app/)

<br />

[Funcionalidades](#-funcionalidades)
&nbsp;•&nbsp;
[Tecnologias](#-tecnologias)
&nbsp;•&nbsp;
[Como executar](#-como-executar)
&nbsp;•&nbsp;
[Estrutura](#-estrutura-do-projeto)
&nbsp;•&nbsp;
[Autor](#-autor)

</div>

---

## ✨ Sobre o projeto

O **Blog Pessoal** é uma aplicação frontend que permite a usuários autenticados gerenciar temas e postagens por meio de uma API REST.

O projeto foi desenvolvido para praticar conceitos fundamentais e modernos do ecossistema React, incluindo componentização, tipagem estática com TypeScript, gerenciamento de estado, Context API, roteamento, consumo de APIs e feedback visual para o usuário.

> 💡 Projeto criado para fins de estudo, prática e composição de portfólio em Desenvolvimento Full Stack Java.

## 🌐 Demonstração

Acesse a aplicação publicada:

🔗 **[Projeto Blog Pessoal — Vercel](https://blogpessoal-react-jcrf.vercel.app/)**

---

## 🚀 Funcionalidades

### 🔐 Autenticação

- Login de usuários
- Logout de usuários
- Cadastro de novos usuários
- Controle global de autenticação com Context API
- Uso de token nas requisições protegidas
- Redirecionamento de usuários não autenticados

### 🏷️ Gerenciamento de temas

- Listagem de todos os temas
- Cadastro de temas
- Edição de temas
- Exclusão de temas
- Exibição de carregamento durante requisições
- Notificações de sucesso e erro

### 📚 Gerenciamento de postagens

- Listagem de postagens
- Cadastro de postagens
- Edição de postagens
- Exclusão de postagens
- Associação de uma postagem a um tema
- Exibição do título, texto e tema relacionado

### 🎨 Experiência do usuário

- Interface estilizada e responsiva
- Navegação entre páginas com React Router DOM
- Feedback visual com notificações
- Loaders durante operações assíncronas
- Componentes reutilizáveis
- Tratamento de erros de autenticação e comunicação com a API

---

## 🛠 Tecnologias

<div align="center">

| Tecnologia | Utilização |
| :--- | :--- |
| [React](https://react.dev/) | Criação de interfaces baseadas em componentes |
| [TypeScript](https://www.typescriptlang.org/) | Tipagem estática e maior segurança no código |
| [Vite](https://vite.dev/) | Ambiente de desenvolvimento e geração do build |
| [React Router DOM](https://reactrouter.com/) | Gerenciamento de rotas e navegação |
| [Axios](https://axios-http.com/) | Requisições HTTP para a API REST |
| [Tailwind CSS](https://tailwindcss.com/) | Estilização responsiva da interface |
| [React Toastify](https://fkhadra.github.io/react-toastify/) | Alertas de sucesso, informação e erro |
| [React Spinners](https://www.davidhu.io/react-spinners/) | Indicadores de carregamento |
| [Phosphor Icons](https://phosphoricons.com/) | Biblioteca de ícones |
| [ESLint](https://eslint.org/) | Padronização e análise da qualidade do código |

</div>

---

## 📁 Estrutura do projeto

```text
src/
│
├── assets/             # Imagens e arquivos estáticos
├── components/         # Componentes reutilizáveis
├── contexts/           # Context API e autenticação
├── models/             # Interfaces e tipagens
├── pages/              # Páginas da aplicação
├── services/           # Funções de comunicação com a API
├── utils/              # Utilitários, como ToastAlerta
│
├── App.tsx             # Estrutura principal e rotas
├── App.css             # Estilos da aplicação
├── index.css           # Estilos globais
└── main.tsx            # Ponto de entrada da aplicação
```

---

## ⚙️ Como executar

### Pré-requisitos

Antes de executar o projeto, instale:

- [Node.js](https://nodejs.org/)
- npm
- Git

Verifique a instalação:

```bash
node --version
npm --version
```

### 1. Clone o repositório

```bash
git clone https://github.com/JoelRamalhoF/blogpessoal_react.git
```

### 2. Acesse a pasta do projeto

```bash
cd blogpessoal_react
```

### 3. Instale as dependências

```bash
npm install
```

### 4. Execute em desenvolvimento

```bash
npm run dev
```

Depois, abra a URL exibida pelo Vite no terminal. Normalmente:

```text
http://localhost:5173
```

---

## 📦 Scripts disponíveis

| Comando | Descrição |
| :--- | :--- |
| `npm run dev` | Inicia o servidor local para desenvolvimento |
| `npm run build` | Gera a versão otimizada da aplicação para produção |
| `npm run preview` | Executa uma prévia local do build gerado |
| `npm run lint` | Verifica o código com ESLint |

### Build de produção

Para gerar os arquivos de produção:

```bash
npm run build
```

Os arquivos otimizados são criados em:

```text
dist/
```

Para testar o build localmente:

```bash
npm run preview
```

---

## 🔌 Comunicação com a API

As chamadas para a API REST são centralizadas no diretório:

```text
src/services/
```

A aplicação utiliza Axios para enviar e receber dados do backend.

| Método HTTP | Finalidade |
| :--- | :--- |
| `GET` | Buscar temas, postagens e dados de usuários |
| `POST` | Cadastrar novos usuários, temas e postagens |
| `PUT` | Atualizar temas e postagens |
| `DELETE` | Excluir temas e postagens |

Nas rotas que exigem autenticação, o token do usuário é enviado no cabeçalho da requisição:

```typescript
headers: {
  Authorization: token
}
```

---

## 🔔 Feedback visual

A aplicação utiliza React Toastify, organizado por meio do utilitário `ToastAlerta`, para informar ao usuário o resultado das operações.

Exemplos de feedback:

```text
✓ Usuário autenticado com sucesso!
✓ Usuário desconectado com sucesso!
✓ Tema cadastrado com sucesso!
✓ Tema atualizado com sucesso!
✓ Tema deletado com sucesso!
✓ Postagem cadastrada com sucesso!
✕ Erro ao autenticar o usuário
✕ Erro ao consultar dados da API
```

Durante requisições assíncronas, a interface exibe loaders para indicar que a operação está em andamento.

---

## 🗺️ Próximas melhorias

- [ ] Persistir a autenticação usando `localStorage`
- [ ] Criar componente reutilizável para rotas protegidas
- [ ] Implementar paginação de temas e postagens
- [ ] Adicionar busca e filtros de postagens
- [ ] Criar uma página de perfil mais completa
- [ ] Implementar upload de foto de perfil
- [ ] Adicionar modo escuro
- [ ] Melhorar acessibilidade nos formulários
- [ ] Adicionar testes unitários e de integração
- [ ] Aperfeiçoar o tratamento de erros da API
- [ ] Integrar com backend publicado em produção

---

## 👨‍💻 Autor

<div align="center">

Desenvolvido por **Joel Ramalho Filho**.

[![GitHub](https://img.shields.io/badge/GitHub-JoelRamalhoF-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JoelRamalhoF)

[![Repositório](https://img.shields.io/badge/Repositório-blogpessoal__react-6366F1?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JoelRamalhoF/blogpessoal_react)

<br />

Feito com 💜 usando React, TypeScript e Vite.

</div>

---

<div align="center">

Projeto desenvolvido para fins educacionais e de portfólio.

</div>
