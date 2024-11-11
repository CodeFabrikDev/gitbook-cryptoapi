---
description: Gera um segredo TOTP para o usuário configurar a autenticação de duplo fator.
---

# \[POST] /2fa/generate

O método **\[POST] /2fa/generate** gera um segredo TOTP (Time-Based One-Time Password) para o usuário, permitindo a configuração de autenticação de dois fatores (2FA) em sua conta. O segredo TOTP é um código exclusivo que pode ser escaneado em aplicativos autenticadores, como Google Authenticator ou Authy, para gerar códigos de autenticação temporários. Esse processo adiciona uma camada extra de segurança, exigindo que o usuário insira um código de autenticação adicional ao efetuar login, além da senha, protegendo a conta contra acessos não autorizados.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "userId": "user123"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
