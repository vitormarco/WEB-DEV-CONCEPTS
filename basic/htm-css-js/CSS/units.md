## Units

A unidade mais popular é **px**. Pixels correspondem mais ou menos com aquilo que você está vendo em sua tela. 1px, é referente
mais ou menos uma unidade da tela, por exemplo um monitor full hd tem 1920px de largura por 1080px de altura.

## EMs

O `em` é uma unidade _relativa_, que é igual ao tamanho da fonte `(font-size)` do tamanho do elemento atual.<br>
(padrão de font-size na web é 16px, por isso, em possui como tamanho padrão 1em = 16px)

Exemplo:

```html
<style>
  p {
    /* Mude a fonte e veja que padding irá mudar */
    font-size: 16px;

    padding-bottom: 2em;
    border: 1px solid;
  }
</style>

<p>This paragraph has a relative amount of bottom padding!</p>
```

Outro exemplo, para fixação:

```html
<style>
  p {
    /* Change me! */
    font-size: 40px;
  }
</style>

<p>
  <span style="font-size: 1em"> This </span>
  <span style="font-size: 0.8em"> sentence </span>
  <span style="font-size: 0.64em"> gets </span>
  <span style="font-size: 0.5em"> quieter </span>
  <span style="font-size: 0.4em"> and </span>
  <span style="font-size: 0.32em"> quieter </span>
</p>
```

`EM` não são muito utilizados. Usa-los significa que UI irá mudar dependendo do tamanho da fonte, isso pode ser útil em alguns casos,
mas na maioria dos casos vai ser irritante. O `rem` acaba sendo mais útil, na maior parte das circunstancias.

## REMs

O `rem` é parecido com `em`, com uma diferença crucial: ele sempre é relativo ao elemento root, ou seja, tag <html>.
Como foi comentando antes, a tag html tem como tamanho de fonte padrão 16px, então 1rem é igual 16px.

Ou seja, `rem` acaba sendo mais consistente do que o `em`, pois respeita as preferencias do usuário quando o mesmo diminui ou aumenta o tamanho padrão da fonte.

**Obs.:** Não altere o tamanho padrão em px na tag html. Pois isso irá sobrescrever as escolhas do usuário.
Maneira correta seria alterar atráves da porcentagem `(%)`

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>

    <style>
      /* 🚫 Maneira errada */
      html {
        font-size: 24px;
      }

      /* ✅ Maneira correta */
      html {
        font-size: 150%;
      }
    </style>
  </head>
  <body>
    <p>Exemplo</p>
  </body>
</html>
```

> Se não está afim de fazer calculos, recomendo o seguinte site que faz [conversão](https://nekocalc.com/px-to-percentage-converter)

## Percentages

A porcentagem normalmente é usada com largura e altura, pois consome um porção do espaço livre.

```html
<style>
  .box {
    width: 250px;
    height: 250px;
    background-color: pink;
  }

  .child {
    width: 50%;
    height: 75%;
    background-color: black;
  }
</style>

<div class="box">
  <div class="child"></div>
</div>
```

No exemplo, criamos uma div pai, e uma div filho. A div pai tem um tamanho de 250x250px, e a filho 50% da largura e 75% da altura.
Se o tamanho do pai mudar, então filho irá mudar também. No nosso exemplo o filho está com 125x187.5 px.

> Se vocês estiver com alguma dúvida de como e quando utilizar cada medida, recomendo leitura desse [artigo](https://www.joshwcomeau.com/css/surprising-truth-about-pixels-and-accessibility/)
