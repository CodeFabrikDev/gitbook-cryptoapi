---
description: Registra um novo webhook associado a uma transação de saque específica
---

# \[POST] /webhook/register

O método **\[POST] /webhook/register** permite o registro de um novo webhook associado a uma transação de saque específica. Ao configurar o webhook, o usuário pode receber notificações em tempo real sobre o status de uma transação de retirada, como confirmações, processamento ou conclusão. Essa funcionalidade é ideal para desenvolvedores e plataformas que desejam monitorar automaticamente o progresso das transações e integrar notificações instantâneas em seus sistemas, facilitando o acompanhamento e a automação de ações relacionadas a saques em criptomoedas.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

exemplo:

```
{
  "url": "https://meusite.com/webhook",
  "transactionId": "TX123456"
}
```

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
{
  "id": 1,
  "url": "https://meusite.com/webhook",
  "transactionId": "TX123456"
}
```
{% endtab %}
{% endtabs %}
