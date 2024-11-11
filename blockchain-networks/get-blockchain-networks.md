---
description: Listar todas as redes blockchain disponíveis
---

# \[GET] /blockchain-networks

O método **\[GET] /blockchain-networks** da nossa API permite que você acesse e consulte as redes blockchain suportadas para integração em sua aplicação. Com este endpoint, você pode obter uma lista completa das principais redes blockchain disponíveis para transações.

Este recurso é ideal para desenvolvedores que buscam identificar as redes compatíveis com sua plataforma ou aplicativo, facilitando a escolha da blockchain mais adequada para o tipo de transação ou serviço que desejam implementar. A API fornece informações detalhadas sobre cada rede, como nome, o ChainID(código da rede) e o endereço de depósito.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, basta clicar em "Execute" para utilizar o método.

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
[
  {
    "id": 1,
    "name": "Ethereum",
    "chainId": "1",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 2,
    "name": "Binance Smart Chain",
    "chainId": "56",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 3,
    "name": "Polygon",
    "chainId": "137",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  },
  {
    "id": 4,
    "name": "Avalanche",
    "chainId": "43114",
    "depositAddress": "0x6de381fb542aa0911a3cd1f6ffb59b3ac9caa1c7"
  }
]
```
{% endtab %}
{% endtabs %}
