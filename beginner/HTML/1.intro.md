## HTML

Surgimento do HTML veio com uma necessidade de compartilhar de forma fácil documentos dentro das instituições.
Antes do html, o computador não entendia de forma clara cada bloco em um texto.

Exemplo:

_Maneira como você enxerga_

Minhas Férias <br>

Eu passei as férias com minha família. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum aliquet diam neque, at venenatis elit accumsan eu. Nunc sed ex quis risus vestibulum blandit id a nulla. Integer purus risus, rhoncus a justo a, iaculis luctus est. Integer ac quam ut ipsum eleifend auctor ac sed est. Maecenas vel sodales justo, at hendrerit metus. Sed ipsum purus, efficitur sagittis facilisis in, scelerisque a eros. Pellentesque quis arcu lobortis eros pretium laoreet. <br>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum aliquet diam neque, at venenatis elit accumsan eu. Nunc sed ex quis risus vestibulum blandit id a nulla. Integer purus risus, rhoncus a justo a, iaculis luctus est. Integer ac quam ut ipsum eleifend auctor ac sed est. Maecenas vel sodales justo, at hendrerit metus. Sed ipsum purus, efficitur sagittis facilisis in, scelerisque a eros. Pellentesque quis arcu lobortis eros pretium laoreet.<br>

Você consegue ler de forma simples esse texto, dizer o que é o titulo e o que são os parágrafos.

_Maneira como o computador enxerga_

Minhas Férias Eu passei as férias com minha família. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum aliquet diam neque, at venenatis elit accumsan eu. Nunc sed ex quis risus vestibulum blandit id a nulla. Integer purus risus, rhoncus a justo a, iaculis luctus est. Integer ac quam ut ipsum eleifend auctor ac sed est. Maecenas vel sodales justo, at hendrerit metus. Sed ipsum purus, efficitur sagittis facilisis in, scelerisque a eros. Pellentesque quis arcu lobortis eros pretium laoreet. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum aliquet diam neque, at venenatis elit accumsan eu. Nunc sed ex quis risus vestibulum blandit id a nulla. Integer purus risus, rhoncus a justo a, iaculis luctus est. Integer ac quam ut ipsum eleifend auctor ac sed est. Maecenas vel sodales justo, at hendrerit metus. Sed ipsum purus, efficitur sagittis facilisis in, scelerisque a eros. Pellentesque quis arcu lobortis eros pretium laoreet.

Para o computador, tudo é uma sequência de texto, ele não conseguia diferenciar o que era o título e os seus parágrafos.

Como isso veio a implementação do html e suas **tags**.

## Tags

Uma tag vem do inglês que significa etiqueta. Então a ideia é que cada parte do texto tenha uma etiqueta que você consegue dizer para o computador o que cada coisa significa.
No nosso exemplo, o título seria uma tag de título e os parágrafos uma tag de parágrafo.

Formato dessa tag é o seguinte `<NOME_TAG>TEU_CONTEÚDO</NOME_TAG>`.

O `<NOME_TAG>` é uma tag de abertura, que indica que apartir daquele ponto começa uma determinada TAG.

E `</NOME_TAG>` é uma tag de fechamento, que indica que naquele ponto uma determinada tag que foi aberta se encerra.

No momento que tempos uma **tag de abertura** + **conteúdo** + **tag de fechamento** temos como resultado um _Elemento HTML completo_

Exemplo:

```html
<p>O meu primeiro parágrafo</p>
```

#### Dicas

um comentário no html da para ser utilizado como `<!-- aqui o comentário -->`
