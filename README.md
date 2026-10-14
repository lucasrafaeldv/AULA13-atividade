<div align="center">

#  Atividade 13 · API de Clientes

API em **Node.js** com **Express** para gerenciar uma base de clientes armazenada em arquivo JSON.

![Node.js](https://img.shields.io/badge/Node.js-18%2B-339933?logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-5-000000?logo=express&logoColor=white)
![License](https://img.shields.io/badge/licença-ISC-blue)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)

</div>

---

##  Índice

- [Sobre o projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias](#-tecnologias)
- [Estrutura do projeto](#-estrutura-do-projeto)
- [Pré-requisitos](#-pré-requisitos)
- [Instalação](#-instalação)
- [Como executar](#-como-executar)
- [Dados](#-dados)
- [Rotas da API](#-rotas-da-api)
- [Scripts disponíveis](#-scripts-disponíveis)
- [Imagens](#-imagens)
- [Melhorias futuras](#-melhorias-futuras)
- [Autor](#-autor)
- [Licença](#-licença)

---

##  Sobre o projeto

Projeto desenvolvido como atividade da **Aula 13**. A aplicação é um servidor web feito com Node.js e Express que trabalha com uma lista de clientes (id, CPF e nome) guardada em um arquivo JSON.

##  Funcionalidades

- Servidor HTTP construído com Express
- Suporte a CORS para aceitar requisições de outras origens
- Dados de clientes armazenados em arquivo JSON
- Modo de desenvolvimento com recarregamento automático

##  Tecnologias

| Tecnologia | Uso |
|------------|-----|
| [Node.js](https://nodejs.org/) | Ambiente de execução JavaScript |
| [Express 5](https://expressjs.com/) | Framework web para criar o servidor e as rotas |
| [CORS](https://www.npmjs.com/package/cors) | Liberação de requisições entre origens diferentes |

##  Estrutura do projeto

```
AULA13-atividade/
├── dados/            # Arquivos de dados (ex.: cliente.json)
├── imgs/             # Imagens do projeto
├── src/              # Código-fonte da aplicação
├── .gitignore
├── package.json
├── package-lock.json
└── server.js         # Ponto de entrada do servidor
```

##  Pré-requisitos

Antes de começar, você precisa ter instalado:

- [Node.js](https://nodejs.org/) (versão 18 ou superior recomendada)
- npm (já vem junto com o Node.js)
- [Git](https://git-scm.com/) para clonar o repositório

##  Instalação

```bash
# 1. Clone o repositório
git clone https://github.com/lucasrafaeldv/AULA13-atividade.git

# 2. Entre na pasta do projeto
cd AULA13-atividade

# 3. Instale as dependências
npm install
```

##  Como executar

**Modo normal:**

```bash
npm start
```

**Modo desenvolvimento** (reinicia o servidor automaticamente quando um arquivo é alterado):

```bash
npm run dev
```

>  **Dica:** confira no arquivo `server.js` qual porta o servidor utiliza e acesse `http://localhost:<porta>` no navegador.

##  Dados

Os clientes ficam em um arquivo JSON (`cliente.json`), que contém uma lista de objetos com os campos abaixo:

| Campo | Tipo   | Descrição                |
|-------|--------|--------------------------|
| `id`   | string | Identificador do cliente |
| `cpf`  | string | CPF do cliente           |
| `nome` | string | Nome do cliente          |

**Exemplo:**

```json
[
  {
    "id": "1",
    "cpf": "123456789",
    "nome": "Antony"
  },
  {
    "id": "2",
    "cpf": "123456789",
    "nome": "Joao"
  },
  {
    "id": "3",
    "cpf": "123456789",
    "nome": "Rafael"
  }
]
```

##  Rotas da API

>  **A completar:** liste aqui as rotas definidas no `server.js` / `src`, seguindo o formato da tabela.

| Método | Rota | Descrição |
|--------|------|-----------|
| `GET`  | `/`  | (descreva o que a rota faz) |

##  Scripts disponíveis

| Comando | O que faz |
|---------|-----------|
| `npm start` | Inicia o servidor com `node server.js` |
| `npm run dev` | Inicia o servidor com recarregamento automático (`node --watch`) |

##  Melhorias futuras

- [ ] Validar o CPF (11 dígitos) e impedir CPFs repetidos
- [ ] Adicionar rotas para criar, editar e remover clientes
- [ ] Criar testes automatizados
- [ ] Documentar a API com exemplos de requisição e resposta

