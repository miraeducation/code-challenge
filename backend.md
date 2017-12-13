# Teste Técnico - Backend

## Objetivo
Construção de uma API para manutenção de dados de usuários.

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
- Desenvolver usando *Java* ou *Kotlin*
- Serviço deve respeitar os princípios RESTFul
- Utilizar Maven ou Gradle para build do seu projeto

## Lembrando..
- Não esqueça de testes e documentações
- **Executaremos** seu serviço e esperamos não ter que alterar ou configurar nada para atingir este objetivo com sucesso
- Está com dúvidas? Converse com o seu contato na Mira! :)
