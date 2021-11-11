# Car registry

## Revelevant informations

Build with Spring 2.4.5 e Java 11

## Project Description

This project was builded to develop a backend to a car registration at a store. 

This is just a study project, feel free to get/change it as you want.

## Endpoints

```bash
/veiculos
Método: GET
Objetivo: Get all cars
```
```bash
/veiculos/{id}
Método: GET
Objetivo: Get a car by it's ID
```
```bash
/veiculos/find
Método: GET
Objetivo: Make a search for specific car
Parâmetros:
 vendidos= Boolean - True/False/Null - Return just the sold cars.
 decada= Integer - Search a car by a decade.
 fabricante= String - Search cars by manufacturer
 recentes= Boolean - True/False/Null - Shows only cars from the last 2 weeks
```
```bash
/veiculos
Método: POST
Objetivo: Registry a new car
Parâmetros: JSON:
{
    "id": Integer - id ,
    "veiculo": String - model,
    "marca": String - manufacturer,
    "ano": Integer- year,
    "descricao": String - description,
    "vendido": Boolean - true/false informs if the car was sold
}
```
```bash
/veiculos/{id}
Método: PUT
Objetivo: Change all data for a vehicle
Parâmetros: JSON:
{
    "id": Integer - id ,
    "veiculo": String - model,
    "marca": String - manufacturer,
    "ano": Integer- year,
    "descricao": String - description,
    "vendido": Boolean - true/false informs if the car was sold
}
```
```bash
/veiculos/{id}
Método: PATCH
Objetivo: Change only sent data
Parâmetros: JSON:
{
    "id": Integer - id ,
    "veiculo": String - model,
    "marca": String - manufacturer,
    "ano": Integer- year,
    "descricao": String - description,
    "vendido": Boolean - true/false informs if the car was sold
}
```
```bash
/veiculos/{id}
Método: DELETE
Objetivo: Delete a vehicle from the bank
```
