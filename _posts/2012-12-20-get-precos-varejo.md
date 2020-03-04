---
category: Pesquisa Preços
route: '/pesquisa_preco_varejos'
title: 'Pesquisa Preços Varejo'
type: 'GET'

layout:
---

Esta rota permite que usuarios obtemnham os preços de varejo

### MODELO DE REQUISIÇÃO

* ```htpps://api.profitmais.com.br/big/pesquisa_preco_varejos?accessToken=API_TOKEN```
* Para acessar a rota é necessário passar o token como parametro 

**params:{accessToken:API_TOKEN}**.

### MODELO DE RESPOSTA

Retorna uma coleção de produtos com seus respectivos preços.

```Status: 200 OK```
```[
    {
        "id_lj":null,
        "id_conc":"GBA 01",
        "ean":"23792700000",
        "fg_promo":"0",
        "prc_vrj":"38.25",
        "prc_atc":null,
        "gatilho_atc":null,
        "prc_fid":null,
        "med_conv":null,
        "url_foto1":null,
        "url_foto2":null,
        "qtd_un_conversao":0,
        "id":null
    }, ...
]```

Caso ocorram erros, acesse [lista de codigos de response status](#response-status-codes).
