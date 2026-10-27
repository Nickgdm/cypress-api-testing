<pre>
╔═════════════════════════════════════════════════════════════════════════════════════════════════════════╗
║                                TESTES AUTOMATIZADOS DE API — HUB DE LEITURA                             ║
╚═════════════════════════════════════════════════════════════════════════════════════════════════════════╝
</pre>
Projeto de estudo de automação de testes de API REST para o sistema Hub de Leitura, utilizando Cypress.

## SOBRE O PROJETO

O repositório contém testes voltados à validação de endpoints da API, incluindo requisições HTTP, códigos de status e conteúdo das respostas. A execução depende da disponibilidade da API e da configuração dos dados e das credenciais esperadas pelos cenários.

## OBJETIVOS

- Automatizar requisições para a API do Hub de Leitura.
- Validar respostas e comportamentos dos endpoints cobertos pelos testes.
- Praticar operações HTTP GET, POST, PUT e DELETE.
- Verificar códigos de status e conteúdo das respostas.
- Praticar a organização e a execução de testes automatizados de API.

## TECNOLOGIAS E FERRAMENTAS

- JavaScript
- Node.js e npm
- Cypress
- Faker, para geração de dados de teste

## PRÉ-REQUISITOS

- Node.js e npm instalados.
- Dependências do projeto instaladas.
- API do Hub de Leitura em execução e acessível em `http://localhost:3000/api/`, conforme a configuração registrada em `cypress.config.js`.
- Endpoints, dados e credenciais necessários aos cenários disponíveis no ambiente.

Alguns testes utilizam autenticação e funções auxiliares definidas em `cypress/support`. Verifique esses arquivos para compreender os requisitos do ambiente.

## INSTALAÇÃO E EXECUÇÃO

Instale as dependências:

```bash
npm install
```

Execute a suíte em modo headless:

```bash
npm test
```

Abra a interface do Cypress para selecionar e acompanhar os testes:

```bash
npx cypress open
```

Consulte o arquivo `package.json` para confirmar os comandos disponíveis no projeto.

## ESTRUTURA DO PROJETO

```text
hub-de-leitura-api-teste/
├── cypress/
│   ├── e2e/
│   ├── fixtures/
│   └── support/
├── cypress.config.js
├── package.json
├── package-lock.json
└── README.md
```

## CENÁRIOS DE TESTE

Os testes documentados abrangem cenários relacionados a:

- Listagem de usuários.
- Consulta de usuário por ID.
- Filtragem de resultados.
- Cadastro de usuários com dados válidos e inválidos.
- Atualização de usuários.
- Exclusão de usuários.

A execução depende dos endpoints, dos dados e das credenciais esperados pelo projeto. Há um cenário de exclusão marcado com `it.skip`, portanto ele não é executado pela suíte enquanto permanecer ignorado.

Os cenários listados descrevem a cobertura indicada pelos arquivos do projeto; os resultados precisam ser confirmados por meio da execução no ambiente configurado.

## BOAS PRÁTICAS

- Organizar os testes por meio da estrutura do Cypress.
- Separar arquivos de suporte e dados de teste dos cenários.
- Validar status HTTP e conteúdo das respostas.
- Considerar os requisitos de autenticação e a disponibilidade da API.
- Evitar armazenar credenciais ou segredos diretamente no código.
- Registrar falhas e confirmar os resultados pela execução real da suíte.

## APRENDIZADOS

O projeto oferece prática com automação de API utilizando Cypress, configuração de URL base, envio de requisições HTTP, autenticação, geração de dados dinâmicos e validação de status e conteúdo das respostas.

## CONSIDERAÇÕES FINAIS

Antes de executar a suíte, confirme que a API está ativa em `http://localhost:3000/api/` ou ajuste a configuração para o ambiente utilizado. Consulte os arquivos em `cypress/e2e` e os comandos auxiliares em `cypress/support` para conhecer os cenários e as dependências.
<pre>
╔═════════════════════════════════════════════════════════════════════════════════════════════════════════╗
║       Atividade desenvolvida durante a formação profissionalizante em Quality Assurance (QA) pela       ║
║                     EBAC — Escola Britânica de Artes Criativas e Tecnologia                             ║
╚═════════════════════════════════════════════════════════════════════════════════════════════════════════╝
</pre>
