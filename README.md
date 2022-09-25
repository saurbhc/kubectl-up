Start and stop local Kubernetes clusters.

* Docker Desktop
* MiniKube

`kubectl up` will start and initialize a local cluster. `kubectl down` will stop local cluster.

Installation:

```bash
git clone https://github.com/saurbhc/kubectl-up.git -o ~/kubectl-up
export PATH=~/kubectl-up:$PATH ;# add to your ~/.bashrc
```

Install Docker Desktop

Install your local Kubernetes provider.

- [Kubernetes on Docker Desktop](https://docs.docker.com/desktop/kubernetes/).

- Minikube

    - via brew
        ```bash
        brew install minikube
        ```
    - via curl
        ```bash
        curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-arm64
        sudo install minikube-darwin-arm64 /usr/local/bin/minikube
        ```

Usage:

```bash
kubectl up
```

- Alternatives:

    ```bash
    kubectl up docker-desktop-and-minikube ;# default
    ```

    ```bash
    kubectl up docker-desktop
    ```

    ```bash
    kubectl up minikube
    ```

```bash
kubectl down
```
