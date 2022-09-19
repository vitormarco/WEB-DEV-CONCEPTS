## Client-side vs Server-side

São abordagem de como determinado código é executado na web.

### Client-side

É tudo aquilo que é usado na máquina local do cliente, ou seja, seu tempo de execução está somente atrelado a máquina do cliente.
Normalmente é a responsividade, algum calculo de interação do usuário (por exemplo, abrir o menu lateral, adicionar itens no carrinho de compra).

### Server-side

É tudo aquilo que é usado no nivel do servidor. Normalmente é uma operação que tem que permitir uma persistencia, e que o usuário não pode ter acesso. Por exemplo, se você que transferir um dinheiro para um amigo, você não deveria ter acesso a conta do seu amigo (somente a sua). E você também não deveria alterar manualmente os dados (se não você poderia adicionar 1 trilhão na conta).

Quem vai fazer as operações de quanto realmente usuário tem de dinheiro, a transferencia de uma conta para outra é o servidor.

Para transferir o dinheiro para seu amigo, no momento que tu seleciona uma quantia e aperta confirmar, isso vai para o servidor, o servidor vai validar a quantia e "conectar" com conta do teu amigo, enviando assim o valor e persistindo que você retirou uma quantida X e seu amigo ganhou uma quantia X.

### Desenvolvedores

#### Front-end

- "Client-side"
- UX
- UI
- Responsividade
- Uso em N navegadores
- layout
- animações
- integração com backend (fazer as chamadas e tratar as respostas)

#### Back-end

- "Server-side)
- Persistência dos dados
- Regra de negócio
- Algoritmos complexos (analisa, transformações de imagem, Processamento de dados)
- Performance (como se comporta com x usuários acessando o sistema)
- Acesso ao BD.
- Escalabilidade
