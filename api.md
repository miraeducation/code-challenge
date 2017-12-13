# API
Para a implementação dos testes de frontend e mobile será necessário consumir os seguintes serviços com os respectivos contratos:

### Receber informações sobre o usuário (professor)

```http
GET https://api-test.miraeducacao.com.br/me

{
   "id": "ecc9a6ed-2456-4f21-8909-60535ed1670b",
   "name": "João Ferreira"
}
```

### Receber listagem de turmas

```http
GET https://api-test.miraeducacao.com.br/teacher/{teacherId}/classes

[
   {
      "id": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
      "discipline": "Geometria",
      "level": "6º ano",
      "term": "B",
      "period": "Manhã"
   },
   {
      "id": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
      "discipline": "Física",
      "level": "8º",
      "period": "Noturno",
      "term": "C"
   }
]
```

### Receber listagem de turmas

```http
GET https://api-test.miraeducacao.com.br/teacher/{teacherId}/classes

[
   {
      "id": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
      "discipline": "Geometria",
      "level": "6º ano",
      "term": "B",
      "period": "Manhã"
   },
   {
      "id": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
      "discipline": "Física",
      "level": "8º",
      "period": "Noturno",
      "term": "C"
   }
]
```

### Receber a listagem de alunos de uma turma

```http
GET 	https://api-test.miraeducacao.com.br/class/{classId}/students

[
   {
      "id": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
      "orderId": "1",
      "name": "João de Barro"
   },
   {
      "id": "4bbb5158-e60a-4c96-9a3e-ac360b6632f3",
      "orderId": "3",
      "name": "Mário Roberto"
   },
   {
      "id": "9d395096-e02d-11e7-80c1-9a214cf093ae",
      "orderId": "4",
      "name": "Rosana Silva"
   },
   {
      "id": "a243b392-e02d-11e7-80c1-9a214cf093ae",
      "orderId": "16",
      "name": "Humberto Ramos"
   },
   ...
   {
      "id": "4324fsfd-cfsafas-4fasa2-8fs21-sasf",
      "orderId": "8",
      "name": "Maria Alberta"
   }
]
```

### Inserir uma chamada de uma turma

```http
POST 	https://api-test.miraeducacao.com.br/class/{classId}/lesson
{
   "date": "2016-09-13T13:30:52.123Z"
   "lessonOrder": 1,
   "attendances": [
      {
         "studentId": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
         "status": "PRESENT"
      },
      {
         "studentId": "4bbb5158-e60a-4c96-9a3e-ac360b6632f3",
         "status": "PRESENT"
      },
      {
         "studentId": "4324fsfd-cfsafas-4fasa2-8fs21-sasf",
         "status": "ABSENCE"
      }
   ]
}
```

### Atualizar uma chamada de uma turma

```http
PUT 	https://api-test.miraeducacao.com.br/class/{classId}/lesson/{lessonId}
{
   "id": "10ff4245-4621-42f3-9c75-e10244f43134",
   "date": "2016-09-13T13:30:52.123Z"
   "lessonOrder": 1,
   "attendances": [
      {
         "studentId": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
         "status": "PRESENT"
      },
      {
         "studentId": "4bbb5158-e60a-4c96-9a3e-ac360b6632f3",
         "status": "ABSENCE"
      },
      {
         "studentId": "4324fsfd-cfsafas-4fasa2-8fs21-sasf",
         "status": "PRESENCE"
      }
   ]
}
```

> Para efeitos de simplicidade, não há necessidade de autenticação nem autorização para consumo dos serviços.
