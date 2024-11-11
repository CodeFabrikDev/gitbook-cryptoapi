---
description: Obter detalhes de uma rede blockchain específica
---

# \[GET] /blockchain-networks/{id}

O método **\[GET] /blockchain-networks/{id}** da nossa API permite que você consulte informações detalhadas sobre uma rede blockchain específica, fornecendo dados cruciais sobre sua configuração, status e características. Ao inserir o **ID da Rede**, você recebe um conjunto completo de informações relacionadas a essa blockchain, incluindo parâmetros técnicos, status atual, taxas de transação, capacidade de processamento e muito mais.

Este endpoint é ideal para desenvolvedores e plataformas que precisam obter detalhes precisos sobre uma rede específica para realizar integrações ou monitorar o desempenho de suas transações em tempo real. Ele também é útil para verificar configurações como consenso, tempo médio de bloqueio, métodos de validação e compatibilidade com contratos inteligentes.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para ver os detalhes de uma das redes disponíveis, basta inserir o ID da rede blockchain desejada e então clicar em "Execute".

#### Parâmetros

| Nome | Descrição             |
| ---- | --------------------- |
| id   | ID da rede blockchain |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
```
{% endtab %}
{% endtabs %}
