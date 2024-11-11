---
description: >-
  Obtém a lista de todos os pares de moedas que podem ser negociados, com filtro
  opcional para moedas base e cotação.
---

# \[GET] /tokens/trading-pairs

O método **\[GET] /transaction-status/conversion** retorna a lista completa de todos os pares de moedas disponíveis para negociação, com a opção de aplicar filtros para moedas base e cotação. Ao fornecer parâmetros como a moeda base (por exemplo, BTC, USDT) ou a moeda de cotação (como BRL ou USD), os usuários podem refinar a consulta para obter apenas os pares que atendem às suas necessidades específicas. Esse recurso é essencial para plataformas de câmbio e negociação de criptomoedas, permitindo que traders e desenvolvedores acessem informações atualizadas sobre os pares de moedas disponíveis e realizem transações de forma mais eficiente e personalizada.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para filtrar a lista de todos os pares de moedas que podem ser negociados, basta inserir a moeda base e a moeda de cotação e então clicar em "Execute", caso deseje ver a lista completa, basta deixar em branco.

#### Parâmetros

| Nome  | Descrição                                            |
| ----- | ---------------------------------------------------- |
| base  | Moeda base para filtrar os pares de negociação       |
| quote | Moeda de cotação para filtrar os pares de negociação |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "id": "BAT-ETH",
    "base_currency": "BAT",
    "quote_currency": "ETH",
    "display_name": "BAT-ETH",
    "status": "online",
    "trading_disabled": false
  },
  {
    "id": "SYLO-USD",
    "base_currency": "SYLO",
    "quote_currency": "USD",
    "display_name": "SYLO-USD",
    "status": "delisted",
    "trading_disabled": true
  },
  {
    "id": "COMP-USD",
    "base_currency": "COMP",
    "quote_currency": "USD",
    "display_name": "COMP-USD",
    "status": "online",
    "trading_disabled": false
  },
  {
    "id": "ARKM-USD",
    "base_currency": "ARKM",
    "quote_currency": "USD",
    "display_name": "ARKM/USD",
    "status": "online",
    "trading_disabled": false
  }
  ]
```
{% endtab %}
{% endtabs %}
