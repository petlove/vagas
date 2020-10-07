# Desafio de código Backend Ruby

O objetivo deste exercício é analisar sua familiaridade com a plataforma Rails,
atendendo um caso de uso com os recursos de modelagem e validação que o framework oferece.
Por favor, tente resolver o teste sem ajuda de ninguém. Lembre-se de que discutiremos a
solução pessoalmente.

Boa sorte e obrigado por participar!

### Cenário: Você precisa escrever uma aplicação para gestão de animais.

  - Pessoas tem animais, e animais tem tipos.
  - Uma pessoa tem os atributos nome, documento e data de nascimento.
  - Um animal tem  os atributos nome, custo mensal e tipo.

## Regras

  - Pessoas podem ter vários animais
  - Pessoas devem ter mais de 18 anos para ter andorinhas
  - Pessoas que tenham nome começando com a letra "A" não podem ter animais do tipo Gato
  - Pessoas que já tiverem custos com animais acima de 1000 não podem ter mais animais

## Informações para popular o sistema

Crie um seed para popular o banco de dados de acordo com os dados abaixo:

### Pessoas

| NOME            | DOCUMENTO | DATA DE NASCIMENTO       |
|-----------------|-----------|--------------------------|
| Johnny Cash     | 555555555 | 26 de fevereiro de 1932  |
| Sid Vicious     | 555555555 | 10 de maio de 1957       |
| Axl Rose        | 555555555 | 6 de fevereiro de 1962   |
| Joey Ramone     | 555555555 | 19 de maio de 1951       |
| Bruce Dickinson | 555555555 | 7 de agosto de 1958      |
| Kurt Cobain     | 555555555 | 20 de fevereiro de 1967  |
| Elvis Presley   | 555555555 | 17 de agosto de 2008     |

### Animais

| NOME                   | CUSTO MENSAL | TIPO         | DONO            |
|------------------------|--------------|--------------|-----------------|
| Pé de Pano             |  199,99      | Cavalo       | Jhonny Cash     |
| Rex                    |  99,99       | Cachorro     | Sid Vicious     |
| Ajudante do Papai Noel |  99,99       | Cachorro     | Axl Rose        |
| Rex                    |  103,99      | Papagaio     | Joey Ramone     |
| Flora                  |  103,99      | Lhama        | Bruce Dickinson |
| Dino                   |  177,99      | Iguana       | Kurt Cobain     |
| Lassie                 |  407,99      | Ornitorrinco | Elvis Presley   |


## Questões

As questões devem ser respondidas com queries do `ActiveRecord`.
Inclua os trechos de código que respondem as perguntas abaixo:

### Qual é o custo médio dos animais do tipo cachorro?

    2.6.0 :007 > Animal.dogs_cost_average
   (0.9ms)  SELECT AVG("animals"."mensal_cost") FROM "animals" WHERE (animal_type = 'Cachorro')
 => 0.9999e2

### Quantos cachorros existem no sistema?

    2.6.0 :002 > Animal.dogs_count
   (1.5ms)  SELECT COUNT(*) FROM "animals" WHERE (animal_type = 'Cachorro')
 => 2 

### Qual o nome dos donos dos cachorros (Array de nomes)

    2.6.0 :001 > Person.dogs_owners_name
   (1.1ms)  SELECT "people"."name" FROM "people" INNER JOIN "animals" ON "animals"."person_id" = "people"."id" WHERE (animals.animal_type = 'Cachorro') ORDER BY "people"."name" ASC
 => ["Axl Rose", "Sid Vicious"]

### Retorne as pessoas ordenando pelo custo que elas tem com os animais (Maior para menor)

    2.6.0 :002 > Person.mensal_cost_order
   (2.9ms)  SELECT "people"."name", SUM(animals.mensal_cost) FROM "people" INNER JOIN "animals" ON "animals"."person_id" = "people"."id" GROUP BY "people"."name" ORDER BY SUM(animals.mensal_cost) DESC, name
 => [["Elvis Presley", 0.40799e3], ["Johnny Cash", 0.19999e3], ["Kurt Cobain", 0.17799e3], ["Bruce Dickinson", 0.10399e3], ["Joey Ramone", 0.10399e3], ["Axl Rose", 0.9999e2], ["Sid Vicious", 0.9999e2]] 

### Levando em consideração o custo mensal, qual será o custo de 3 meses de cada pessoa?

    2.6.0 :001 > Person.three_month_mensal_cost
   (1.7ms)  SELECT "people"."name", SUM(animals.mensal_cost)*3 FROM "people" INNER JOIN "animals" ON "animals"."person_id" = "people"."id" GROUP BY "people"."name" ORDER BY (SUM(animals.mensal_cost)*3) DESC, name
 => [["Elvis Presley", 0.122397e4], ["Johnny Cash", 0.59997e3], ["Kurt Cobain", 0.53397e3], ["Bruce Dickinson", 0.31197e3], ["Joey Ramone", 0.31197e3], ["Axl Rose", 0.29997e3], ["Sid Vicious", 0.29997e3]]

# Entrega do projeto

- Crie uma aplicação Rails nova para executar o desafio. Pode escolher o banco de dados de preferência.
- Ao finalizar, suba a sua proposta para o projeto que você criou no GitHub. Exemplo: https://github.com/seuNome/pet-code;
- Envie-nos o link do projeto. Exemplo: https://github.com/seuNome/test-backend-ruby.git
- Pronto! Basta aguardar o nosso RH entrar em contato. Entramos em contato rapidinho ;)
