---
title: 'Response status codes'

layout: 
---

### Success

Os sucessos diferem dos erros, pois seu corpo pode não ser um objeto de resposta simples com um código e uma mensagem. Os cabeçalhos, no entanto, são consistentes em todas as chamadas:

* `GET`, `PUT`, `DELETE` retorna `200 OK` quando bem sucedidos,
* `POST ` retorna 201 quando bem sucedido,


### Error

Error responses simplismente retornam [HTTP error codes](http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html) padrão, junto com algumas informações adicionais:

* O código de erro é enviado de volta como um cabeçalho de status,
* O corpo inclui um objeto que descreve o código e a mensagem (para fins de depuração e / ou exibição),

Por exemplo, para uma chamado com o token inválido....

```Status: 401 Access denied```
```{
    code: 401,
    message: 'Access denied: invalid authentication token.'
}```