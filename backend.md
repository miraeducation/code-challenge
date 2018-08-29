# Teste Técnico - Backend

## Objetivo
O objetivo do teste é:
   - Construir uma API para manutenção de dados de usuários.

## Contexto
Estamos desenvolvendo uma aplicação para cadastro de pessoas na qual existem duas situações de cadastro:
   - uma pessoa fazendo cadastro *único* via portal
   - uma lista de pessoas sendo inseridas de uma única vez (*bulk*)

No lado do servidor precisamos desenvolver uma API para o CRUD de pessoas, considerando as duas situações mencionadas.

As informações de uma pessoa que precisamos cadastrar são:
- Nome
- Sobrenome
- CPF
- Data de nascimento
- Endereço
- Telefones
- Emails
- Ativo (S /N)

> TLDR: o serviço deve prover endpoints de inserção, busca, atualização e remoção de um ou mais usuários

> Uma nova pessoa é considerada ativa e recebe um `id` gerado automaticamente

### Funcionalidades extras
- Endpoint de busca por nome, sobrenome e/ou CPF
- Endpoint para ativar/desativar uma lista de ids de pessoas

## Requisitos técnicos
- Desenvolver usando *Java*, *Kotlin* ou *Python*, utilizando os frameworks SpringBoot, Django ou Flask
- Serviço deve respeitar os princípios RESTFul
- Utilizar Gradle para build do seu projeto
- Os dados manipulados pela API devem ser armazenados em uma base de dados Embedded
- Implemente testes, garanta que todas as requisições funcionam como deveriam funcionar

## Lembrando..
- Não esqueça de testes e documentações
- **Executaremos** seu serviço e esperamos não ter que alterar ou configurar nada para atingir este objetivo com sucesso
- Está com dúvidas? Converse com o seu contato na Mira! :)

## Diferenciais
- Publicação do ambiente em um serviço cloud de hospedagens (Heroku, AWS, GCP, etc)
- 
