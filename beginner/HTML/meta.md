## Meta

Tag referente aos metadados (informação sobre os dados). É utilizada também dentro da tag `<head>`.
Suas funções são:

- conjunto de caractres disponíveis (por exemplo, para reconhecer acentos, normalmente no Brasil, usamos UTF-8)
- descrição da página, é o responsável por colocar um descritivo quando compartilha o link ou quando você pesquisa uma determinada coisa
- keywords (palavras-chaves)
- author do documento
- configurações de viewport

**Não é visivel na tela do usuário, mas sim para percepções da máquina**

```html
<!DOCTYPE html>
<html>
  <head>
    <meta name="keywords" content="HTML, CSS, JavaScript" />

    <meta name="description" content="Free Web tutorials for HTML and CSS" />

    <meta name="author" content="John Doe" />

    <meta http-equiv="refresh" content="30" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  </head>
</html>
```

São tagas conhecidas como self closing

> Referencia [W3C](https://www.w3schools.com/tags/tag_meta.asp)
