---
description: Criação de carteira Blockchain
---

# \[POST] /wallet/create

O método **\[POST] /wallet/create** permite a criação de uma nova carteira em blockchain, vinculada à conta do usuário. A carteira gerada inclui um endereço público único, usado para armazenar e transacionar criptomoedas com segurança. Este endpoint facilita a gestão de ativos digitais ao criar automaticamente uma carteira que pode receber depósitos, realizar saques e monitorar saldos em tempo real. Ideal para plataformas que desejam fornecer carteiras individuais aos seus usuários, este método oferece um ponto de entrada seguro para começar a transacionar no blockchain de forma descentralizada e rastreável.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, basta clicar em "Execute" para utilizar o método.

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "publicKey": "0x0ED99A476FCCeD2f609C80A312FDAFdeDEE85AA1"
}
```
{% endtab %}
{% endtabs %}
