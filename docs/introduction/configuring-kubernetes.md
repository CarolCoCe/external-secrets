# Install and Configure Kubernetes

For more details, check the [official documentation](https://kubernetes.io/docs/home/).

## Installation Guide

### Install Docker

```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh

# Test Docker

sudo docker version
```
### Install Kind (Kubernetes in Docker)

#### For Linux AMD64 / x86_64
```bash 
curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.23.0/kind-linux-amd64
chmod +x ./kind
sudo mv ./kind /usr/local/bin/kind

# Test Kind
kind --version
```

#### For macOS using Homebrew
```bash
brew install kind

# Test Kind
kind --version
```

More installation options at https://kind.sigs.k8s.io/docs/user/quick-start/#installation


### Install Kubectl

#### For Linux AMD64 / x86_64
```bash 
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x ./kubectl
sudo mv ./kubectl /usr/local/bin/kubectl

# Test kubectl
kubectl version
```

#### For macOS using Homebrew
```bash
brew install kubectl

or

brew install kubernetes-cli

# Test kubectl
kubectl version --client

```
More installation options at https://kubernetes.io/docs/tasks/tools/#kubectl

### Install Helm3

#### For Linux AMD64 / x86_64
```bash
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
sh ./get_helm.sh

# Test Helm
helm version

```

#### For macOS using Homebrew
```bash
brew install helm

# Test Helm
helm version

```
More installation options at https://helm.sh/docs/intro/install/





