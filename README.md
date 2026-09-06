# API Connect 🚀

Uma API RESTful modular e escalável desenvolvida em **Node.js** e **Express** como Produto Mínimo Viável (MVP) para gerenciamento e persistência de usuários. O projeto foi projetado aplicando as melhores práticas de arquitetura de software, incluindo o princípio de **Separação de Responsabilidades (SoC)**, validação estrita de dados de entrada e padronização determinística de respostas HTTP.

---

## 🎯 Objetivo do Projeto

A **API Connect** tem como propósito servir como um serviço back-end desacoplado para integração com aplicações front-end ou mobile. Ela oferece operações completas de CRUD (*Create, Read, Update, Delete*) para o recurso de usuários, garantindo resiliência, validações de integridade e respostas padronizadas em formato JSON.

---

## 🛠️ Tecnologias Utilizadas

* **Node.js**: Ambiente de execução JavaScript assíncrono no servidor.
* **Express.js**: Microframework para gerenciamento de rotas e middlewares HTTP.
* **CORS**: Middleware para liberação de requisições Cross-Origin.
* **Nodemon**: Ferramenta de desenvolvimento para recarregamento automático do servidor.
* **Crypto (Módulo Nativo)**: Geração de identificadores únicos universais (`UUID v4`).

---

## 📁 Estrutura de Arquivos da Arquitetura (SoC)

```text
api-connect/
├── node_modules/
├── src/
│   ├── data/
│   │   └── mockData.js          # Camada de simulação de dados (RAM)
│   ├── controllers/
│   │   └── connectController.js # Regras de negócio e validações
│   ├── routes/
│   │   └── connectRoutes.js     # Mapeamento de endpoints e métodos HTTP
│   └── server.js                # Bootstrap e inicialização do servidor
├── .gitignore                   # Exclusão de dependências e arquivos sensíveis
├── package.json                 # Manifesto de dependências e scripts
└── README.md                    # Documentação técnica do projeto
