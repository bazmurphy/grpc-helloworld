# gRPC Hello World

[https://grpc.io/docs/languages/go/quickstart](https://grpc.io/docs/languages/go/quickstart)

## Generate gRPC code

```sh
$ protoc \
    --go_out=. \
    --go_opt=paths=source_relative \
    --go-grpc_out=. \
    --go-grpc_opt=paths=source_relative \
    protocolbuffer/helloworld.proto
```

## Run the server

```sh
go run greeter_server/main.go
```

## Run the client

```sh
go run greeter_client/main.go
```

## Add name as a command line argument

```sh
go run greeter_client/main.go --name=Baz
```
