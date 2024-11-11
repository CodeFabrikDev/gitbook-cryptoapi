---
description: Lista todos os endereços de depósito gerados para cada rede blockchain
---

# \[GET] /deposit/list

O método **\[GET] /deposit/list** retorna uma lista de todos os endereços de depósito gerados para cada rede blockchain associada à conta do usuário. Ele fornece uma visão centralizada dos endereços públicos, permitindo que os usuários visualizem facilmente os endereços específicos de cada rede (como Bitcoin, Ethereum, entre outras), para os quais podem receber depósitos. Essa funcionalidade é útil para plataformas que gerenciam múltiplas criptomoedas e desejam facilitar o acompanhamento dos endereços ativos, garantindo que as transações sejam enviadas para os locais corretos na rede blockchain.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para listar todos os depositos gerados, basta  clicar em "Execute".

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "networkId": 1,
    "networkName": "Ethereum",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 2,
    "networkName": "Binance Smart Chain",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 3,
    "networkName": "Polygon",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "networkId": 4,
    "networkName": "Avalanche",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  }
]
```
{% endtab %}
{% endtabs %}
