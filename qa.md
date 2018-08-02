# Teste Técnico - QA

### Instruções

O seu objetivo é criar um projeto de automação de testes para um fluxo de cadastro mobile disponível no link abaixo:

    https://invis.io/6DNBJXW2UWC

Utilize os critérios de aceite para descrever os cenários de teste.

#### Requisitos

- O projeto deve ser desenvolvido utilizando `Appium`, caso você não conheça pode escolher outra ferramenta e descrever um pouco sobre a mesma
- Os cenários de teste devem ser escritos em `BDD`
- Crie a identificação dos elementos da forma que achar melhor, visto que as telas são só para consulta e não serão utilizadas para rodar o projeto
- Utilize as demais ferramentas e linguagem de desenvolvimento que preferir

### Critérios de Aceite

EU como professor
QUERO realizar o meu cadastro e o meu primeiro acesso através do aplicativo 
PARA QUE eu possa usar o aplicativo, e desta forma, facilitar a minha rotina dentro e fora da sala de aula

O QUE É ESPERADO:
- Quero abrir o aplicativo em meu celular e poder clicar na opção “primeiro acesso”;
- O CPF e a data de nascimento devem ser válidos para que eu possa prosseguir com o cadastro; 
- Caso o CPF seja informado errado deve ser exibida a mensagem “CPF inválido”; 
- Caso o CPF já esteja cadastrado deve ser exibida a mensagem de erro “CPF já cadastrado”; 
- Caso a data de nascimento seja inválida deve ser exibida a mensagem de erro “Data de nascimento inválida”; 
- Os e-mails devem ser idênticos para que eu possa prosseguir com o cadastro; 
- Caso seja informado um e-mail inválido deve ser exibida a mensagem de erro “E-mail inválido”; 
- Caso os e-mails não sejam idênticos deve ser exibida a mensagem de erro “Os e-mails não coincidem”;
- A senha deve conter no mínimo 4 caracteres; 
- Caso seja informada uma senha com menos de 4 caracteres em algum dos campos de senha deve ser exibida a mensagem de erro “A senha deve ter 4 caracteres ou mais”;    
- Caso as senhas não sejam idênticas deve ser exibida a mensagem de erro “As senhas não coincidem”; 
- A senha será considerada fraca quando houver apenas letras ou números; 
- A senha será considerada média quando houver letras e números; 
- A senha será considerada forte quando houver letras, números e caracteres especiais;
- Todos os campos são obrigatórios, caso um campo não seja preenchido o botão “avançar” do fluxo não deve ser habilitado na tela. 