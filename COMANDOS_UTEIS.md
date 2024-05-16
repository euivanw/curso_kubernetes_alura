### Criar um Pod

```shell
kubectl run <nome-do-pod> --image=<imagem>:<tag>
```

### Listar os Pods

```shell
# lista os pods
kubectl get pods
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
kubectl delete pod <nome-do-pod>
kubectl delete -f <nome-do-arquivo.yml>
```

### Entrar no shell de um Pod

```shell
kubectl exec -it <nome-do-pod> -- shell
```
