# parking-control

API para controle de estacionamento.
 
Tecnologias utilizadas:
- JDK 11
- Maven
- Postman
- PgAdmin (Postgres)
- Eclipse IDE

Projeto online: https://parking-control-api-lca.herokuapp.com

Para testá-lo, pode ser usado o postman com os seguintes métodos:

- POST (cria novo registro de vaga no estacionamento) <br/>
Endpoint: https://parking-control-api-lca.herokuapp.com/parking-spot <br/>
Atributos a serem passados:
```
{
    "parkingSpotNumber": "205B",
    "licensePlateCar": "RRS8562",
    "brandCar": "audi",
    "modelCar": "q5",
    "colorCar": "black",
    "responsibleName": "Carlos Daniel",
    "apartment": "205",
    "block": "B"
}
```

- GET ALL (pesquisa todos os registros, já pronto pra paginação) <br/>
Endpoint: https://parking-control-api-lca.herokuapp.com/parking-spot?page=0&size=5&sort=registrationDate,ASC

- GET ONE (pesquisa registro pelo id) <br/>
Endpoint: https://parking-control-api-lca.herokuapp.com/parking-spot/ID_PARA_SER_PESQUISADO_AQUI

- DELETE (deleta registro pelo id) <br/>
Endpoint: https://parking-control-api-lca.herokuapp.com/parking-spot/ID_PARA_SER_DELETADO_AQUI

- PUT (atualiza registro pelo id) <br/>
Endpoint: https://parking-control-api-lca.herokuapp.com/parking-spot/ID_PARA_SER_ATUALIZADO_AQUI
