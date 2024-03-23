# Argo CD

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


3. **List all pods in the `argocd` namespace**:

    ```bash
    kubectl get pod -n argocd
    ```

    This command will display all pods running in the `argocd` namespace.

4. **List all secrets in the `argocd` namespace**:

    ```bash
    kubectl get secrets -n argocd
    ```

    This command will display all secrets stored in the `argocd` namespace.



5. **Retrieve the initial admin password secret**:



  
    ```bash
    kubectl get secrets argocd-initial-admin-secret -n argocd -o yaml
    ```

    This command will display detailed information about the secret containing the initial admin password in YAML format.




![Alt text](https://raw.githubusercontent.com/hassanahtasham/ArgoCD/main/Argocd.png "Argo CD Sync the Changes")