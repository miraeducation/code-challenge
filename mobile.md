# Teste Técnico - Mobile

### Instruções

O seu objetivo é desenvolver um app que recebe um vetor *V* de um serviço externo, e dado um inteiro *N*, seu app informará se existem dois valores em *V* que somados resultam em *N*. 

### Restrições:

- *N* pode ser um número entre -197 e 197;
- *V* possui tamanho fixo 16 e pode conter valores inteiros entre -99 e 99;

<br />

![brisolla_2](https://user-images.githubusercontent.com/1713923/40144356-aa90cba4-5934-11e8-8bff-4dda177b5de4.png)

 <br />

O app deve seguir a UI apresentada. A primeira tela contém respectivamente:

- Os valores em V, carregado através do endereço https://k9h52hczu2.execute-api.us-east-2.amazonaws.com/prod/random_array_generator;

- O campo `Número` que representa N no nosso problema;

- Um botão `Verificar` que aplica o algorítmo que irá validar a existência de dois números em V cuja soma é N. A resposta deve ser apresentada via Toast: "Existe" ou "Não existe" e o campo `Número` deve ser limpo para novas verificações;

- Um botão `Redefinir Lista` que chamará o serviço do primeiro ítem e carregará um novo vetor V no app;

- Um botão `Histórico de consulta` que abre uma nova tela apresentando as execuções do botão `Verificar`:

 <br />

![brisolla_1](https://user-images.githubusercontent.com/1713923/40144323-96278edc-5934-11e8-9e65-36acc0dbeb8a.png)

 <br />

A tela de `Histórico de consulta` contém:

Top bar contendo um botão de *backward* que redireciona o usuário para a tela inicial;

Uma lista onde cada linha é uma consulta já realizada. `N` é o número inserido para consulta no algoritmo, `RESULTADO` é a resposta que o algoritmo retornou para o `N` inserido na lista corrente;

Cada linha contém um botão `ver lista` que apresenta através de um popup, o vetor V no momento daquela consulta;

#### Requisitos
- Desenvolver usando as seguintes linguagens:
  - Android: *Java* ou *Kotlin*
  - iOS: *Swift*
- App deve ser 100% crash free
- Implementação de testes (integrados e unitários)
- Criação de um `README.md` (arquitetura, libs, instruções de execução, etc)

#### Dicas
- Use libs externas, sempre que julgar necessário
- Gaste um tempo desenhando a sua solução antes de iniciar a codificação.
- Seja criativo e também resiliente, pense nos corner cases, serviços REST podem ficar indisponíveis e o app precisa tratar esses casos
