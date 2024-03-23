### Install
```
helm install argocd charts/argo-cd/ --create-namespace --dependency-update --set argo-cd.configs.secret.argocdServerAdminPassword=$ARGOCD_ADMIN_PWD
```