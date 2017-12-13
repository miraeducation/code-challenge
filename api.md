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

### Salvar uma chamada de uma turma

```http
POST 	https://api-test.miraeducacao.com.br/class/{classId}/lesson
{
   "id": "10ff4245-4621-42f3-9c75-e10244f43134",
   "date": "2016-09-13T13:30:52.123Z"
   "lessonOrder": 1,
   "attendances": [
      {
         "id": "85f63a71-6ca0-4206-aab7-860ad852a61b",
         "studentId": "e8c6d161-c8d1-4e90-8e0f-affd06ac005c",
         "status": "PRESENT"
      },
      {
         "id": "30e22663-1e2c-41c0-999b-b63141881d39",
         "studentId": "af10781d-29a9-4975-93e0-7e84da831cfe",
         "status": "PRESENT"
      },
      {
         "id": "ff419d56-72c4-4d5f-8235-33fe3b882b25",
         "studentId": "a3d92a48-7db4-4f61-a620-48e6342abb8c",
         "status": "ABSENCE"
      }
   ]
}
```

> Para efeitos de simplicidade, não há necessidade de autenticação nem autorização para consumo dos serviços.
