# ArgoCD Project

This is a a demo project for setting up ArgoCD in your Kuberenetes Cluster and with a basic Example


# Installing ArgoCD in Kubernetes

## Installation Steps

1. **Create a Namespace**: Run the following command to create a namespace named `argocd`:

    ```bash
    kubectl create namespace argocd
    ```

2. **Apply ArgoCD Manifests**: Apply the ArgoCD manifests to your Kubernetes cluster using the following command:

    ```bash
    kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
    ```


   
    This will deploy ArgoCD components in the `argocd` namespace.



![Alt text](https://raw.githubusercontent.com/hassanahtasham/ArgoCD/main/Argocd.png "Argo CD Sync the Changes")