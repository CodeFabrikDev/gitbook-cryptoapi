---
description: Converte uma quantidade específica de criptomoeda para BRL
---

# \[POST] /conversion/crypto-to-brl

O método **\[POST] /conversion/crypto-to-brl** realiza a conversão de uma quantidade específica de uma criptomoeda, como BTC (Bitcoin) ou USDT (Tether), para o valor equivalente em BRL (real brasileiro). Ao fornecer a quantidade desejada de criptomoeda, o método retorna o valor correspondente em BRL, com base na cotação atual de mercado. Esse recurso é útil para aplicações que precisam exibir o valor de criptomoedas em moeda local, ajudando usuários a visualizar o valor de seus ativos digitais em reais, o que facilita transações, cálculos e a tomada de decisões financeiras.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "cryptoAmount": 0.5,
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
  "cryptoAmount": 0.5,
  "equivalentBrl": "2.85",
  "fee": "0.00",
  "finalAmountInUsd": "0.50",
  "cryptoSymbol": "USDT",
  "networkId": 1,
  "networkName": "Ethereum",
  "rateInfo": {
    "brlToUsdRate": 0.174,
    "cryptoToUsdRate": 1
  }
}
```
{% endtab %}
{% endtabs %}
