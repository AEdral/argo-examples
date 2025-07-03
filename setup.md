minikube start

kubectl get services -n argocd

kubectl port-forward service/argocd-server -n argocd 8080:443

kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d



kubectl get all -n dev

kubectl port-forward service/myhelmapp 8888:80 -n dev

