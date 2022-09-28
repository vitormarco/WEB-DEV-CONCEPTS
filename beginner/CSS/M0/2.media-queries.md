## Media Queries

Media queries usa a @media sintaxe. Você pode fazer uma correlação com a condicional if.

Ela segue o seguinte formato:

```css
@media (max-width: 300px) {
  .small-only {
    color: red;
  }
}
```

Ou seja, se a resolução da janela está entre 0px e 300px de largura, a regra estabelecida será aplicada. <br>

### Hidden content (conteúdo escondido)

É normal usar combinação de media queries para ter interfaces alternativas, dependendo do tamanho da tela.

```html
<div class="large-screens">Eu irei aparecer apenas em telas largas.</div>
<div class="small-screens">Enquanto, eu só irei aparecer em telas menores</div>
```

```css
@media (min-width 300px) {
  .large-screens {
    display: block;
  }
  .small-screens {
    /* é uma declaração para remover elementos do processo de renderização */
    display: none;
  }
}
```

### Valid conditions

Dentro dos parentes, normalmente é utilizado _max-width_ para adicionar estilos em telas pequenas ou <br>
_min-width_ para adicionar estilos em telas maiores.

Min width e max width, podem tipicamente ser confundidas com uma declaração CSS. E isso é errado, elas são consideradas
_media feature_, não propriedades CSS.

```css
/* 🚫 Isso não é válido, pois `font-size` não pode ser uma querie */
@media (font-size: 32px) {
}
```
