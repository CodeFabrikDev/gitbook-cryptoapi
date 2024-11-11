---
description: Verifica o status de uma transação de conversão de moedas pelo ID da transação
---

# \[GET] /transaction-status/conversion

O método **\[GET] /transaction-status/conversion** permite verificar o status de uma transação de conversão de criptomoedas, utilizando o ID da transação. Ao fornecer o ID único da transação, o método retorna informações detalhadas sobre o progresso da conversão, como se a transação foi concluída, está pendente ou falhou. Esse recurso é útil para plataformas que desejam monitorar e fornecer atualizações em tempo real aos usuários sobre o status de suas conversões entre criptomoedas, oferecendo transparência e facilitando o acompanhamento de processos financeiros em andamento.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para verificar o status de uma transação da conversão, basta inserir o ID da transação e então clicar em "Execute".

#### Parâmetros

| Nome          | Descrição                                            |
| ------------- | ---------------------------------------------------- |
| transactionId | ID da transação de conversão para verificar o status |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "transactionId": "TX123456",
  "status": "Completed"
}
```
{% endtab %}
{% endtabs %}
