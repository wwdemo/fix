# fix

kubectl -s http://127.0.0.1:8888 delete pods --namespace=default `kubectl -s http://127.0.0.1:8888 get pods --namespace=default | awk '{print $1}'`
