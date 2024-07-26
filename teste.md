# Desafios Práticos de JavaScript (ES6+)

> **Nota:**
>  - Utilize a abordagem ES6+ para resolver os exercícios.
>  - Entrega: todas as soluções devem estar em um único repositório (GitHub via fork).
>  - O estilo do código fica a critério do candidato e não é o foco principal do teste.
>  - Caso não consiga resolver todos os exercícios, envie mesmo assim.

## Desafios

### E.1 Calcular o valor total das parcelas de um financiamento

Crie uma função que receba o valor de um produto, a quantidade de parcelas e a taxa de juros mensal. A função deve retornar o valor total a ser pago ao final do financiamento.

A fórmula é a seguinte:

$$ A = P \times \left( \frac{(1 + i)^n - 1}{i} \right) $$

Onde:
- $A$ é o valor total a ser pago ao final do financiamento.
- $P$ é o valor da parcela.
- $i$ é a taxa de juros mensal.
- $n$ é o número de parcelas.

### E.2 Verificar a disponibilidade de um produto no estoque

Crie uma função que receba o SKU de um produto e uma lista de produtos no estoque. A função deve retornar `true` se o produto estiver disponível em estoque e `false` caso contrário.

Considere a seguinte lista de produtos:

```javascript
const produtos = [
    { sku: 1001, nome: 'Camiseta', quantidade: 5 },
    { sku: 1002, nome: 'Calça', quantidade: 10 },
    { sku: 1003, nome: 'Vestido', quantidade: 3 }
];
```

### E.3 Calcular o frete para uma entrega

Crie uma função que receba o peso do pedido, a distância para a entrega e uma tabela de preços por peso e distância. A função deve retornar o valor do frete.

Considerando a seguinte tabela de preços:

```javascript
// Tabela de preços
const tabelaPrecos = {
    '0-1,0-5': 10.0,    // Até 1 kg e até 5 km: R$ 10.00
    '0-1,6-10': 15.0,   // Até 1 kg e 6-10 km: R$ 15.00
    '1-5,0-5': 20.0,    // 1-5 kg e até 5 km: R$ 20.00
    '1-5,6-10': 25.0,   // 1-5 kg e 6-10 km: R$ 25.00
    '5-10,0-5': 30.0,   // 5-10 kg e até 5 km: R$ 30.00
    '5-10,6-10': 35.0   // 5-10 kg e 6-10 km: R$ 35.00
};
```

### E.4 Atualizar o estoque após uma venda

Crie uma função que receba uma lista de itens vendidos (cada item com SKU e quantidade) e o estoque atual. A função deve retornar o estoque atualizado após a venda.

Considere a seguinte lista de itens vendidos:

```javascript
const itensVendidos = [
    { sku: 1001, quantidade: 2 },
    { sku: 1002, quantidade: 1 },
    { sku: 1003, quantidade: 5 }
];
```

E a seguinte lista de estoque:

```javascript
const estoque = [
    { sku: 1001, quantidade: 5 },
    { sku: 1002, quantidade: 2 },
    { sku: 1003, quantidade: 5 }
];
```

Ao final a função deve retornar a seguinte lista de estoque atualizada:

### E.5 Gerar relatório de vendas

Crie uma função que receba uma lista de vendas (cada venda com SKU, quantidade e valor total) e um período de datas. A função deve retornar um relatório com o total vendido por SKU e o valor total vendido no período.

Considere a seguinte lista de vendas:

```javascript
const vendas = [
    { sku: 1001, quantidade: 2, valorTotal: 50.00, data: '2021-01-01' },
    { sku: 1002, quantidade: 1, valorTotal: 20.00, data: '2021-01-01' },
    { sku: 1003, quantidade: 5, valorTotal: 100.00, data: '2021-01-02' },
    { sku: 1001, quantidade: 1, valorTotal: 25.00, data: '2021-01-02' }
];

```


## Instruções de Entrega

1. Crie um repositório no GitHub e faça um fork deste repositório.
2. Adicione suas soluções no repositório.
3. Envie o link do seu repositório com as soluções.

Boa sorte com os desafios! Se precisar de ajuda, sinta-se à vontade para entrar em contato.