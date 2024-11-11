---
description: Obtém a cotação para um par de moedas específico
---

# \[GET] /exchange-rates/pair

O método **\[GET] /exchange-rates/pair** da nossa API permite que você consulte o valor atual de um par de criptomoedas específico, como **BTCUSD**, **ETHUSD**, entre outros. Este endpoint fornece informações em tempo real sobre a cotação de diversos pares de moedas, permitindo que você integre dados de mercado diretamente em sua aplicação, plataforma de e-commerce, ou serviço financeiro.

Com esse recurso, é possível obter a cotação de um par de moedas específico em diferentes unidades de medida, como o valor em dólares americanos (USD), euros (EUR), ou outras moedas fiduciárias e digitais. O método retorna informações precisas sobre o preço de compra e venda, bem como a variação de preço em um período determinado, ajudando a tomar decisões informadas sobre transações e investimentos.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para obter a cotação para um par de moedas específico, basta inserir o ID da criptomoeda desejada(ex: bitcoin, ethereum, etc) e a moeda contra a qual será cotada(ex: usd, brl), então clicar em "Execute".

#### Parâmetros

| Nome       | Descrição                                     |
| ---------- | --------------------------------------------- |
| cryptold   | ID da criptomoeda conforme CoinGecko          |
| vcCurrency | Moeda contra a qual a criptomoeda será cotada |

### Response Body

{% tabs %}
{% tab title="Code: 200" %}
```
{
  "cryptoId": "bitcoin",
  "vsCurrency": "usd",
  "price": 82274
}
```
{% endtab %}
{% endtabs %}
