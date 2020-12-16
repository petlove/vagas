# Teste Técnico - BI/Analytics

## Contexto

A **Petlove** é a maior plataforma voltado para os pets da América Latina. Cuidando de todo o fluxo do pai/mãe de pet, desde com abastecimento de produtos (via e-commerce [aqui](https://www.petlove.com.br/)), junto com o cuidado do veterinário (via [Vet Smart](https://www.vetsmart.com.br/)), garantindo um ERP e sistema de gestão adequado (via [Vetus](https://vetus.com.br/)) ou fornecendo serviços como passeios ou pet sitter (via [DogHero](https://www.doghero.com.br/)).

Tendo em vista esse cenário tão diverso, a área de Dados do grupo Petlove criou squads com pessoas que possuem habilidades diferentes para ajudar cada frente de negócios a terem entregas melhores. 

Seu desafio vai ser participar do time de **Assinatura**: um serviço que o pai/mãe de pet contrata um conjunto de itens para receber na frequência que desejar, pagando uma assinatura no período selecionado pelo cliente (e recebendo um desconto ao contratar o serviço).

 

## Problema

O time de assinatura tem uma meta para reduzir o churn dos assinantes. Contudo, nos últimos três meses, apesar de todas as melhorias de usabilidade da plataforma o churn vem sendo cada vez maior nos assinantes, como apontado abaixo:

![Churn Progress Over Time](./materials/churn.png)

Seu **desafio** será ajudar o time de produto e negócios a **REDUZIR** o churn com uma análise de dados dos assinantes e não assinantes, propondo: *Aprendizados* e *Próximos Passos*. Ou seja, o resultado final PRECISA ser um material que apresente esses dois pontos e fique claro para todos, desde o diretor da empresa até o time de tecnologia que vai ver sua apresentação.

Lembrando que definimos o **churn** aqui em todos os usuários que cancelaram a assinatura naquele período.

## Ferramentas

Segue as ferramentas que usamos e que SUGERIMOS que você utilize para continuar no processo seletivo:

1. **Python/Jupyter Notebooks/SQL** para quando é necessário código;
2. **PowerPoint/Google Slides** para apresentar os resultados para o time externo;
3. **GitHub** como repositório para armazenar os códigos e algumas - pequenas - documentações. 

## Materiais

O time de engenharia de dados forneceu uma prévia dentro de um SQLite com os dados mais úteis para você. Esse material já vai ser suficiente para você tirar os insights necessários, segue a estrutura básica:

| tables             | description                                                                                        |
|--------------------|----------------------------------------------------------------------------------------------------|
| subscribers        | Tabela que contém todas as assinaturas, cobranças e inícios.                                       |
| users              | Dados dos usuários, clientes e outros detalhes do sistema.                                         |
| orders             | Tabela transacional com todos os pedidos, efetivados ou não.                                       |
| orders_line_items  | Tabela com os detalhes transacionais, só que abrindo em detalhes de quais itens foram contradados. |
| itens_sku          | Dados em detalhes de cada produto, segmentação, família e afins.                                   |
| events_platform    | Tabela com TODOS os eventos do grupo, Petlove como as outras empresas.                             |
| subscribers_cohort | Tabela simplificada para fazer o devido cálculo de cohort.                                         |
| marketing_channel  | Referências de todos os canais e subcanais tagueados pelo time de marketing.                       |
<br>

Aqui é um diagrama da documentação providenciado pelos arquitetos de como você pode conectar as tabelas, para facilitar sua análise:

*[COLOCAR UMA IMAGEM DO DIAGRAMA DO SQLITE]*

## Entrega Final e Critérios

O que é esperado que você entregue dentro do período do teste:

1. **Códigos:** seja em python/notebook ou sql, para entender como foram calculados os gráficos e insights;
2. **Documentação técnica:** de preferência um README com markdown, para explicar a lógica dos códigos mais detalhada;
3. **Apresentação final:** podendo ser em formato PDF ou PPTX, com todos os insights para resolver o problema.

Os **critérios de avaliação** serão:

1. **Storytelling/Oratória:** quão fácil foi para você explicar os conceitos? Os insights ficaram explícitos e os resultados da análise ficaram claros após apresentação?
2. **Qualidade do Código:** avaliar a performance e facilidade na leitura/compreensão no conteúdo. Algumas referências para nós são: Para código no geral ([aqui](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)), para o python em si ([aqui](https://google.github.io/styleguide/pyguide.html)) e para o SQL em si ([aqui](https://about.gitlab.com/handbook/business-ops/data-team/platform/sql-style-guide/));
3. **Documentação:** o material possui uma documentação clara de como você chegou nos cálculos? Um README adequado para explicar a análise ou resultados finais? Lembrando que é importante ter uma documentação TÉCNICA para entender o código e, caso alguém de outro squad veja seu material, possa seguir seus passos para chegar nos mesmos resultados;o,
4. **Visualização**: gráficos fáceis de entender, com eixos explícitos e aprendizados no material para simplificar a compreensão do time de negócios. Lembrando que aqui NÃO SERÁ AVALIADO o design no sentido ARTÍSTICO, mas se ele é funcional para a análise, sem atrapalhar a compreensão;
5. **Próximos Passos:** as ações necessárias para serem executadas após a conclusão da análise são úteis? E resolvem as dores do time de negócio? Os próximos passos ficaram claros para todos durante a apresentação?

**OBSERVAÇÕES:** NÃO será avaliado nenhum modelo estatístico de previsão do churn. Caso você queira produzir algo, fique à vontade. Mas a PRIORIDADE será a análise e o material final para o time de negócios/produto.
