# 📦 Desafio: Controle de Estoque

## 📝 Descrição

Este projeto é um sistema simples de **controle de estoque** desenvolvido com **HTML** e **JavaScript puro**, ideal para o gerenciamento de produtos em uma loja virtual de eletrônicos. Ele permite **cadastro**, **venda**, **reposição**, **remoção** e **exibição de relatórios** dos produtos, com regras de negócio bem definidas para garantir integridade do estoque.

---

## 🖥️ Funcionalidades

* **Cadastrar Produto**

  * Registra nome, código único e quantidade do produto.
  * Exige todos os campos preenchidos.
  * A quantidade mínima para cadastro é de 10 unidades.
  * Impede códigos duplicados.

* **Repor Estoque**

  * Atualiza o estoque de um produto existente.
  * Requer nome, código e quantidade a repor (> 0).
  * Exibe mensagem de sucesso ou erro.

* **Vender Produto**

  * Reduz a quantidade em estoque.
  * Impede vendas que ultrapassem a quantidade disponível.
  * Exibe mensagem de sucesso ou erro.
  * Alerta se o estoque ficar abaixo de 10 unidades.

* **Exibir Relatório**

  * Mostra todos os produtos com suas quantidades e status do estoque.
  * Identifica e exibe:

    * Produto com **maior** e **menor** quantidade em estoque.
    * Produto **mais vendido** e **menos vendido**.
  * Status:

    * **OK**: Estoque igual ou acima de 10.
    * **Precisa Repor**: Estoque abaixo de 10.

* **Remover Produto**

  * Remove um produto de todas as listas com base em nome e código.
  * Utiliza o método `.splice()` para exclusão.

---

## 📋 Regras de Negócio

* Estoque mínimo: **10 unidades** por produto.
* Não é permitido cadastrar produtos com código repetido.
* Não é permitido vender sem estoque suficiente.
* Após cada operação de **venda** ou **reposição**, o relatório é atualizado.

---

## ⚠️ Restrições Técnicas

* **Não utilizar** `indexOf`, `includes` ou `JSON`.
* Pesquisas são feitas com loops `for` e comparações diretas.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5**: Interface do usuário.
* **JavaScript**: Manipulação de dados e lógica de negócio.

---

## 💡 Exemplo de Relatório

```
Código: ABZ | Produto: Arroz | Quantidade em Estoque: 12 (OK)
Código: ABPSC | Produto: Feijão | Quantidade em Estoque: 4 (Precisa Repor)
Código: 123A | Produto: Caneta | Quantidade em Estoque: 75 (OK)
Código: EHFD | Produto: Caderno | Quantidade em Estoque: 2 (Precisa Repor)

Produto com maior quantidade de estoque: Caneta
Produto com menor quantidade em estoque: Caderno
Produto mais vendido: Arroz
Produto menos vendido: Feijão
```

---

## 🚀 Como Usar

1. Abra o arquivo `.html` em seu navegador.
2. Preencha os campos para cadastrar, repor, vender ou remover produtos.
3. Clique em “Exibir Relatório” para ver o status do estoque.

---

## ✅ Conclusão

Este projeto cumpre os requisitos de um sistema de controle de estoque básico com lógica de negócios e manipulação de arrays sem recursos avançados de JavaScript. Ideal para estudos introdutórios de estrutura de dados e lógica de programação.
