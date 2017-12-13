# Teste Técnico - Frontend

## Objetivo
Hoje um dos grandes investimentos de tempo do professor no Brasil é o preenchimento do diário de classe. Para ajudar o professor a economizar esse tempo que poderia estar sendo usado para ensinar, a Mira Educação transformou o diário de classe em um portal web para ser usado em seu **smartphone**.

> Lembrem-se: somos offline e mobile first! Neste caso, apenas mobile first já é suficiente, mas vamos testar seu projeto no desktop também :)

Uma das funcionalidades do diário de classe é a chamada -attendance-, onde o professor lança faltas para alunos ausentes e presença para os presentes. O objetivo deste exercício é desenvolver uma lista de chamada simples, seguindo a descrição a seguir:
- Ao entrar no portal web o professor visualiza a lista de turmas -classes- que ele leciona;
- Após selecionar a turma -class- desejada, a lista de alunos -students- referentes àquela turma é carregada.
- Na listagem de turmas a opção de presença -presence- é representada por um ícone check verde e a ausência -absence- por um ícone x vermelho.
- Para alterar uma presença para uma ausência, basta clicar no ícone de presença, transformando-o em um ícone de ausência. E para reverter uma ausência para uma presença, basta clicar no ícone de ausência.
- Ao final da lista há um botão "Enviar" que submete aquela chamada para o servidor. Após o  envio, o professor recebe um popup de sucesso ou erro, e é redirecionado para a listagem de turmas novamente.
- Uma vez que *uma chamada para uma turma em um mesmo dia é salva*, o professor ao tentar realizar novamente uma chamada para aquela *mesma turma* e naquele *mesmo dia*, pode decidir entre alterar a última chamada realizada ou criar uma nova chamada (para aulas duplas, triplas ou n-plas).

Para representar a regra acima, perguntamos ao professor (através de um pop-up) se ele está querendo alterar a chamada já realizada ou se ele quer lançar uma nova chamada. Caso ele decida criar uma nova chamada, a chamada anterior fica impossibilitada de alteração e a nova chamada é considerada a segunda chamada para aquela aula - `lessonOrder = 2`.

> Por padrão, ao realizar uma nova chamada para uma turma específica, todos os alunos vêm com presença.

## UI

A primeira tela apresenta o nome do professor recuperado no endpoint `/me` e a lista de suas aulas.

<img width="601" alt="screen shot 2017-12-13 at 14 34 19" src="https://user-images.githubusercontent.com/664138/33950601-fb21c874-e013-11e7-91d3-7d41acadf7aa.png">

Quando o processo seleciona a turma, é disponibilizada a listagem de alunos para lançamento de chamada.

<img width="600" alt="screen shot 2017-12-13 at 14 34 36" src="https://user-images.githubusercontent.com/664138/33950609-00aca67e-e014-11e7-89c2-2a5824607b4f.png">

> A data da chamada será inferida a partir da data do navegador.

- Ao salvar a chamada, o popup é disponibilizado para o usuário:

<img width="602" alt="screen shot 2017-12-13 at 14 35 43" src="https://user-images.githubusercontent.com/664138/33950639-0e30f78c-e014-11e7-902e-1f8bc1368b19.png">

## Requisitos técnicos

- Desenvolver usando as seguintes tecnologias:
  - Webpack
  - React com flux
  - Stylus
  - Javascript ES6 / ES7
- Opcionais:
  - Progressive Web App
  - Suporte offline
- Não devem ser utilizados frameworks como Meteor, Ionic ou similares
- Implementação de testes (integrados e unitários)
- Criação de um `README.md` (arquitetura, instruções de execução, entre outros)


## Dicas
- Gaste um tempo desenhando a sua solução antes de iniciar a codificação
- Seja criativo e também resiliente, pense nos corner cases, a API pode ficar indisponível e o portal web precisa lidar com essa indisponibilidade
- Está com dúvidas? Converse com o seu contato na Mira! :)
