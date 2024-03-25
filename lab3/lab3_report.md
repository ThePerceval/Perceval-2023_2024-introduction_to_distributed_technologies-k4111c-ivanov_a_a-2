University: [ITMO University](https://itmo.ru/ru/) <br>
Faculty: [FICT](https://fict.itmo.ru) <br>
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024 <br>
Group: K4111c <br>
Author: Ivanov Alexander Anatolievich <br>
Lab: Lab3 <br>
Date of create: 15.03.2024 <br>
Date of finished:  <br>


**1. Создаём ConfigMap со значениями переменных.** 
ConfigMap — это объект Kubernetes, который используется для хранения несекретных данных в паре «ключ-значение». Поды могут использовать их как переменные окружения или как файлы конфигурации в Volume.<br>

![alt text](images/image.png)

**2. Создаём ReplicaSet, в который передаём указанные переменные.** 
ReplicaSet — это процесс, который запускает несколько экземпляров модуля pod и сохраняет указанное количество модулей pod постоянными<br>

![alt text](images/image-1.png)

**3. Создаем Service для доступа к приложению**<br>
Сервис Kubernetes (Service) — это уровень абстракции, который определяет логический набор подов, перенаправляет внешний трафик, балансирует нагрузку и реализует service discovery для этих подов

![alt text](images/image-2.png)

**4. Создаем сертификат и импортируем его в Secret**<br>
В кластере Kubernetes объекты типа секрет Secret предназначены для хранения конфиденциальной информации, такой как пароли, OAuth-токены или ssh-ключи.

![alt text](images/image-3.png)

**5. Создаем Ingress и указываем в нем созданный секрет и домен** <br>
Ingress— это набор правил внутри вашего кластера, предназначенных для того, чтобы входящие подключения могли достичь сервисов (Services) ваших приложений.

![alt text](images/image-4.png)

**6. Применяем все вышенаписанные манифесты, для создания всех объектов и проверяем их создание** <br>

![alt text](images/image-5.png)

**7. Включаем в minikube аддон с ingress.**<br>

![alt text](images/image-7.png)

**8. Прописываем в файле /etc/hosts адрес minikube и домен** <br>

![alt text](images/image-6.png)

**9. Включаем туннель в minikube и переходим в бразуере по адресу `https://lab3-app.info`.** <br>

![alt text](images/image-8.png)

![alt text](images/image-9.png)

**10. Сертификат.**<br>
![alt text](images/image-10.png)

**11. Схема.**<br>
![alt text](images/image-11.png)







