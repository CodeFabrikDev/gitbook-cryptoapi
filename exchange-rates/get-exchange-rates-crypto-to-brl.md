---
description: Obtém a cotação de uma criptomoeda para BRL(Real)
---

# \[GET] /exchange-rates/crypto-to-brl

O método **\[GET] /exchange-rates/crypto-to-brl** permite a obtenção da cotação atual de uma criptomoeda específica, como o Bitcoin (BTC), em relação ao real brasileiro (BRL). Ele consulta dados em tempo real de mercados financeiros e retorna o valor mais recente da conversão entre a criptomoeda e o BRL, possibilitando que aplicações e usuários acompanhem as variações de preço e tomem decisões informadas em suas transações.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para obter a cotação de uma criptomoeda para BRL, basta inserir o ID da criptomoeda desejada(ex: BTC, ETH, etc) e então clicar em "Execute".

#### Parâmetros

| Nome         | Descrição              |
| ------------ | ---------------------- |
| cryptoSymbol | Símbolo da criptomoeda |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "symbol": "BTCBRL",
  "price": 475081.32000000007
}
```
{% endtab %}
{% endtabs %}
