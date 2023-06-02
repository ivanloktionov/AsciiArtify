# Install and work wih ArgoCD:
**According to https://argo-cd.readthedocs.io/en/stable/**
> sudo kubectl create namespace argocd
> sudo kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

**According to https://argo-cd.readthedocs.io/en/stable/getting_started/**
> sudo kubectl port-forward svc/argocd-server -n argocd 8080:443

**Also, for gif recording sync timeout has been changed to 5s**:
sudo kubectl patch cm argocd-cm -n argocd -p '{"data":{"timeout.reconciliation":"5s"}}'

![simplescreenrecorder-2023-06-02_07 12 22](https://github.com/ivanloktionov/AsciiArtify/assets/71848058/18b5c573-3280-407e-81c2-7cc5916960da)
