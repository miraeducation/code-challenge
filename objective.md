# Objetivo

> Utilizado para os testes de frontend e mobile

Hoje um dos grandes investimentos de tempo do professor no Brasil é o preenchimento do diário de classe. Para ajudar o professor a economizar esse tempo que poderia estar sendo usado para ensinar, a Mira Educação transformou o diário de classe em um serviço (app ou portal web) para ser usado em seu **smartphone**.

> Lembre-se! Somos offline e mobile first:
> - Para apps: ser offline first significa ser resiliente e operável em momentos de falta de conectividade
> - Para web/frontend: ser mobile first não significa que não testaremos seu código em um desktop (big screen) :)

Uma das funcionalidades do diário de classe é a chamada -attendance-, onde o professor lança faltas para alunos ausentes e presença para os presentes. O objetivo deste exercício é desenvolver uma lista de chamada simples, seguindo a descrição a seguir:
- Ao entrar no serviço o professor visualiza a lista de turmas -classes- que ele leciona;
- Após selecionar a turma -class- desejada, a lista de alunos -students- referentes àquela turma é carregada.
- Na listagem de turmas a opção de presença -presence- é representada por um ícone check verde e a ausência -absence- por um ícone x vermelho.
- Para alterar uma presença para uma ausência, basta clicar no ícone de presença, transformando-o em um ícone de ausência. E para reverter uma ausência para uma presença, basta clicar no ícone de ausência.
- Ao final da lista há um botão "Enviar" que submete aquela chamada para o servidor. Após o  envio, o professor recebe um popup de sucesso ou erro, e é redirecionado para a listagem de turmas novamente.
- Uma vez que *uma chamada para uma turma em um mesmo dia é salva*, o professor ao tentar realizar novamente uma chamada para aquela *mesma turma* e naquele *mesmo dia*, pode decidir entre alterar a última chamada realizada ou criar uma nova chamada (para aulas duplas, triplas ou n-plas).

Para representar a regra acima, perguntamos ao professor (através de um pop-up) se ele está querendo alterar a chamada já realizada ou se ele quer lançar uma nova chamada. Caso ele decida criar uma nova chamada, a chamada anterior fica impossibilitada de alteração e a nova chamada é considerada a segunda chamada para aquela aula - `lessonOrder = 2`.

> Por padrão, ao realizar uma nova chamada para uma turma específica, todos os alunos vêm com presença.
