# Protoc actions

This actions allow you generate client and server for grpc

# How to use

```yml
- name: Genereate code for squzy-storage protofile
  uses: brainyard-io/protoc-actions
  with:
    path: -I./proto --go_out=plugins=grpc,request_context=true:./generated proto/squzy-storage-proto/v1/service.proto
```

*Supports:*
- GRPC client server
- GRPC gateway
- Swagger from protofiles

thanks @PxyUp
