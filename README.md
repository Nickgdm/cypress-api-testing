# Testes Automatizados de API — Hub de Leitura

Projeto de automação de testes de API REST para o sistema educacional Hub de Leitura, utilizando Cypress.

## Objetivos
- Automatizar requisições para a API do Hub de Leitura.
- Validar respostas e comportamentos dos endpoints cobertos pelos testes.
- Praticar organização e execução de testes de API com Cypress.

## Tecnologias
- JavaScript
- Node.js e npm
- Cypress

## Pré-requisitos
- Node.js e npm instalados.
- Dependências do projeto instaladas.
- API do Hub de Leitura disponível no endereço esperado pela configuração dos testes.

## Instalação e execução
```bash
npm install
npx cypress open
```
Para execução em modo headless:
```bash
npx cypress run
```
Confira `package.json`, `cypress.config.js` e os arquivos em `cypress/` para confirmar scripts, URL base e especificações disponíveis.

## Estrutura do projeto
```text
hub-de-leitura-api-teste/
├── cypress/
├── cypress.config.js
├── package.json
├── package-lock.json
└── README.md
```

## Desafios práticos
Configurar a URL da API, preparar dados válidos e inválidos, enviar requisições automatizadas e validar status HTTP e conteúdo das respostas conforme os cenários existentes.

## Boas práticas adotadas
- Separação dos testes e configuração do Cypress.
- Execução repetível por comandos documentados.
- Validação explícita das respostas da API.

## 📚 Aprendizados
O projeto permite praticar automação de API com Cypress, incluindo configuração do ambiente, envio de requisições HTTP e validação de respostas. A leitura dos testes ajuda a identificar como os cenários cobrem os comportamentos implementados pela API.

## Considerações finais
A execução requer que a API esteja disponível e que a URL configurada corresponda ao ambiente local. Consulte os arquivos de teste para os cenários efetivamente implementados.

---

## 🎓 Formação
Atividade desenvolvida durante a formação profissionalizante em **Quality Assurance (QA) pela EBAC — Escola Britânica de Artes Criativas e Tecnologia**.