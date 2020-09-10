# Desafio de Java + JSF + Primefaces + Hibernate

Esse teste foi desenvolvido para testar seus conhecimentos em Java, Maven, JSF, Primefaces e Hibernate.
Por favor, tente resolver o teste sem ajuda de ninguém. Lembre-se de que discutiremos a
solução pessoalmente.

Boa sorte e obrigado por participar!

### Cenário: Precisamos desenvolver um sistema de gestão para um pequeno pet shop, esse sistema deve controlar

  1. Usuários: você deve criar o cadastro, com nome, e-mail e senha
  2. Proprietário: Cadastro completo, com dados pessoais e endereço
  3. Animais: Nome, data de nascimento, raça, espécie e proprietário
  4. Serviços: Descrição do serviço e valor de venda
  5. Agenda: Criar agendamento com os dados do animal, proprietário, serviço e horário

## Regras

  - Você pode gerenciar as dependências e build com gradle ou maven coloque um README com as instruções para rodar o projeto
  - O projeto pode ser em qualquer IDE: Eclipse, Intellij ou Netbeans (Amamos o Eclipse S2)
  - Banco de dados a seu critério, damos preferência para PostgreSQL
  - Você deve usar Hibernate, da versão 5 para cima
  - Somente para o cadastro de clientes é obrigatório o desenvolvimento do frontend com primefaces
  - Abuse de annotations, não gostamos de XMLs

## Informações para popular o sistema

Crie um script para popular o banco de dados de acordo com os dados abaixo:

### Serviços

Descrição: Banho
Valor: R$ 50,00

Descrição: Tosa
Valor: R$ 50,00

Descrição: Consulta Clínica
Valor: R$ 100,00

### Agendamentos

Proprietário: Sid Vicious
Animal: Rex
Serviço: Banho
Data: Hoje as 15:00

Proprietário: Sid Vicious
Animal: Rex
Serviço: Tosa
Data: Hoje as 15:30

Proprietário: Axl Rose
Animal: Ajudante do Papai Noel
Serviço: Tosa
Data: Hoje as 15:00

Proprietário: Axl Rose
Animal: Ajudante do Papai Noel
Serviço: Banho
Data: Hoje as 15:30

Proprietário: Axl Rose
Animal: Ajudante do Papai Noel
Serviço: Consulta Clínica
Data: Hoje as 16:00


## Questões - Colocar somente as querys

Inclua os trechos com as queries que respondem as perguntas abaixo:

### Quantos agendamentos existem para o Rex do Jhonny Cash?

    SUA RESPOSTA AQUI

### Como saber se temos algum Cavalo cadastrado como animal?

    SUA RESPOSTA AQUI

### Buscar todos os agendamentos com dados do animal, serviço e proprietário

    SUA RESPOSTA AQUI

### Se o petshop trabalhar todos os dias com os mesmos agendamentos, quanto ele faturará em 3 meses considerando que 1 mês = 30 dias.

    SUA RESPOSTA AQUI

### Quanto tempo falta para o agendamento do Rex, do Sid Vicious, considerando que agora são 11h?

    SUA RESPOSTA AQUI    

### Como incrementar o valor de venda de todos os serviços que foram agendados no mês passado?

    SUA RESPOSTA AQUI

# Entrega do projeto

- Crie uma aplicação nova para executar o desafio. Pode escolher o banco de dados de preferência.
- Ao finalizar, suba a sua proposta para o projeto que você criou no GitHub. Exemplo: https://github.com/seuNome/pet-code;
- Envie-nos o link do projeto. Exemplo: https://github.com/seuNome/test-backend-java.git
- Pronto! Basta aguardar o nosso RH entrar em contato. Entramos em contato rapidinho ;)