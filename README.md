# Demo sobre live coding da Digital Innovation One - Spring WebFlux

## Stack utilizada

- Java8
- Spring WebFlux
- Spring Data
- DynamoDB
- JUnit
- sl4j
- Reactor

### Slides da palestra: https://speakerdeck.com/kamilahsantos/live-coding-dio-api-de-herois-com-spring-webflux

### Palestra gravada: https://www.youtube.com/watch?v=1VllPZYn6RI&t=3257s

### Executar AWS Dynamo DB:

```shell
docker run -p 8000:8000 --name dynamodb amazon/dynamodb-local -jar DynamoDBLocal.jar -inMemory -sharedDb
```

Para listar as tabelas criadas: `aws dynamodb list-tables --endpoint-url http://localhost:8000`
Para listar os conteúdos da tabela: `aws dynamodb scan --table-name Heroes_Table --endpoint-url http://localhost:8000`

Documentacao gerada pela aplicação: http://localhost:8080/swagger
