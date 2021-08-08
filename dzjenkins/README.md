# Домашнее задание к занятию "09.03 Jenkins"

## Подготовка к выполнению

1. Установить jenkins по любой из [инструкций](https://www.jenkins.io/download/)
![Screenshot](1-1.png)
2. Запустить и проверить работоспособность
3. Сделать первоначальную настройку
4. Настроить под свои нужды
![Screenshot](1-2-3-4.png)
5. Поднять отдельный cloud
![Screenshot](1-5.png)
6. Для динамических агентов можно использовать [образ](https://hub.docker.com/repository/docker/aragast/agent)
7. Обязательный параметр: поставить label для динамических агентов: `ansible_docker`
![Screenshot](1-7.png)
8.  Сделать форк репозитория с [playbook](https://github.com/aragastmatb/example-playbook)
![Screenshot](1-8-1.png)
![Screenshot](1-8-2.png)

## Основная часть

1. Сделать Freestyle Job, который будет запускать `ansible-playbook` из форка репозитория
![Screenshot](2-1-1.png)
![Screenshot](2-1-2.png)
![Screenshot](2-1-3.png)
2. Сделать Declarative Pipeline, который будет выкачивать репозиторий с плейбукой и запускать её
![Screenshot](2-2-1.png)
![Screenshot](2-2-2.png)
![Screenshot](2-2-3.png)
3. Перенести Declarative Pipeline в репозиторий в файл `Jenkinsfile`
![Screenshot](2-3.png)
4. Перенастроить Job на использование `Jenkinsfile` из репозитория
![Screenshot](2-4-1.png)
![Screenshot](2-4-2.png)
![Screenshot](2-4-3.png)
5. Создать Scripted Pipeline, наполнить его скриптом из [pipeline](./pipeline)
![Screenshot](2-5.png)
6. Заменить credentialsId на свой собственный
![Screenshot](2-6-1.png)
![Screenshot](2-6-2.png)
7. Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозитрий в файл `ScriptedJenkinsfile`
![Screenshot](2-7.png)
8. Отправить ссылку на репозиторий в ответе
https://github.com/AlexanderSpitsyn07/myjenk
