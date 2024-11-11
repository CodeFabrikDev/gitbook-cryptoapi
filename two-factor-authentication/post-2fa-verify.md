---
description: Verifica o código de autenticação TOTP fornecido pelo usuário.
---

# \[POST] /2fa/verify

O método **\[POST] /2fa/verify** verifica a validade de um código de autenticação TOTP (Time-Based One-Time Password) fornecido pelo usuário, como parte do processo de autenticação de dois fatores (2FA). Ao receber o código temporário gerado por um aplicativo autenticador (por exemplo, Google Authenticator ou Authy), o método confirma se o código é correto e se está dentro do tempo de validade. Essa verificação adiciona uma camada extra de segurança ao processo de login, garantindo que apenas usuários com acesso ao dispositivo autenticador possam concluir o login e acessar a conta.

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
