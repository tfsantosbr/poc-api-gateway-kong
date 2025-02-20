# TASK

## Criar 2 microserviços de exemplo

- [x] Criar microserviço de Orders

  - [x] Criar endpoint de Healfhcheck
  - [x] Criar endpoint de CRUD de Orders
  - [x] Adicione compatibilidade com Dockerfile

- [x] Criar microserviço de Products

  - [x] Criar endpoint de Healfhcheck
  - [x] Criar endpoint public de categoria de Produtos
  - [x] Criar endpoint de CRUD de Produtos

## Krakend

- [x] Estrutura

  - [x] Provisionar o Kong no Docker Compose

- [x] Funcionalidades

  - [x] Mapear endpoints de Orders
  - [x] Mapear endpoints de Products
  - [x] Adicionar Rate Limit no endpoint GET /orders
  - [x] Adicionar Rate Limit no endpoint GET /products
  - [ ] Adicionar Autenticação (Keycloak) na rota POST /orders
  - [ ] Adicionar Autorização (Keycloak) POST /orders (somente manager e email verificado)
  - [x] Adicionar Correlation ID
  - [x] Adicionar Monitoramento
    - [x] Métricas
    - [x] Traces
    - [x] Logs
