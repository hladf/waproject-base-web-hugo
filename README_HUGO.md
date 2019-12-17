teste-tecnico-web-hugo
==================

## Anotações gerais:

Fiz uma sessão a mais no menu para controlar o `estoque de produtos` (e não `pedidos` como disse no email)

Por conta dos imprevistos com bugs e o fato de não ter tido o tempo de sabado e domingo, acabei dando preferência á fazer funcionar primeiro do que caprichar no visual e fazer uma boa visualização de detalhes do produto.


### Bugs encontrados:
api: 
- `docker-compose up` estava dando problemas pra subir, que agora não recordo exatamente quais eram, mas um deles era por conta da linha de `volumes` do `docker-compose.yml` sobre acesso de usuário em uma pasta, algo do tipo, então depois de um tempo, só renomeei o original para `docker-compose_old.yml` e criei meu próprio arquivo pra subir um container postgres igual para prosseguir com o projeto.

front:
- popup de excluir item da lista não abre, nem na lista de usuários.
- faltando um `/save` no final da rota de `user.save` (arrumei no meu repo)
- no `useCallbackObservable` do `UserFormDialog` estava faltando passar o model no array (que foi consertado dia 16 por voces), por isso deu o bug que comentei no ultimo email de não estar cadastrando.
