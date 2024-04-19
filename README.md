# Nginx Ingress Helm

- Nginx Helm
```bash
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
helm repo update
helm repo ls
helm search repo ingress-nginx
helm search repo ingress-nginx --versions
helm show values ingress-nginx/ingress-nginx --version 4.10.0
helm upgrade --install nginx-ingress ingress-nginx/ingress-nginx --version 4.10.0 --namespace nginx-ingress --create-namespace -f values.yaml --wait
```
