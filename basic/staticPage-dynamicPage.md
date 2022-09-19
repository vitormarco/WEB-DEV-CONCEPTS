## Static Page

Toda página, independende do momento que você entra, vai carregar a mesma informação.
Página só vai precisar do html, css, JS e toda vez que entra, ela vai buscar no servidor.

**OBS.:** Aqui tecnologias como (CSS, JS, HTML) já basta para ser desenvolvido. Hospedagem simples.

## Dynamic Page

Já aqui, é diferente, ocorre um processamento no servidor, e o servidor decide o que vai te entregar naquele momento (um exemplo é o youtube)
Aqui pode funcionar das seguintes maneiras:

- o servidor te devolve um html, mas dentro do html tem algum JS que faz uma nova requisião para buscar os dados (normalmente para um API) e depois o JS monta a página com os dados atualizado;
- O servidor já faz o processamento do html e dos dados e te entrega (NextJS tem essa abordagem para SSR)

**OBS.:** Aqui, normalmente vamos ter uma tecnologia backend para fazer o uso (ex: node). Para ter um processamento a cada requisição
