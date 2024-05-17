### Criar um Pod

```shell
kubectl run <nome-do-pod> --image=<imagem>:<tag>
```

### Listar os Pods

```shell
# lista os pods
kubectl get pods

# lista os pods com mais informações
kubectl get pods -o wide

# acompanha em tempo real
kubectl get pods --watch
```

### Descrever um Pod

```shell
kubectl describe pod <nome-do-pod>
```

### Atualizar um Pod existente

```shell
kubectl edit pod <nome-do-pod>
```

### Criar um Pod definido de maneira declarativa

```shell
kubectl apply -f <nome-do-arquivo.yml>
```

### Apagar um Pod

```shell
# apaga manualmente
kubectl delete pod <nome-do-pod>

# apaga via arquivo de declaração
kubectl delete -f <nome-do-arquivo.yml>
```

### Entrar no shell de um Pod

```shell
kubectl exec -it <nome-do-pod> -- shell
```

### Lista o Services

```shell
# lista os serviços
kubectl get services

# lista os serviços com mais informações
kubectl get services -o wide
```
