---
description: Obtém as taxas de transação atuais para uma moeda específica na mempool.
---

# \[GET] /transaction-fee/single

O método **\[GET] /transaction-fee/single** mostra as taxas de transação atuais para uma moeda específica na mempool, que é o conjunto de transações pendentes aguardando confirmação na rede blockchain. Ao consultar as taxas de uma moeda específica, como BTC ou ETH, o método retorna informações em tempo real sobre as taxas médias, mínimas e máximas, ajudando os usuários a ajustar suas transações para confirmação mais rápida ou taxas mais econômicas. Essa funcionalidade é essencial para usuários e plataformas que desejam otimizar o custo e a velocidade de suas transações, fornecendo dados precisos e atualizados sobre o congestionamento e o custo das transações na rede blockchain escolhida.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para verificar a taxa de uma moeda, basta inserir a moeda e então clicar em "Execute".

#### Parâmetros

| Nome     | Descrição                 |
| -------- | ------------------------- |
| currency | Código da rede blockchain |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "currency": "BTC",
  "fastest_fee_usd": 9.71,
  "normal_fee_usd": 2.52,
  "slow_fee_usd": 4.49
}
```
{% endtab %}
{% endtabs %}
