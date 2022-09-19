## Como internet funciona

Quando você acessa o navegador (browser), você pesquisa algum site, por exemplo: "www.github.com". Até então o navegador não sabe o que ele deve exibir. **Lembrando:** Navegador está em "client-side".

Então, atráves do **Dominio** (url digitada), a web faz uma requisição para o **servidor** (server-side) que está atrelado aquele dominio. O servidor, devolve o `.HTML` do dominio. No site que usamos como exemplo, possívelmente (na estrutura de pastas convencionais), existe um index.html que mostra o "home" do githhub. Mas vamos supor que exista um arquivo chamado urlGit/projetos.htlm, bom esse é uma outra resposta do servidor, para os projetos (o que muitos fazem é normalmente criar uma pasta projetos/index.html) o que também irá direcionar para dentro do arquivo (outra forma também é criar alguma especie de direcionamento para remover a extensão do arquivo, apache tem uma abordagem, o nginx outra).<br>
**OBS.:** No React (quando se utiliza o create-react-app), por exemplo, ele é um pouco diferente. Normalmente quando compila um projeto, ele gera um index.html só, isso é chamado de SPA (Single Page Application), e normalmente quem faz o que tem que ser exibido é o proprio JS. No SPA, não existiria uma estrutura de pastas como eu mencionei.
<br>

Quando então o servidor devolve o HTML para o cliente, cliente começa a ler o HTML, nessa leitura ele percebe que existe um indicativo por exemplo do CSS ou JS. Apartir disso ele pede novamente para o servidor os arquivos necessarios.

#### Site no ar

1. contratar uma **hospedagem** (digitalOcean, AWS, Azure, Heroku, netlify, Vercel etc.)
   > tu pode usar até pc da tua casa, mas não é uma boa abordagem.
2. comprar um determinado **dominio** (meusitefeliz.com, meusitefelizdaweb.net)
3. Usar um **dns** para fazer um link dos dois

#### Fluxo

Client-side -> servidor dns -> dominio

Servidor dns, é onde fica armazenado a relação ip <-> nome do dominio

github.com (nome do dominio) - 192.176.9.9 (ip) de acesso
quando cliente não sabe o dominio, normalmente ele vai fazer uma consulta no servidor dns, depois disso, essa consulta não ocorre mais.
