# challenge-ci-cd

kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

argocd admin initial-password -n argocd

kubectl port-forward svc/argocd-server -n argocd <exposed-port-to>:443
