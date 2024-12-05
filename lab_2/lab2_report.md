University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FICT](https://fict.itmo.ru)\
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)\
Year: 2024/2025\
Group: K4110c\
Author: Krapivin Vladislav Valerievich\
Lab: Lab1\
Date of create: 3.12.2024\
Date of finished:

___
# Лабораторная работа №2 "Развертывание веб сервиса в Minikube, доступ к веб интерфейсу сервиса. Мониторинг сервиса."
## Цель работы
Ознакомиться с типами "контроллеров" развертывания контейнеров, ознакомится с сетевыми сервисами и развернуть свое веб приложение.
## Ход работы
### 1. Запуск Minikube 



### 2. Создание манифеста Deployment.yaml в котором описываются Deployment и Service 



### 3. Применение конфигурационного файла формата .yaml



### 4. Прокидывание порта "Port-forwarding"



### 5. Подключение к контейнерам через веб браузер. 



## Выводы
- Среди параметров `REACT_APP_USERNAME`, `REACT_APP_COMPANY_NAME` и `Container name` изменяется только последний, поскольку сервис может обращаться к любому из подов в ReplicaSet. В нашем случае ReplicaSet состоит из 2 подов.



