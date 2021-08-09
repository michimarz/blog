---
title: "REST Web Services (JAX-RS)"
date: 2021-08-09T10:23:34+02:00
draft: false
---

## HATEOAS

Nie potrzebujemy dokumentacji żeby skorzystać z jakiejś strony www.  
Idziesz do strony głównej i tam widzisz linki do innych stron.  

HATEOAS jest zastosowaniem tej koncepcji dla usług REST.  
Usługa w responsie dołącza linki do innych powiązanych usług dla danego zasobu.

Na przykład w odpowiedzi na ``GET /accounts/12345 HTTP/1.1 ...`` możemy otrzymać:

```json
HTTP/1.1 200 OK

{
    "account": {
        "account_number": 12345,
        "balance": {
            "currency": "usd",
            "value": 100.00
        },
        "links": {
            "deposits": "/accounts/12345/deposits",
            "withdrawals": "/accounts/12345/withdrawals",
            "transfers": "/accounts/12345/transfers",
            "close": "/accounts/12345/close"
        }
    }
}
```

## Richardson Maturity Model

#### Level 0
inaczej zwany Swamp of POX (gdzie POX = Plain Old XML)

* Jeden URL (endpoint)
* Wszystkie szczegóły zawarte są w treści requesta

#### Level 1
Korzysta z koncepcji Resource URI
* osobne URI dla każdego zasobu

#### Level 2
Korzysta z HTTP Methods
* używa właściwych metod HTTP, oraz właściwych Status Codes

#### Level 3
Implementuje HATEOAS
* response zawiera linki, które klient może użyć w dalszej kolejności

Level 3 można jeszcze podzielić wg HMM (Hypermedia Maturity Model)

<!-- TODO -->


