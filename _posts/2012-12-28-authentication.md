---
route: '/access-token'
title: 'Autenticação'

layout: 
---

Para acessar as informações basta solicitar um código de acesso para a equipe Profit+

### Response

Sends back a collection of things.

```Status 401```
```{
  "error": {
    "statusCode": 401,
    "name": "Error",
    "message": "Autorização Necessária",
    "code": "AUTHORIZATION_REQUIRED",
    "stack": "Error: Autorização Necessária...
}```

Caso ocorram erros, acesse [lista de codigos de response status](#response-status-codes).