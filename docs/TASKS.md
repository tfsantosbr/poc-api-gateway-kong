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

- [ ] Estrutura

  - [ ] Provisionar o Kong no Docker Compose

- [ ] Funcionalidades

  - [ ] Mapear endpoints de Orders
  - [ ] Mapear endpoints de Products
  - [ ] Adicionar Rate Limit no endpoint GET /orders
  - [ ] Adicionar Rate Limit no endpoint GET /products
  - [ ] Adicionar Autenticação (Keycloak)
  - [ ] Adicionar Autorização (Keycloak) POST /orders (somente manager e email verificado)
  - [ ] Adicionar Correlation ID
  - [ ] Adicionar Monitoramento
    - [ ] Métricas
    - [ ] Traces
    - [ ] Logs
