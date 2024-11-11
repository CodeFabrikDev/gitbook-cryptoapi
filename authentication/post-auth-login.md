---
description: Autenticar e obter um token JWT
---

# \[POST] /auth/login

O método **\[POST] /auth/login** autentica as credenciais do usuário e retorna um token JWT (JSON Web Token) para acesso seguro aos demais endpoints protegidos da aplicação. Ao enviar as credenciais de login, como e-mail e senha, o usuário recebe um token JWT válido, que pode ser usado para autenticação em chamadas subsequentes, evitando a necessidade de reapresentar as credenciais. O uso de JWT oferece uma maneira segura e eficiente de gerenciar sessões de usuário em aplicações distribuídas, garantindo que apenas usuários autenticados possam acessar recursos sensíveis durante o período de validade do token.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "username": "admin",
  "password": "password123"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InNkdmFsZSIsInN1YiI6MSwiaWF0IjoxNzMxMzMwMTU1LCJleHAiOjE3MzEzNTg5NTV9.8SzGYaLV4rTzXA70Rx4AhKdSxku0STA06zUcRNvp9A2"
}
```
{% endtab %}
{% endtabs %}
