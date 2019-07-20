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

# Безопасность в kubernetes

- создан Service Account bob с добавление в группу admin
- создан Service Account dave
- создан Namespace prometheus
- создан Service Account carol
- создана роль с правами на чтение всех подов
- добавлен Service Account prometheus в созданную группу на чтение всех подов
- создан Namespace dev
- создан Service Account jane, права admin ns-dev
- создан Service Account ken, права view ns-dev
