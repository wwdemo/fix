# fix

Restart ICP:<br>
kubectl -s http://127.0.0.1:8888 delete pods --namespace=kube-system \`kubectl -s http://127.0.0.1:8888 get pods --namespace=kube-system | awk '{print $1}'\`

Restart Acme Air:<br>
kubectl -s http://127.0.0.1:8888 delete pods --namespace=default \`kubectl -s http://127.0.0.1:8888 get pods --namespace=default | awk '{print $1}'\`
