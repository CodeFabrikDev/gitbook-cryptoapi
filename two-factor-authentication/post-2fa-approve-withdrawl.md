---
description: >-
  Aprova uma solicitação de saque verificando o código de autenticação de duplo
  fator.
---

# \[POST] /2fa/approve-withdrawl

O método **\[POST] /2fa/approve-withdrawl** permite aprovar uma solicitação de saque após a verificação do código de autenticação de dois fatores (2FA) fornecido pelo usuário. Ele assegura que o usuário não só iniciou a transação, mas também possui acesso ao dispositivo autenticador, adicionando uma camada crítica de segurança ao processo de retirada de fundos. Ao validar o código temporário TOTP (Time-Based One-Time Password) ou outro método de 2FA, este método ajuda a proteger a conta contra retiradas não autorizadas, garantindo que apenas usuários autenticados possam completar transações financeiras.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "userId": "user123",
  "token": "123456"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
