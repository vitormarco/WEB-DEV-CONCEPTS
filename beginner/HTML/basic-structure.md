## Estrutura básica

Para um juiz ler um processo ou médico ler um laudo, e entender as questões técnicas, eles precisam ter cursado suas
respectivas faculdades. Para o navegador, ele precisa "saber" o que ele está lendo, quando entra em um arquivo. Primeira
coisa é a extensão (.html), logo após, precisamos indicar qual versão do html esse arquivo está.

Isso se dá pelo seguinte código no topo do nosso arquivo:

```html
<!DOCTYPE html>
```

Seguinte código, indica para o navegador que ele está lendo um arquivo html na versão 5. **Essa declaração não é case sensitive**

> Caso você se depara com uma outra estrutura, significa que está em uma versão inferior [Older HTML Documents](https://www.w3schools.com/tags/tag_doctype.asp)

logo após essa versão, toda página conterá no minimo 3 dos elementos a seguir

```html
<html lang="pt-BR">
  <head></head>

  <body></body>
</html>
```

### html tag

Essa tag é responsável por indicar o inicio dos códigos html e o fim. Sempre importante adicionar atributo `lang` nessa tag,
para auxiliar os motores de busca.

O lang é constituído de `ISO 639-1` códigos de linguagem como `pt, en, fr e de` que significa Português, Inglês, Francês e Alemão.
E também é constituído pelo `ISO` código do país. Por exemplo, `BR e US`. Para códigos como `fr-FR` pode ocultar o código do país.
Mas no caso do Brasil ou Estados Unidos por exemplo, deve adicionar o país referência para linguagem porque somente `pt` significa que é de portugal.

> referencia [W3C html tag](https://www.w3schools.com/tags/tag_html.asp)

### Head

Tudo o que o navegador precisa saber para carregar a página correta. Ou seja onde vai os metadata (dados sobre dados).
tipicamente definem titulo do documento, conjunto de caracteres permitido, styles, scripts e outras meta informações.

> referencia [W3C head tag](https://www.w3schools.com/tags/tag_head.asp)

### Body tag

Tudo que o navegador precisa exibir para o usuário. Só pode ter um `body`.

> referencia [W3C body tag](https://www.w3schools.com/tags/tag_body.asp)

HTML segue uma hierarquia, body e head são filhas da tag html. Mas body e head são tags irmãs.
