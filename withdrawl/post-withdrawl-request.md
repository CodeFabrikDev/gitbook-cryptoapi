---
description: >-
  Solicita um saque de criptomoeda, exigindo um código de aprovação de duplo
  fator.
---

# \[POST] /withdrawl/request

O método **\[POST] /withdrawl/request** permite solicitar um saque de criptomoeda, exigindo a confirmação adicional por meio de um código de autenticação de dois fatores (2FA) para garantir a segurança da transação. Ao realizar a solicitação de saque, o usuário deve fornecer o código temporário gerado por um aplicativo autenticador, como Google Authenticator ou Authy, para validar a operação. Esse processo adiciona uma camada extra de proteção, evitando saques não autorizados e garantindo que apenas usuários autenticados possam concluir transações de retirada de fundos.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "address": "0xRecipientAddress123",
  "amount": 1.5,
  "networkId": 1,
  "coin": "USDT",
  "userId": "user123",
  "approvalCode": "b3b7c9b2-48d6-4f0b-8881-3f2cdb15a5e9"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
