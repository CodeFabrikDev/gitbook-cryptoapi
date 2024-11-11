---
description: Obtém a cotação de uma criptomoeda para USD(Dólar)
---

# \[GET] /exchange-rates/crypto-to-usd

O método **\[GET] /exchange-rates/crypto-to-usd** permite a obtenção da cotação atual de uma criptomoeda específica, como o Bitcoin (BTC), em relação ao dólar americano (USD). Ele consulta dados em tempo real de mercados financeiros e retorna o valor mais recente da conversão entre a criptomoeda e o USD, possibilitando que aplicações e usuários acompanhem as variações de preço e tomem decisões informadas em suas transações.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para obter a cotação de uma criptomoeda para USD, basta inserir o ID da criptomoeda desejada(ex: BTC, ETH, etc) e então clicar em "Execute".

#### Parâmetros

| Nome         | Descrição              |
| ------------ | ---------------------- |
| cryptoSymbol | Símbolo da criptomoeda |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "cryptoId": "bitcoin",
  "vsCurrency": "usd",
  "price": 82194
}
```
{% endtab %}
{% endtabs %}
