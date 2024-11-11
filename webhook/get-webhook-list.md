---
description: Retorna uma lista de todos os webhooks cadastrados
---

# \[GET] /webhook/list

O método **\[GET] /webhook/list** retorna uma lista completa de todos os webhooks cadastrados pelo usuário.

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
    "url": "https://meusite.com/webhook",
    "transactionId": "TX123456"
  }
]
```
{% endtab %}
{% endtabs %}
