- Get pods of Pending and Running status

```
kubectl get pods -n dev --field-selector=status.phase=Pending
kubectl get pods -n dev --field-selector=status.phase=Running
```
- Scale RepicationController

```
kubectl scale --replicas=1000 replicationcontroller/nginx-rc -n dev
```

- Describe a replication controller

```
kubectl describe -n dev replicationcontroller/nginx-rc
```

- Get Node Information

```
kubectl get nodes -o wide
```

- Add new labels to the node

```
kubectl label nodes minikube-m03 workload=dev colour=yellow
```




https://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@github.com/JitenPalaparthi/hitachi-training.git