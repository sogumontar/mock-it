# Api For Mock.it

## Create new mock json

+ Endpoint : ``/api/mock/``
+ HTTP Method : ``POST``
+ Request Body :

```json
{
    "data": "recipients: [{id: 1,full_name: Andree Panjaitan,email: andree99@gmail.com,address: Porsea,username: andree99,role: ROLE_CUSTOMER},{id: 2, full_name: Hendra simangunsong,email: hendra@gmail.com, address: Silaen, username: hendra123, role: ROLE_CUSTOMER}],"
}
```

## Get mock json

+ Endpoint : ``/api/mock/{endPoint}``
+ HTTP Method : ``GET``
+ Request Header :
    + Accept : ``application/json``
+ Response Body (Success) :

```json
{
    "code": 200,
    "status": "OK",
    "message": "Agenda deleted successfully",
    "data": "recipients: [{id: 1,full_name: Andree Panjaitan,email: andree99@gmail.com,address: Porsea,username: andree99,role: ROLE_CUSTOMER},{id: 2, full_name: Hendra simangunsong,email: hendra@gmail.com, address: Silaen, username: hendra123, role: ROLE_CUSTOMER}],",
    "date": "2022-02-24" 
}
```

+ Response Body (Fail) :

```json
{
    "timestamp": "2021-05-14T04:22:26.690+0000",
    "code": 404,
    "status": "NOT FOUND",
    "message": "End point not found"
}
```

```json
{
    "timestamp": "2021-05-14T04:22:26.690+0000",
    "status": 500,
    "error": "Internal Server Error",
    "message": "System Busy"
}
```
