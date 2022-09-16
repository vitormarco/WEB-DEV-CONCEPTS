## Combinators

São usados quando você precisa estilizar uma combinação especifica de código. <br>
Vamos imaginar que você necessita estilizar um link, ou elemento a. <br>
Você diria, bom só usar [selector](./Selectors.md), mas se fosse somente um tipo de link especifico, vamos supor, somente <br>
links de navegação do site (ex. home - sobre nós) e não os links contidos nos documentos. <br>
Talvez passou na sua cabeça usar um selector de uma classe, é funcionaria, mas em vez disso você poderia utilizar um combinator.

Vejamos um exemplo

```html
<nav>
  <a href="">Home</a>
  -
  <a href="">About us</a>
</nav>

<p>
  Hello world! You might be interested in reading <a href="">an article</a>!
</p>
```

e o css:

```css
nav a {
  color: red;
  font-weight: bold;
}
```

estamos selecionando combinando dois selectors, estamos falando para css. Selecione nav e os elementos a descendentes de nav terão <br>
seguinte estilo.

Então podemos dizer que um combinator pode ser caracter que combina multiplos selectors. No nosso exemplo, podemos dizer que <br>
o espaço em branco entre eles (nav - a) criam um selector de descendencia.

Um selector de descendencia, irá aplicar para todos os descendetes, não importa o quão profundo está a descendecia.

```html
<nav>
  <ul>
    <li>
      <a href="">Home</a>
    </li>
    <li>
      <a href="">Shop</a>
    </li>
  </ul>
</nav>
```

Nesse caso não importa se o filho de nav é ul, o que importa na regra CSS criada em cima, irá aplicar para qualquer nav <br>
que tenha como, não importa o nivel, um descendente `<a>` o estilo será aplicado.

Existe então, no CSS, uma diferença entre descendentes e filho. Podemos fazer uma referencia arvore genealogica, um level abaixo
em uma arvore genealogica é o filho, filho do filho é o neto. E assim por diante.

Mas e se queremos aplicar um estilo apenas no filho?
Bom existe outro combinator `>`

```html
<style>
  li {
    margin-bottom: 8px;
  }

  .main-list > li {
    border: 2px dotted;
  }
</style>

<ul class="main-list">
  <li>Salt</li>
  <li>Pepper</li>
  <li>
    Fruits & Veg:
    <ul>
      <li>Apple</li>
      <li>Banana</li>
      <li>Carrots</li>
    </ul>
  </li>
</ul>
<style>
  li {
    margin-bottom: 8px;
  }

  .main-list > li {
    border: 2px dotted;
  }
</style>
<ul class="main-list">
  <li>Salt</li>
  <li>Pepper</li>
  <li>
    Fruits & Veg:
    <ul>
      <li>Apple</li>
      <li>Banana</li>
      <li>Carrots</li>
    </ul>
  </li>
</ul>
```

No exemplo temos `.main-list > li` ou seja, selecionamos o selector da classe, e dizemos que queremos aplicar somente ao `filho`
da classe. Ou seja, borda só será aplicada em **salt**, **pepper** e **Fruits & Veg**. Os itens dentro de **Fruits & veg** no caso <br>
**Apple**, **Banana** e **Carrots** não terão borda.

> Aqui mostramos dois exemplo, para mais informações poderá acessar [W3C Schools](https://www.w3schools.com/css/css_combinators.asp)
> ou [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Combinators)
