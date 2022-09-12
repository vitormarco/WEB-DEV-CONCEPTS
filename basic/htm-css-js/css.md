# Sobre CSS

Aqui iremos abordar alguns conceitos do CSS, para servir como orientação

### Property (propriedade)

São atributos que você pode especificar valores, como "color", "font-size" ou "margin"

```css
h1 {
  margin: 20px;
  color: red;
}
```

### Selector (seletores)

Seletores são o que descreve algum elemento da página, esses elementos podem ser o elemento em si, como também <br>
um id para um elemento especifico ou até mesmo uma classe para representar um ou mais elementos.

```css
/* ".apple" é um exemplo de seletor do tipo classe. Irá selecionar todos os elementos que contem class .apple */
.apple {
  background: red;
}

/* "#banana" é exemplo de seletor do tipo id. Irá selecionar somente o id especifico */
#banana {
  background: yellow;
}
/* "h1" é um elemento do html, nesse caso, ele irá selecionar todos os h1 da página e aplicar folha de estilo */

h1 {
  color: black;
}
```

### Declaration (declaração)

É a combinação de property (propriedade) e um value(valor)

```css
/* "padding" é a nossa propriedade e o 24px é nosso valor. Juntos são considerados uma declaração */
h1 {
  padding: 24px;
}
```

### Rule (regra)

Uma regra, é um coleção de declarações atribuidas para um ou mais seletores. <br>
Uma regra pode ser um conhecida como style(estilo), multiplas regras, são um stylesheet(folha de estilo)

css = cascading stylesheet (Folha de estilo em cascata)

```css
/* Nesse exemplo todo o bloco de h1 é uma rule, ou seja da linha 51 até 58 */
h1 {
  color: red;
  font-family: sans-serif;
}
```

### Unit (unidade)

Alguns valores tem unidade (como unidade de medida). Esses valores pode ser em px, %, rem ou em

```css
/* nesse caso do exemplo estamos usando px, mas poderia ser em rem 1rem = 16px ou até mesmo porcentagem */
div {
  border-radius: 16px;
}
```
