---
description: >-
  Verifica o status de uma transação de saque de criptomoedas pelo ID da
  transação
---

# \[GET] /transaction-status/withdrawl

O método **\[GET] /transaction-status/withdrawl** permite verificar o status de uma transação de saque de criptomoedas, utilizando o ID único da transação. Ao fornecer o ID, o método retorna o estado atual da retirada, informando se a transação foi processada, está em andamento ou se houve algum erro. Esse recurso é essencial para usuários que desejam acompanhar o progresso de seus saques, oferecendo uma visão clara e em tempo real sobre o status da transação e garantindo maior transparência e confiança nas operações financeiras.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para verificar o status de uma transação da conversão, basta inserir o ID da transação e então clicar em "Execute".

#### Parâmetros

<table><thead><tr><th width="364">Nome</th><th>Descrição</th></tr></thead><tbody><tr><td>transactionId</td><td>ID da transação de conversão para verificar o status</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "transactionId": "TX987654",
  "status": "Pending"
}
```
{% endtab %}
{% endtabs %}
