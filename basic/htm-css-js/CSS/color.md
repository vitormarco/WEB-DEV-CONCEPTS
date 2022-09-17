## Color

Serve para alterar a cor textual de um elemento especifico.

```css
p {
  color: red;
}
```

### Color formats

CSS inclui diferentes maneiras de representar as cores.
A mais comum entre os desenvolvedores é hexadecimal (#FF0000).

- hexa codes (#FF0000)
- Keywords (red)
- RGB (rgb(255, 0, 0))
- HSL (0deg, 100%, 50%)

#### HSL

Parametros:

1. Visto como 'circulo' de cores
2. Saturação (quão intenso ou pigmentado é)
3. luminosidade

Podemos analisar que saturação quão mais proxima de zero, mais ela se aproxima do `cinza` e quanto mais perto de 100%, <br>mais inteso será a cor.
Já a luminosidade quanto mais próxima de 0%, mais `escura` será a cor, sendo o 0% o `preto` e quanto mais próxima de 100%, mais clara será a cor, sendo
100% o `branco`.

## Transparency

Algumas cores, nos permite adicionar um valor extra para o `alpha channel`. Ele representa a opacidade, vai de zero (0) à um (1).
Sendo o um o valor padrão, que significa que cor totalmente opaca e sólida. Já zero, a cor é invisivel. Podemos especificar um valor decimal, para criar
uma cor semi-transparente.

```html
<style>
  .box {
    width: 50px;
    height: 50px;
  }

  .box0 {
    background-color: hsl(340deg 100% 50% / 1);
  }

  .box1 {
    background-color: hsl(340deg 100% 50% / 0.75);
  }

  .box2 {
    background-color: hsl(340deg 100% 50% / 0.5);
  }

  .box3 {
    background-color: hsl(340deg 100% 50% / 0.25);
  }
</style>

<div class="box0 box"></div>
<div class="box1 box"></div>
<div class="box2 box"></div>
<div class="box3 box"></div>
```

**OBS.:** Importante não confundir a barra (/) com divisão, basicamente é um padrão moderno do CSS, que significa separação.
Essa barra nos permite criar grupos de valores. Primeiro grupo, é sobre a color (340deg 100% 50%) e segundo é sobre a opacidade (0.5).
da para usar em border-radius para separar valores horizontais e verticais. E também é utilizado em CSS GRID, quando um elemento é subdividido em multiplas linhas ou colunas.

A versão do HSL color é parte da revisão de 2016 do como as cores funcionam no CSS. Maior parte dos browsers suportam, mas no IE (Internet Explore) não irá.
Se o projeto presta suporte para IE, será então necessario uma abordagem diferente.

## Background colors

Como já vimos, a propriedade `color` apenas afeta o cor do texto. Se quisermos alterar o `fundo` do elemento, devemos utilizar
a propriedade `background-color`.

Vamos ver como funciona um efeito de marcação ou destaque no texto.

```html
<style>
  em {
    background-color: hsl(50deg 100% 50%);
  }
</style>

<p>
  This is a paragraph with a
  <em>highlighted section</em>.
</p>
```

resultado:

<p>
  This is a paragraph with a
  <em style="background-color:  hsl(50deg 100% 50%); color: black">highlighted section</em>.
</p>
