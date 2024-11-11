---
description: >-
  Obtém as taxas de transação atuais para um par de moedas (base e quote) na
  mempool.
---

# \[GET] /transaction-fee/pair

O método **\[GET] /transaction-fee/pair** obtém as taxas de transação atuais para um par de moedas específico (moeda base e moeda de cotação) na mempool, onde transações aguardam processamento na rede blockchain. Ao especificar o par de moedas, como BTC/USDT ou ETH/BRL, o método retorna dados em tempo real sobre as taxas de transação para conversões entre essas moedas, incluindo taxas médias, mínimas e máximas. Esse recurso é útil para usuários e plataformas que desejam acompanhar os custos de transações entre pares específicos, permitindo que ajustem suas operações conforme as condições atuais de congestionamento e os custos na blockchain.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para verificar o status de uma transação da conversão, basta inserir o ID da transação e então clicar em "Execute".

#### Parâmetros

<table><thead><tr><th width="364">Nome</th><th>Descrição</th></tr></thead><tbody><tr><td>base</td><td>Código da moeda base</td></tr><tr><td>quote</td><td>Código da moeda de cotação</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "base": {
    "currency": "BTC",
    "fastest_fee_usd": 8.49,
    "normal_fee_usd": 2.52,
    "slow_fee_usd": 7.77
  },
  "quote": {
    "currency": "ETH",
    "fastest_fee_usd": 4.28,
    "normal_fee_usd": 3.78,
    "slow_fee_usd": 3.04
  }
}
```
{% endtab %}
{% endtabs %}
