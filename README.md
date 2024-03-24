### Install
```
helm repo add argo https://argoproj.github.io/argo-helm
helm install argocd argo/argo-cd --namespace argocd --create-namespace --dependency-update --set argo-cd.configs.secret.argocdServerAdminPassword=$ARGOCD_ADMIN_PWD
helm upgrade argocd ./bootstrap/argo/ --namespace argocd -f ./bootstrap/argo/values.yaml
```