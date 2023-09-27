docker build -t abauruel/gitops:latest .

docker run --rm -p 8080:8080 abauruel/gitops:latest 

docker push abauruel/gitops:latest

### Criando cluster K8S 
kind create cluster --name=gitops   
### apply context
kubectl cluster-info --context kind-gitops

## install kustomize
brew install kustomize