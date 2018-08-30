# Teste Técnico - Backend

## Objetivo
O objetivo do teste é:
   - Construir uma API para manutenção de dados de usuários.

## Contexto
Estamos desenvolvendo uma aplicação para manutenção de cadastro de pessoas na qual existem as seguites situações:
   - uma pessoa fazendo cadastro *único* via portal
   - uma lista de pessoas sendo inseridas de uma única vez (*bulk*)
   - receber a lista de pessoas inseridas
   - atualizar uma pessoa
   - remover uma pessoa logicamente da base

No lado do servidor precisamos desenvolver uma API para o CRUD de pessoas, considerando as duas situações mencionadas.

As informações de uma pessoa que precisamos cadastrar são:
- Nome
- Sobrenome
- CPF
- Data de nascimento
- Endereço
- Telefones
- Emails
- Ativo (S/N)

> Uma nova pessoa é considerada ativa e recebe um `id` gerado automaticamente

### Funcionalidades extras
- Endpoint de busca por nome, sobrenome e/ou CPF

## Requisitos técnicos
- Desenvolver usando *Java*, *Kotlin* ou *Python*
- Serviço deve respeitar os princípios RESTFul
- Implemente testes, garanta que todas as requisições funcionam como deveriam funcionar
- README.md explicando como executar o projeto

## Diferenciais
- Publicação do ambiente em um serviço cloud de hospedagens (Heroku, AWS, GCP, etc)
- Configurar a aplicação para rodar em um container

## Lembrando..
- O fluxo de interação com o BitBucket também será avaliado (commits, pushs, comentários)
- **Executaremos** seu serviço e esperamos não ter que alterar ou configurar nada para atingir este objetivo com sucesso
- Está com dúvidas? Converse com o seu contato na Mira! :)
