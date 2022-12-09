# argo-helm-hooks
Sample manifests for argo cd and helm hooks implementation

# setting up argo on kind cluster

Install small k8s single node cluster using kind and install argo cd on it

```shell
# create and verify connectivity
kind create cluster --name demo
kubectl get nodes

# install argo cd using helm chart
helm repo add argo-cd https://argoproj.github.io/argo-helm
helm install argo argo-cd/argo-cd
```
