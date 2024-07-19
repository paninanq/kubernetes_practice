# Задача
Поднять microk8s
Запустить в нем postgresql
Запустить grafana так, чтобы её база выла в postgresql
# Решение

`microk8s.start`

`microk8s add-node`

Написала .yaml файлы для поднятия postgre, grafana, ingress

`microk8s kubectl apply -f db_service.yaml`

`microk8s kubectl apply -f db_deployment.yaml`

`microk8s kubectl apply -f grafana_service.yaml`

`microk8s kubectl apply -f grafana_deployment.yaml`

`microk8s kubectl apply -f ingress.yaml`
