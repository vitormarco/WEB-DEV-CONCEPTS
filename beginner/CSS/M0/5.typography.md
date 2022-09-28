## Typography

O texto é o aspecto mais importante da web. Remova o texto da página, e virá ser totalmente inútil a página web.
Isso não é verdade sobre imagens, cores ou estilo. (think about)

### Font families

Podemos mudar qual a fonte ser usada em uma página web através da **propriedade** `font-family`:

```css
font-family: Arial;
```

É chamado de _family_ porque cada font consiste de múltiplos caracteres de definição:
Por exemplo _"Roboto"_ inclui 12 definições individuais: 6 font weights com 2 variações (normal e itálico)

Há algumas fonts chamadas "web safe fonts", ou fontes seguras da web, isso significa que existe uma variedade de fontes
pré instaladas na maior parte dos sistemas operacionais como por exemplo:

- Arial
- Times New Roman
- Tahoma

Família de fontes vem com diferentes estilos, os mais populares São:

- Serif
- Sans-serif
- Monospace

Se nós quisermos, podemos deixar o SO (Sistema Operacional) decidir qual fonte pegar para cada estilo

```css
/* value podem ser 'sans-serif' ou 'monospace para escolher uma font pelo sistema*/
p {
  font-family: serif;
}
```

podemos também instalar uma font e usar, por exemplo:

```css
font-family: "Roboto", sans-serif;
```

Nesse exemplo, estamos dizendo para usar a `Roboto`, uma font do google, caso não consiga utilizar a próxima fonte na tomada de decisão
vai ser uma sans-serif escolhida pelo SO.

### Formatação de texto mais comuns

Softwares de processamento de texto como `Google docs` ou `Microsoft Word`, disponibilizam um conjuto grande de maneiras de formatar o texto.
E o CSS também, contudo iremos focar em 3 dessas maneiras:

- Bold
- Italic
- Underline

### Bold text

Criamos um texto em negrito com esse valor, e atribuímos a propriedade `font-weight`

```css
font-weight: bold;
```

Também podemos usar a forma numérica que vai de 1 a 1000, sendo um o peso mais fraco e 1000 o mais forte.

```css
/* Textos mais 'leves' ou 'thin text', textos finos */
font-weight: 300;

/* Peso normal das fontes */
font-weight: 400;

/* Famoso bold */
font-weight: 700;
```

#### Italic text

Normalmente usamos quando queremos dar um enfase em alguma parte do texto. Na web, normalmente essa ênfase é uma inclinação em ângulo.
O texto em ângulo, sugere que as palavras estão sendo 'inclinadas'.

```css
font-style: italic;
```

#### Underline text

Na web, `underline` tem como função algo extremamente específico: informar que existe um link.

Não devemos, usar como efeito visual ou algo para destacar algo importante, pois irá confundir o usuário.

Alocamos esse tipo de estilo com a propriedade `text-decoration`:

```css
a {
  text-decoration: none;
}
```

### Alignment

Outro processamento de texto bastante conhecido é o alinhamento.
O responsável no CSS por fazer isso é a propriedade `text-align`

```css
p {
  text-align: left;
}

p {
  text-align: right;
}

p {
  text-align: center;
}
```

`text-align` é capaz de alinhar outros elementos, como por exemplo, as imagens. Mas no geral, iremos utilizar outras abordagens.
Devemos deixar `text-aling` somente para textos.

### Text Transforms

Podemos ajustar a formatação do texto usando a propriedade `text-transform`.

```css
/* Irá renderizar tudo com caixa alta */
text-transform: uppercase;

/* Irá deixar somente primeira letra com caixa alta */
text-transform: capitalize;
```

Por que utilizar? Bom é aconselhável usar esta propriedade CSS para que mantemos a caixa "original".
No futuro, caso editemos o html, talvez seja necessário a remoção da caixa alta em tudo por exemplo.
Se tivéssemos editado o HTML, teríamos que identificar cada instância do texto e alterar. Já com css, só precisamos remover em um lugar.

### Spacing

Podemos ajustar o espaçamento de duas maneiras:

1. aumentar o espaçamento entre os caracteres de forma horizontal com a propriedade `letter-spacing`
2. aumentar a distancian entre a linhas de forma vertical usando a propriedade ``line-height`

```css
h3 {
  letter-spacing: 3px;
  line-height: 2;
}
```

<!-- Um pouco confuso, melhorar -->

`line-height` é um pouco estranho, pois não leva unidade no valor. <br>
Isso funciona com uma proporção `line-height: 2;` significa que vai ser duas vezes mais alta que um elemento com altura 1.

⚠️ No objetivo de tornar os websites mais acessível possível, devemos sempre escolher um valor generoso para `line-height`. Pois isso
ajuda a melhorar a experiência daqueles com dificuldade de visão, assim como dificuldades cognitivas como a dislexia.

Podemos passar uma unidade para line-height como no exemplo abaixo:

```css
p {
  line-height: 20px;
}
```

Mas no geral, não devemos fazer isso. Pois se o usuário aumentar o tamanho da fonte, como já vimos, queremos manter as alturas com dimensão proporcional.

#### In React

Se você está usando JSX, tome cuidado.
Se por algum acaso usar inline-styles e não passar uma unidade, o React irá assumir como pixel o default

```jsx
function SomeComponent() {
  return <p style={{ lineHeight: 24 }}>Hello World</p>;
}
render(<SomeComponent />);
```

será 24px, e como dito, devemos evitar essa prática
