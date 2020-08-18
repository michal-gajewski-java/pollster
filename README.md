# Pollster - Ankieter
REST API backend application that serves CRUD API for Pollster functionality.

## Technologies

* Java 8
* Spring Boot 2
* Hibernate
* PostgreSQL
* H2
* JUnit 5
* Mockito 3
* REST

## Features

* C - Create new Survey
* R - Read Survey details
* U - Update Survey data
* D - Delete existing Survey

## Endpoints

POST - /pollster/surveys

request body/payload: 
````
{
    "id": null,
    "name": "Badanie zainteresowan studentów",
    "owner": "Instytut Psychologii"
}
````
response
````
{
    "id": 1,
    "name": "Badanie zainteresowan studentów",
    "owner": "Instytut Psychologii"
}
````

GET - /pollster/surveys/{id}

path param: /pollster/surveys/1

response
````
{
    "id": 1,
    "name": "Badanie zainteresowan studentów",
    "owner": "Instytut Psychologii"
}
````

PUT - /pollster/surveys/{id}

path param: /pollster/surveys/1

request body/payload: 
````
{
    "id": 1,
    "name": "Badanie opini konsumentow o stanie gospodarki krajowej",
    "owner": "Instytut Nauk Ekonomicznych"
}
````
response
````
{
    "id": 1,
    "name": "Badanie opini studentów o rynku pracy",
    "owner": "Instytut Nauk Ekonomicznych"
}
````

DELETE - /pollster/surveys/{id}

path param: /pollster/surveys/1