
# EvolutionAPI + n8n
## Requisitos

- Docker


## Instalação

Para instalar e inicializar tudo, basta rodar o seguinte comando no terminal:

```bash
  docker compose up -d
```
    
## Como Usar

### n8n

O n8n poderá ser acessado em ``http://localhost:5678`` e solicitará a criação de uma conta no primeiro acesso.

Se aparecer uma modal oferecendo uma chave gratuita para liberar todas as funcionalidades, siga o processo.

Para utilizar a EvolutionAPI no n8n, é preciso instalar um community node no n8n. Isso é feito em ``Settings > Community nodes > Install a community node``. Uma modal aparecerá solicitando um o nome de um npm package, onde deverá ser inserido ``n8n-nodes-evolution-api``. Marque o checkbox e clique em install.

### EvolutionAPI

A EvolutionAPI ficará disponível em ``http://localhost:8080`` e possui uma interface em ``http://localhost:8080/manager`` para gerenciar as instâncias e realizar algumas configurações e integrações.

A ``AUTHENTICATION_API_KEY`` que consta no arquivo ``.env`` não é obtida de nenhum lugar, você mesmo deve inventar uma no formato que quiser.

### Redis

O Redis ficará disponível em ``http://localhost:6379`` e é utilizado pela EvolutionAPI, mas não possui interface.

### PostgreSQL

O PostgreSQL ficará disponível em ``http://localhost:5432``e é utilizado pela EvolutionAPI e pelo n8n. 



## Links

 - [Documentação da EvolutionAPI](https://doc.evolution-api.com/v2/pt/get-started/introduction)

 - [Repositório do community node para n8n da EvolutionAPI](https://doc.evolution-api.com/v2/pt/get-started/introduction)

