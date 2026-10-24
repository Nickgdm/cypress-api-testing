# Testes Automatizados de API — Hub de Leitura

Projeto de automação de testes de API REST para o sistema educacional Hub de Leitura, utilizando Cypress.

## Objetivos
- Automatizar requisições para a API do Hub de Leitura.
- Validar respostas e comportamentos dos endpoints cobertos pelos testes.
- Praticar operações HTTP GET, POST, PUT e DELETE e validações de status e payloads.

## Tecnologias
- JavaScript
- Node.js e npm
- Cypress
- Faker para geração de dados de teste

## Pré-requisitos
- Node.js e npm instalados.
- Dependências instaladas com `npm install`.
- API do Hub de Leitura disponível em `http://localhost:3000/api/`, conforme `cypress.config.js`.
- A API deve conter os endpoints e dados esperados pelos cenários; alguns testes usam autenticação e funções auxiliares definidas em `cypress/support`.

## Instalação e execução

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

## Estrutura do projeto

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

## Cenários cobertos
A suíte contém cenários para listar usuários, consultar por ID, filtrar resultados, cadastrar usuários com dados válidos e inválidos, atualizar usuários e excluir usuários. Os testes dependem da disponibilidade da API e dos dados/credenciais esperados no ambiente.

**Observação:** há um cenário de exclusão marcado como ignorado (`it.skip`) no arquivo de testes; ele não será executado pela suíte. Os resultados reais devem ser confirmados executando os testes no ambiente configurado.

## 📚 Aprendizados
O projeto permite praticar automação de API com Cypress, configuração de URL base, envio de requisições HTTP, autenticação, geração de dados dinâmicos e validação de status e conteúdo das respostas.

## Considerações finais
A execução requer que a API esteja ativa em `http://localhost:3000/api/` ou que a configuração seja ajustada para o ambiente utilizado. Consulte os testes em `cypress/e2e` e os comandos auxiliares em `cypress/support` para conhecer os cenários implementados.

---

## 🎓 Formação
Atividade desenvolvida durante a formação profissionalizante em **Quality Assurance (QA) pela EBAC — Escola Britânica de Artes Criativas e Tecnologia**.
