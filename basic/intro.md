# Responsabilidades dentro da Web

A web é dividida em 3 pilares, que são:

- HTML
- CSS
- Javascript

Cada um é responsável por uma função dentro do código

## HTML

É o responsável por inserir elemento dentro de uma página, por exemplo: <br>

Exibir um ou mais elementos, tais como:

- entrada de texto (input type="text")
- parágrafo (p)
- botão (button)
- lista (ul)
- caixa de seleção (select)
- selecionar uma opção em um grupo (input type="radio")

> A Lista acima apresenta alguns exemplos de elementos disponíveis no HTML, para um lista mais completa, acessa o <br> [W3C School](https://www.w3schools.com/tags/)

## CSS

É o responsável por inserir o estilo nos elementos do html, por exemplo: <br>

- cor da letra
- tamanho da letra
- cor padrão do fundo da página
- tamanho de um botão
- se uma entrada de texto terá ou não borda
- como os elementos serão dispostos

> Para mais referencias acesse [W3C School](https://www.w3schools.com/cssref/default.asp)

## Javascript

É o responsável por manipular a DOM conforme as interações do usuário.
Quando uma página é carregada, o DOM é montado conforme as orientações do HTML e CSS.
Isso é estático e sem javascript, não alteraria. <br>

Um exemplo prático:
Vamo supor que você precisa ir ao supermercado, para evitar o uso desnecessário de papel, você achou um site
que faz uma lista conforme você digita o que quer e pressiona um botão de adicionar ou pressione a tecla 'enter'

Você observa que ao digitar Café, e aplicar à ação, o valor digitado é inserido na lista.
Bom, o que faz essa inserção na DOM, ou seja, nos elementos já montados é o JS. Sem ele, não ocorreria isso, você sempre iria visualizar a lista como da primeira vez que o DOM foi montado.

Uma lista de sites bons para consultar sobre JS:

- [Developer mozilla](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [W3C School](https://www.w3schools.com/js/)

## Ordem de carregamento

1. HTML
2. CSS
3. Javascript

---

Essa é a base da web, essa tríade, é a responsável por dar vida aos sites.
