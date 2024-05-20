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

# apaga todos os pods de uma vez
kubectl delete pods --all
```

### Entrar no shell de um Pod

```shell
kubectl exec -it <nome-do-pod> -- shell
```

### Lista o Services

```shell
# lista os serviços
kubectl get svc

# lista os serviços com mais informações
kubectl get svc -o wide

# acompanha em tempo real
kubectl get svc --watch
```

### Lista os Nodes

```shell
# lista os nodes
kubectl get nodes

# lista os nodes com mais informações
kubectl get nodes -o wide
```

### Apagar um Service

```shell
# apaga manualmente
kubectl delete svc <nome-do-service>

# apaga via arquivo de declaração
kubectl delete -f <nome-do-arquivo.yml>

# apaga todos os services de uma vez
kubectl delete svc --all
```

### Lista os ConfigMaps

```shell
kubectl get configmap
```

### Listar os ReplicaSets

```shell
# lista os replica sets
kubectl get rs

# lista os replica sets com mais informações
kubectl get rs -o wide

# acompanha em tempo real
kubectl get rs --watch
```
