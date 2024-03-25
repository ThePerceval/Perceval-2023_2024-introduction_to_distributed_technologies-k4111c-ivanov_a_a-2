University: [ITMO University](https://itmo.ru/ru/) <br>
Faculty: [FICT](https://fict.itmo.ru) <br>
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024 <br>
Group: K4111c <br>
Author: Ivanov Alexander Anatolievich <br>
Lab: Lab4 <br>
Date of create: 15.03.2024 <br>
Date of finished:  <br>

1.Запускаем minikube с подключенным плагином CNI=calico, режимом работы Multi-Node Clusters и разворачиваем 2 ноды 

![alt text](images/image.png)

2.Проверяем количество нод и подов calico

![alt text](images/image-1.png)

3.Помечаем ноды по географическому положению

![alt text](images/image-2.png)

4.Создание файла манифеста для назначения пула IP узлам на основе их меток.

![alt text](images/image-3.png)

5.Удаляем дефолтный Ippools перед созданием своих и создаем свои

![alt text](images/image-4.png)
![alt text](images/image-5.png)

6.Создаем деплоймент приложения

![alt text](images/image-6.png)

7.Проверяем, какие ip адреса были назначены. Адреса из тех ippool которые мы создавали, следовательно, всё настроено верно.

![alt text](images/image-7.png)

8.Создаем сервис и прокидываем 3000 порт

![alt text](images/image-8.png)

9.Заходим на сайт и видим, что все настроено верно и ip контейнера назначен верно. Container name и Container IP могут меняться, в зависимости от того, на какой под попал запрос.

![alt text](images/image-9.png)

10.Заходим в один из подов и пингуем соседний 
![alt text](images/image-10.png)

11. Схема

![alt text](images/image-11.png)
