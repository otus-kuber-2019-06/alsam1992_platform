# alsam1992_platform
alsam1992 Platform repository

# Знакомство с Kubernetes.

- Установлен kubectl.
- Настроен Kubectl Autocomplete для bash.
- Установлен minicube.
- Установлен Web UI Dashboard для Kubernetes.
- Создан docker образ alsam/alex:latest.
- Создан и применен манифест web-pod.yaml.
- Проверена работа web сервера развернутого из манифеста web-pod.yaml с помощью `kubectl port-forward --address 0.0.0.0 pod/web 8000:8000`
- Сoredns восстанавливается, т.к. управляется через Deployment который при развернтвании автоматитчески создает соответствующий ReplicaSet.
