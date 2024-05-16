### Criar um Pod

```bash
kubectl run <nome-do-pod> --image=<imagem>:<tag>
```

### Listar os Pods

```bash
# lista os pods
kubectl get pods
# acompanha em tempo real
kubectl get pods --watch
```

### Descrever um Pod

```bash
kubectl describe pod <nome-do-pod>
```

### Atualizar um Pod existente

```bash
kubectl edit pod <nome-do-pod>
```

### Criar um Pod definido de maneira declarativa

```bash
kubectl apply -f <nome-do-arquivo.yml>
```
