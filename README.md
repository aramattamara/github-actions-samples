# github-actions-samples

This repo contains samples of Github Actions Workflows

To let minikube use your locally built image:

```shell
minikube image load hello-gitops:local
minikube -n hello-gitops service hello-gitops --url
```
