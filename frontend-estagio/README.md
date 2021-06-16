# Desafio Front-end (Estágio)

Objetivo deste teste é avaliar seus conhecimentos básicos em front-end.

## O Desafio

Criar um formulário responsivo simples para consulta de CEP com Javascript, usando a resposta de uma API :)


![Petlove](https://github.com/petlove/code-challenge/blob/master/frontend/layout_final.gif)

## Endpoint

GET -> response no formato JSON

`https://viacep.com.br/ws/{{CEP}}/json/`

**Exemplo de request**

`https://viacep.com.br/ws/04571010/json/`

**Resposta do endpoint**

```
{
 cep: "04571-010",
 logradouro: "Avenida Engenheiro Luiz Carlos Berrini",
 complemento: "até 1405 - lado ímpar",
 bairro: "Cidade Monções",
 localidade: "São Paulo",
 uf: "SP",
 unidade: "",
 ibge: "3550308",
 gia: "1004"
}
```

## Instruções


### Client Side

- O formulário deve seguir o layout sugerido e conter um input e um botão de submit.

- Ao digitar o CEP no input e clicar no botão "Buscar CEP", consultar a API de CEP utilizando uma requisição e mostrar o resultado na tela.

- Os resultados a serem exibidos são: cep, uf, localidade, logradouro.

## Layout inicial
![Petlove](https://github.com/petlove/code-challenge/blob/master/frontend/layout_tela-inicial.png)

## Layout final
![Petlove](https://github.com/petlove/code-challenge/blob/master/frontend/layout_tela-final.png)


## O que posso usar?

- Você pode usar qualquer framework JS que quiser.
- Para o lado do cliente, gostamos do Vue JS e React! Se preferir, pode fazer usando Vanilla JS :)

## Readme com instruções

- Crie um Readme com as instruções de como executar seu projeto

## O que apreciamos

- Feedbacks visuais para o usuário (alertas, inputs...);
- HTML semântico;
- CSS bem estruturado
- Código limpo e bem organizado;

## Quem buscamos

Queremos uma pessoa que gosta do que faz, que trabalhe em equipe e tenha vontade de inovar. Sempre buscando aprender mais trazendo soluções inovadoras.

Se você se identificou, venha fazer parte da nossa matilha!
