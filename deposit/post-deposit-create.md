---
description: Gera um endereço de depósito específico para uma rede blockchain
---

# \[POST] /deposit/create

O método **\[POST] /deposit/create** gera um endereço de depósito único e específico para uma rede blockchain, permitindo que o usuário receba criptomoedas de forma segura. Ao solicitar a geração de um endereço, o sistema cria automaticamente um endereço público válido para a rede blockchain escolhida (como Bitcoin, Ethereum, ou outras), que pode ser usado para depósitos futuros. Esse recurso facilita a recepção de fundos, fornecendo uma maneira prática e segura de gerenciar transações de entrada, garantindo que os depósitos sejam enviados para o endereço correto na rede blockchain.

### Autorização

Bearer token permite que as solicitações sejam autenticadas usando uma chave de acesso, como um JSON Web Token (JWT). O token é uma sequência de texto incluída no cabeçalho da solicitação.

```
Bearer <Your API token>
```

### Request Body

Não há, para gerar um endereço de deposito, basta inserir o ID da rede e então clicar em "Execute".

#### Parâmetros

<table><thead><tr><th width="364">Nome</th><th>Descrição</th></tr></thead><tbody><tr><td>networkId</td><td>ID da rede blockchain para a qual o endereço de depósito será gerado</td></tr></tbody></table>

### Response Body

{% tabs %}
{% tab title="Code: 201" %}
```
```
{% endtab %}
{% endtabs %}
