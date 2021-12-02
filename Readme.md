# Car registry

## Relevant informations

 - **Java 11**
-	**Spring Framework**
-	**Junit**
-	**Mockito**

## Project Description

This project was builded to develop a backend to a car registration at a store.

This is just a study project, feel free to get/change it as you want.

## Project shortcuts

[Controller](https://github.com/renanponcianop/crud-java-spring/blob/main/src/main/java/com/exercicos/ex5/resources/VeiculoResource.java)

[Service](https://github.com/renanponcianop/crud-java-spring/blob/main/src/main/java/com/exercicos/ex5/services/VeiculoService.java)

[Tests](https://github.com/renanponcianop/crud-java-spring/blob/main/src/test/java/com/exercicos/ex5/services/VeiculoServiceTest.java)
	
## Services implemented:
 
- Vehicle registration
- Vehicle data update
- Delete vehicles
- Display information on how many vehicles are unsold in the base.
- View vehicle distribution information by manufacturing decade
	- Example:
		- 1990s -> 15 vehicles
		- 2000's -> 31 vehicles
- View vehicle distribution information by manufacturer.
	- Example:
		- Ford-> 14 vehicles o
		- Honda-> 8 vehicles
- View cars registered during the last week.
- There must be consistency in the brands provided. There can be **no** wrongly written marks.
	- Example: Volksvagen, Forde, Teslla, etc.


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
