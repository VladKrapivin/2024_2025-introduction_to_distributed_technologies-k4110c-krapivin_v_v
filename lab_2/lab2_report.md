University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FICT](https://fict.itmo.ru)\
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)\
Year: 2024/2025\
Group: K4110c\
Author: Krapivin Vladislav Valerievich\
Lab: Lab2\
Date of create: 3.12.2024\
Date of finished:

___
# Лабораторная работа №2 "Развертывание веб сервиса в Minikube, доступ к веб интерфейсу сервиса. Мониторинг сервиса."
## Цель работы
Ознакомиться с типами "контроллеров" развертывания контейнеров, ознакомится с сетевыми сервисами и развернуть свое веб приложение.
## Ход работы
### 1. Запуск Minikube 

![Minikube](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/start.png)

### 2. Создание манифеста Deployment.yaml в котором описываются Deployment и Service 
- В качестве сервиса был выбран ClusterIP - тип сервиса по умолчанию.

![Deployment](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/yaml.png)

### 3. Применение конфигурационного файла формата .yaml

![Apply](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/apply.png)


### 4. Прокидывание порта "Port-forwarding"

![Port-Forwarding](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/port-forward.png)


### 5. Подключение через веб браузер. 

![React app](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/reactapp.png)

### 6. Логи подов 

![Logs](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/logs.png)

## Выводы
- Среди параметров `REACT_APP_USERNAME`, `REACT_APP_COMPANY_NAME` и `Container name` изменяется только последний (как и IP), поскольку сервис может обращаться к любому из подов в ReplicaSet. В нашем случае ReplicaSet состоит из 2 подов: 65t4f и 9sz5l.

![React app](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/pods.png)

## Схема организации контейнеров и сервисов

![Scheme](https://github.com/VladKrapivin/2024_2025-introduction_to_distributed_technologies-k4110c-krapivin_v_v/blob/main/lab_2/pics/Схема%20организации%20контейнеров%20и%20сервисов.drawio.png)
