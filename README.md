# GraphQL

Repo para estudo sobre GraphQL

GraphQL é um conjunto de padrões para comunicar o front-end com o back-end de maneira diferente a convencional quando se faz chamadas as APIs utilizando RESTful.

Quando uma chamada ao back-end é feita utilizando o padrão RESTful, a rota determina quais dados serão retornados, o back-end tem toda responsabilidade, é encarregado em dizer ao front-end quais dados serão retornados.
Já com o GraphQL quem diz quais dados serão retornados é o front-end não o back-end.

### Problemas que GraphQL resolve:

- **Overfetching** (buscar informações demais, buscar o fetch mais do que o necessário);
    - (Ex. fazer chamada a usuários e o back-end retorna usuários e endereços, mas pode haver momentos em que houver a chamada de usuário que o endereço não é necessário).
- **Underfetching** (quando não são retornados todos os dados necessários);
    - (Ex. a rota para usuário só retorna os usuários quando precisar dos dados de endereço).

### Dificuldades:

- **Cache** por tem somente uma única rota na aplicação;
- **Erros** todas as chamadas http retornam código 200. A tratativa de erros precisa ser feita além do que o browser consegue entender;
