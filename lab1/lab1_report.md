University: [ITMO University](https://itmo.ru/ru/) <br>
Faculty: [FICT](https://fict.itmo.ru) <br>
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024 <br>
Group: K4111c <br>
Author: Ivanov Alexander Anatolievich <br>
Lab: Lab1 <br>
Date of create: 14.03.2024 <br>
Date of finished:  <br>


1. Была произведена установка minikube, после чего он был запущен с помощью команды "minikube start"
![alt text](images/image.png)

2. Был установлен контейнер vault
![alt text](images/image-1.png)

3. Был создан yaml манифест для создания Deployment, который является объектом Kubernetes, представляющим работающее приложение в кластере
![alt text](images/image-2.png)

4. После чего он был развернут в кластере 
![alt text](images/image-3.png)

5. Был создан сервис для доступа к этому контейнеру и к нем был проброшен 8200 порт, благодаря чему vault стал доступен по данному порту в браузере.

![alt text](images/image-4.png)


![alt text](images/image-5.png)

6. Чтобы получить токен для входа в vault были открыты и изучены логи пода, которые были найдены через графический интерфейс. Его можно запустить с помощью команды "minkube dashboard"
![alt text](images/image-6.png)

7. Был произведен вход в vault посредством полученного токена

![alt text](images/image-7.png)

Ответы на вопросы:

1. Было развернуто приложение для хранения секретов Vault в Kubernetes. Для этого был развернут один объект Deployment с двумя репликами пода, после чего для доступа к этому объекту был поднят специальный сервис, к которому был прокинут хостовой порт 8200 из-за чего он стал доступен с браузера.

2. Токен для входа в Vault хранится в логах пода

Схема

![alt text](images/image-8.png)