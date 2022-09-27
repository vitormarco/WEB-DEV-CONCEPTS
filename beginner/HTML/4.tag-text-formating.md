## Tag de formatação de texto

### `<b></b>`

Responsável por colocar uma determinada palavra em negrito

### `<strong></strong>`

Efeito visual semelhante a tag `<b>`, contudo, na questão de semântica, significa que você gostaria de dar um pouco
mais de “importância” para os mecanismos de busca.

### `<i></i>`

Responsável por colocar o texto em itálico

### `<em></em>`

Mesmo efeito visual do itálico, contudo, dá ênfase ao conteúdo na questão semântica. Importante para os mecanismos de buscas

### `<mark></mark>`

Você "marca" o texto, como se fosse com um "marcador de texto".

### `<small></small>`

Deixa o texto menor, como se fosse um "nota de rodapé"

### `<sub></sub>`

desce o nível da linha

### `<sup></sup>`

Sobe o nível da linha

### `<del></del>`

Quando utilizar para uma errata

### `<ins></ins>`

Um dado foi inserido

### Exemplo

```htm
<!DOCTYPE html>
<html>
  <head>
    <title>Minha Página</title>
    <meta charset="utf-8" />
  </head>

  <body>
    <p>
      A área <small><sub>2</sub></small> de <strong>T.I</strong> foi uma das que
      mais cresceram nos últimos anos. Os serviços de
      <mark>tecnologia da informação</mark>, mais que dobraram de tamanho, com
      cerca de <del>95,6%</del> <ins>97,6</ins>, de acordo com o <em>IBG</em>
    </p>

    <h2>
      2<sup><small>2</small></sup
      >=4
    </h2>
  </body>
</html>
```

### Breakline

Como talvez você tenha percebido, por mais que nosso exemplo tenha uma quebra, na prática o navegador exibe o espaço que ele conseguir ocupar.
Bom a tag responsável por "forçar" uma quebra, é o `<br>` (uma tag de auto fechamento breakline)

```html
<p>
  A área 2 de T.I foi uma das que mais <br />
  cresceram nos últimos anos. <br />
  Os serviços de tecnologia da informação, <br />
  mais que dobraram de tamanho, com cerca <br />
  de <del>95,6%</del> <ins>97,6</ins>, de acordo com o <em>IBG</em>
</p>
```

tips: Não usar vários brs seguidos para aumentar o espaço de linha '-' <br>
text <br>
`<br>`<br>
`<br>`<br>
text
