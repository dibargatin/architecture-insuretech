# Инструкция

## Запуск приложения

```
minikube start
minikube addons enable metrics-server

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f hpa-memory.yaml

minikube service scaletestapp-service

minikube dashboard
```

## Запуск нагрузочного теста

```
locust
```