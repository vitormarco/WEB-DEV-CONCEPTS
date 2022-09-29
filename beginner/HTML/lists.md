## Listas

Existes dois tipos de listas no HTML.

- lista ordenada;
- lista não-ordenada.

### Listas ordenadas

São aquelas que possuem uma ordem. A tag responsável é `<ol>` que vem do inglês **ordered list**.

### Listas não-ordenadas

São aquelas que não possui uma numeração de prioridade. A tag responsável é `<ul>` **unordered list**.

### Exemplos

```htm
<h2>Minha lista do supermercado</h2>

<ul>
  <!--li significa List item -->
  <li>Queijo</li>
  <li>Ovos</li>
  <li>Frango</li>
</ul>

<h2>Minha prioridades</h2>

<ol>
  <li>ver as aulas da universidade</li>
  <li>praticar conceitos abordados</li>
  <li>criar um projeto prático</li>
</ol>
```

#### Algumas propriedades da listas

- start: Informa onde começa a lista. Usada em questão de ordem, por exemplo, se você gostaria de começar contar lista pelo 20
- type: Pode ser numeral, numeral romano ou até alfabeto
- reversed: inverte a ordenação da lista

alguns exemplos:

<ol reversed type="i" start="4">
  <li>ver as aulas da universidade</li>
  <li>praticar conceitos abordados</li>
  <li>criar um projeto prático</li>
</ol>

<ol start="20">
  <li>ver as aulas da universidade</li>
  <li>praticar conceitos abordados</li>
  <li>criar um projeto prático</li>
</ol>

<ol type="a" start="8">
  <li>ver as aulas da universidade</li>
  <li>praticar conceitos abordados</li>
  <li>criar um projeto prático</li>
</ol>

> referência: [W3c](https://www.w3schools.com/html/html_lists.asp)
