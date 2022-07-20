# Yudalx_platform
Yudalx Platform repository

HomeWork №1

- Написан Dockerfile который собирает контейнер с nginx
- Ссылка на образ devopstank/nginx-base-app:1.1
- Написан конфиг для nginx default.conf для отдачи файлов помещенных по пути /app
- Написан манифест web-pod.yaml для запуска контейнера с nginx в k8s
- Запушен образ с hipster-frontend devopstank/microservices-demo-frontend
- Добавлены env в сгенеренный манифест hipster-frontend

HomeWork №2
ReplicaSet не отслеживает изменения в podSpec, по этому изменение ссылки на образ не ведет к пересозданию подов
- Написан манифест для деплоя frontend, как через ReplicaSet так и Deployment
- Написан манифест для деплоя paymentservice, как через ReplicaSet так и Deployment
- В манифесте paymentservice-deployment-bg.yaml реализован деплой через blue-green
- В манифесте paymentservice-deployment-reverse.yaml реализован деплой через rollingUpdate с недоступностью максимум одного пода
- Написан манифест node-exporter-daemonset для деплоя node-exporter на все ноды в кластере, включая мастер ноды

HomeWork №3
- Написал манифесты для усвоения работы Role, ClusterRole, RoleBinding, ClusterRoleBinding

HomeWork №4


HomeWork №5
- Создан StatefulSet и Service для Minio
- Чувствительная информация помещена в Secret
