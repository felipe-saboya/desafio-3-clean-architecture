# Readme

## Passos

### 1 DockerCompose

```
docker-compose up -d
```

### 2 MySQL - Makefile

```
make migrate-up
make migrate-down
```

### 3 Start

```
go run cmd/ordersystem/main.go cmd/ordersystem/wire_gen.go
```

> Play :)
 
## Portas

### Web HTTP

localhost:8000

### gRPC

localhost:50051

### GraphQL

localhost:8080

---

# desafio-3-clean-architecture

Olá devs!
Agora é a hora de botar a mão na massa. Para este desafio, você precisará criar o usecase de listagem das orders.
Esta listagem precisa ser feita com:
- Endpoint REST (GET /order)
- Service ListOrders com GRPC
- Query ListOrders GraphQL
  Não esqueça de criar as migrações necessárias e o arquivo api.http com a request para criar e listar as orders.

Para a criação do banco de dados, utilize o Docker (Dockerfile / docker-compose.yaml), com isso ao rodar o comando docker compose up tudo deverá subir, preparando o banco de dados.
Inclua um README.md com os passos a serem executados no desafio e a porta em que a aplicação deverá responder em cada serviço.
