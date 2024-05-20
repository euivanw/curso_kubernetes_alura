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

### Consultar o histórico de mudanças de um deployment

```shell
kubectl rollout history deployment <nome-do-deployment>
```

### Aplicando um deployment e ajustando o motivo da mudança

```shell
kubectl apply -f <arquivo-do-deployment.yaml> --record
kubectl annotate deployment <nome-do-deployment> kubernetes.io/change-cause="<causa-da-mudanca>"
```

### Alterando um deployment com base no histórico de mudanças

```shell
kubectl rollout undo deployment <nome-do-deployment> --to-revision=<numero-revisao>
```

### Listar os StatefulSets

```shell
# lista 
kubectl get pv

# lista  com mais informações
kubectl get statefulset -o wide

# acompanha em tempo real
kubectl get statefulset --watch
```

### Listar os Persistent Volume

```shell
# lista 
kubectl get pv

# lista  com mais informações
kubectl get pv -o wide

# acompanha em tempo real
kubectl get pv --watch
```

### Listar os Persistent Volume Claim

```shell
# lista 
kubectl get pvc

# lista  com mais informações
kubectl get pvc -o wide

# acompanha em tempo real
kubectl get pvc --watch
```
