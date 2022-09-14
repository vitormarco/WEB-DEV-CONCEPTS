## Pseudo-classes

Pseudo-classes são elementos do css que ajudam aplicar uma pedaço de css baseado no estado do Elemento

### Hover

Utilizado quando o mouse passa por cima de algo, assim que mouse passa ele aplica algum estilo.

```css
button:hover {
  color: blue;
}
```

Nesse exemplo, quando passar o mouse por cima de um elemento botão, ele irá trocar a cor do texto para **blue**

### Focus

Alguns elementos que possui intereção como button, links e inputs. Quando interagimos com eles (clicando ou no tab) <br>
estado dessa interação é o focus.

```css
button:focus {
  border: 2px solid blue;
  background: blue;
  color: white;
}
```

### Checked

Essa pseudo-class apenas é utilizada para checkbox e radio buttons que são marcados.

```css
input:checked {
  width: 24px;
  height: 24px;
}
```

```html
<h1>Pizza Toppings</h1>
<br />
<label>
  <input type="checkbox" />
  Avocado
</label>
<br />
<label>
  <input type="checkbox" />
  Broccoli
</label>
<br />
<label>
  <input type="checkbox" />
  Carrots
</label>
```

> Uma lista completa de [pseudo-classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
