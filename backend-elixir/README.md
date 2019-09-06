# Desafio de código Backend Elixir

O objetivo deste exercício é analisar sua familiaridade com Elixir e capacidade
de tirar proveito do poder da linguagem para executar uma tarefa.

Boa sorte e obrigado por participar!

### Desafio Rick and Morty: Most dimensional character ranking

  - Como fãs de [Rick and Morty](http://www.adultswim.com/videos/rick-and-morty/),
  gostaríamos de uma API que nos ofereça algumas informações sobre os personagens.
  Nesse desafio, a proposta é que você desenvolva uma API que retorne um
  ranking dos personagens que mais tem "doppelgangers", ou seja, personagem que
  tem mais versões diferentes dele em outros universos.

  Para isso, você precisará consultar a base de personagens e os locais em que
  ele aparece para descobrir.
  Essas informações estão disponíveis na
  (Rick and Morty API)[https://rickandmortyapi.com].

  O retorno esperado da sua API pode ser algo como:
  ```json
  [{
    "character": "Rick",
    "image": "http://image_url",
    "dimensions_count": 10
  },
  {
    "character": "Morty",
    "image": "http://image_url",
    "dimensions_count": 6
  }]
  ```

  ![rickandmorty](https://user-images.githubusercontent.com/463350/64463152-80053a00-d0f2-11e9-8996-7a360ea343f4.gif)

## Requisitos

  * Você precisa buscar essas informações na API para alimentar uma base local,
    com um modelo de dados que atenda o propósito do desafio;
  * Disponibilizar um endpoint para consulta dessas informações, fazer ordenação
  e filtrar, etc;
  * Crie uma rotina que faça a atualização da sua base de dados 3 vezes ao dia;
  * Precisamos de uma documentação da sua API para utilizar. Pense em utilizar
    o [Swagger](https://swagger.io/);
  * Não esqueça de desenvolver os testes;
  * Vale observar que a Rick and Morty API tem uma limitação de requisições por
    dia, que está disponível em sua
   [documentação](https://rickandmortyapi.com/documentation).


## Regras
  * Por favor, tente resolver o teste sem ajuda de ninguém. Lembre-se de que
  discutiremos a solução pessoalmente;
  * Utilizar [Phoenix](https://phoenixframework.org/) para construir API;
  * Pode utilizar o banco de dados que quiser para fazer o teste;
  * Se a aplicação tiver alguma complexidade extra para instalar/executar incluir
  no README.md as instruções para setup;
  * Vamos avaliar principalmente o que foi proposto para o exercício,
  mas se não conseguir conter sua criatividade e quiser incrementar a aplicação,
  fique a vontade, mas não deixe de entregar o essencial ;) .

## Entrega do projeto

- Crie uma aplicação nova para executar o desafio;
- Ao finalizar, suba a sua proposta para o projeto que você criou no GitHub
Exemplo: https://github.com/seuNome/pet-code;
- Envie-nos o link do projeto. Exemplo: https://github.com/seuNome/test-elixir.git
- Pronto! Basta aguardar o nosso RH entrar em contato. Entramos em contato rapidinho ;)
