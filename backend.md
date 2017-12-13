# Teste Técnico - Backend

## Objetivo
Construção de uma API para manutenção de dados de usuários.

## Contexto
Estamos desenvolvendo uma aplicação para cadastro de pessoas na qual existem duas situações de cadastro:
   - as pessoas que se cadastram online via portal,
   - as pessoas que se cadastram pelo app do tablet dos pesquisadores (que armazena os cadastros e os envia em lote quando possui conexão).
  Além disso a aplicação precisa permitir a edição de usuários com erros de cadastro, a busca de usuários por cpf e a remoção de usuários que não serão utilizados na campanha.
  No lado do servidor precisamos desenvolver uma aplicação para possibilitar esses cadastros.
  As informações que precisamos das pessoas cadastradas são: nome, sobrenome, data de nascimento, endereço, telefones.

## Requisitos técnicos
- Desenvolver usando java ou kotlin
- O serviço deve prover endpoints de inserção, busca, atualização e remoção de usuários
- Serviço deve respeitar os princípios Restful
- Utilizar Maven ou Gradle para build do seu projeto

## Lembrando..
- Não esqueça de testes e documentações
- **Executaremos** seu serviço e esperamos não ter que alterar ou configurar nada para atingir este objetivo com sucesso
