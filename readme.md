k3d cluster create default --agents 3 --registry-create

kubectl create ns argocd

kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl -n argocd apply -f argocd-ingress.yaml 

