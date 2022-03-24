# About
## OpenPolicyAgent Auth Plugin 

Plugin que adiciona a capacidade autenticação baseada em OpenPolicyAgent a stack, criando assim uma lambda que faz essa integração e torna disponível a autenticação dos endpoints ao adicionar uma configuração das operações descritas no contrato OpenAPI responsável por criar os endpoints.

Exemplo:

```yaml
    get:
      operationId: get-auction
      description: Get auction data by id

      # operation level
      security:
        - jwtAuth: []
```
