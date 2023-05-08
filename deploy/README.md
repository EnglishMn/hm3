###Установка postgreSQL
- helm repo add bitnami https://charts.bitnami.com/bitnami
- helm install -f postgre/values.yaml hw-3 bitnami/postgresql -n otus-homework --create-namespace

###Установка Nginx controller (если нужно)
- helm install nginx-ingress-controller nginx-stable/nginx-ingress --namespace=otus-homework

###Деплой приложения
- helm install hw3 ./hw3 --namespace=otus-homework

###Postman collection json
- postman/otus-hw3.postman_collection.json