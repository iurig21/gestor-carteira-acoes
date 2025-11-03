# Gestor de carteira de ações

## Sobre o Projeto

Este projeto foi desenvolvido no âmbito da cadeira de **Programação Web II**.O gestor de carteira de ações é uma aplicação web desenvolvida em Angular que permite aos usuários gerenciar suas carteiras de investimentos em ações de forma simples e intuitiva. Com esta ferramenta, você pode adicionar, editar, visualizar e remover ações do seu portfólio, mantendo um controle organizado dos seus investimentos.

### Funcionalidades

- ✅ Visualização da carteira de ações
- ✅ Adição de novas ações ao portfólio
- ✅ Edição de ações existentes
- ✅ Remoção de ações da carteira
- ✅ Interface responsiva e intuitiva

## Tecnologias Utilizadas

- **Angular** (v19.2.3) - Framework front-end
- **JSON Server** - API REST fake para desenvolvimento
- **TypeScript** - Linguagem de programação
- **HTML/CSS** - Estrutura e estilização


## Requisitos

Antes de rodar o projeto, você deve ter o [json-server](https://github.com/typicode/json-server) instalado globalmente:

```bash
npm install -g json-server
```

## Iniciando o Backend (JSON Server)

Para iniciar a API fake com o json-server, execute:

```bash
json-server --watch db.json
```

Isso iniciará um servidor REST API fake usando o arquivo `db.json`.

### Endpoints da API (json-server)

- `GET /portfolio`  
  Retorna a lista de todas as ações da carteira.

- `GET /portfolio/:id`  
  Retorna uma ação específica pelo id.

- `POST /portfolio`  
  Adiciona uma nova ação à carteira.

- `PUT /portfolio/:id`  
  Atualiza todos os dados de uma ação existente.

- `PATCH /portfolio/:id`  
  Atualiza parcialmente os dados de uma ação existente.

- `DELETE /portfolio/:id`  
  Remove uma ação da carteira pelo id.

## Servidor de Desenvolvimento

Em um terminal separado, inicie o servidor de desenvolvimento do Angular:

```bash
ng serve
```

Depois que o servidor estiver rodando, abra seu navegador e acesse `http://localhost:4200/`. A aplicação irá recarregar automaticamente sempre que você modificar qualquer um dos arquivos fonte.

## Gerando Código

O Angular CLI possui ferramentas poderosas de geração de código. Para gerar um novo componente, execute:

```bash
ng generate component nome-do-componente
```

Para uma lista completa dos esquemas disponíveis (como `components`, `directives` ou `pipes`), execute:

```bash
ng generate --help
```

## Build

Para compilar o projeto, execute:

```bash
ng build
```

Isso irá compilar seu projeto e salvar os artefatos de build no diretório `dist/`. Por padrão, o build de produção otimiza sua aplicação para performance e velocidade.

## Executando Testes Unitários

Para executar testes unitários com o [Karma](https://karma-runner.github.io), use o comando:

```bash
ng test
```

## Executando Testes de Integração (E2E)

Para testes de ponta a ponta (e2e), execute:

```bash
ng e2e
```
