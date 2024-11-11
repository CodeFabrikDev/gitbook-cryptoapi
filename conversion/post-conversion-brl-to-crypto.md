---
description: >-
  Converte um valor em BRL(Real) para uma quantidade equivalente em criptomoeda
  específica
---

# \[POST] /conversion/brl-to-crypto

O método **\[POST] /conversion/brl-to-crypto** converte um valor em reais (BRL) para a quantidade equivalente em uma criptomoeda específica, como USDT (Tether). Essa funcionalidade é útil para usuários e aplicações que desejam conhecer o valor aproximado de compra de criptomoedas em moeda local, facilitando transações e tomada de decisão em tempo real com base nas cotações do mercado.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "amount": 100,
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "originalAmountInBrl": 100,
  "cryptoAmount": 17.2608,
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum",
  "rateInfo": {
    "brlToUsdRate": 0.174,
    "cryptoToUsdRate": 1
  },
  "fee": "0.14",
  "finalAmountInUsd": "17.26"
}
```
{% endtab %}
{% endtabs %}
