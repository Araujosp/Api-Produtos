# 🚀 API de Produtos

API RESTful desenvolvida em **Node.js** para gerenciamento de produtos, com suporte ao upload de imagens, autenticação por JWT e organização modular do código.

O projeto foi desenvolvido com foco em boas práticas de desenvolvimento back-end, separação de responsabilidades e organização da estrutura da aplicação.

## ✨ Funcionalidades

- 📦 **Gerenciamento de produtos:** criação e gerenciamento de produtos por meio de endpoints REST.
- 🖼️ **Upload de imagens:** envio e armazenamento de imagens associadas aos produtos.
- 🔐 **Autenticação JWT:** autenticação baseada em JSON Web Tokens para proteger rotas.
- 🗄️ **Migrations:** controle e versionamento da estrutura do banco de dados.
- 🧩 **Models:** organização das entidades e da interação com os dados.
- ⚙️ **Services:** separação das regras de negócio da aplicação.
- 🛣️ **Rotas e controllers:** organização dos endpoints e do tratamento das requisições.

## 🛠️ Tecnologias

- **Node.js** — ambiente de execução JavaScript.
- **JavaScript** — linguagem utilizada no desenvolvimento.
- **Express** — framework para construção de APIs HTTP, caso utilizado no projeto.
- **JWT** — autenticação e autorização baseada em tokens.
- **Banco de dados relacional** — persistência dos dados.
- **Migrations** — gerenciamento de alterações no esquema do banco de dados.
- **Multer** — processamento de uploads multipart/form-data, caso utilizado no projeto.

## 📁 Organização do projeto

A aplicação utiliza uma estrutura modular para facilitar a manutenção e a evolução do código.

```text
Api-Produtos/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── services/
│   ├── routes/
│   ├── migrations/
│   ├── middlewares/
│   └── ...
├── uploads/
│   └── produtos/
├── .env.example
├── .gitignore
├── package.json
└── README.md
```

*Observação: a estrutura acima é ilustrativa. Ajuste os diretórios conforme os arquivos existentes no projeto.*

## ⚙️ Como executar

### Pré-requisitos

- Node.js instalado.
- npm instalado.
- Banco de dados configurado conforme as dependências do projeto.

### 1. Clone o repositório

```bash
git clone https://github.com/Araujosp/Api-Produtos.git
cd Api-Produtos
```

### 2. Instale as dependências

```bash
npm install
```

### 3. Configure as variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto e configure as variáveis exigidas pela aplicação, como conexão com o banco de dados e chave secreta do JWT.

Consulte o arquivo `.env.example`, caso esteja disponível, para identificar os nomes e os valores necessários.

**Importante:** não compartilhe chaves secretas, senhas ou credenciais no repositório.

### 4. Execute as migrations

Utilize o comando definido no `package.json` para executar as migrations do projeto.

Exemplo, caso exista um script `migrate`:

```bash
npm run migrate
```

### 5. Inicie a API

Utilize o script de inicialização definido no `package.json`. Por exemplo:

```bash
npm start
```

Em ambiente de desenvolvimento, caso exista um script específico:

```bash
npm run dev
```

## 🔐 Autenticação

A API utiliza JWT (JSON Web Token) para autenticação das requisições protegidas.

Após obter um token válido pelo mecanismo de autenticação implementado, envie-o no cabeçalho das requisições protegidas:

```http
Authorization: Bearer SEU_TOKEN
```

## 🖼️ Upload de imagens

A API oferece suporte ao envio de imagens de produtos. O formato da requisição, os tipos de arquivo permitidos, os limites de tamanho e o local de armazenamento dependem da configuração implementada no projeto.

## 🎯 Objetivos do projeto

- Desenvolver habilidades em Node.js e desenvolvimento back-end.
- Construir APIs RESTful organizadas e de fácil manutenção.
- Aplicar autenticação com JWT.
- Implementar upload de arquivos.
- Trabalhar com migrations e persistência de dados.
- Aplicar separação de responsabilidades entre models, services, controllers e rotas.

## 👨‍💻 Autor

**Gabriel Araujo**

- GitHub: [@Araujosp](https://github.com/Araujosp)

---

Desenvolvido para praticar e aprimorar conhecimentos em desenvolvimento back-end com Node.js.
