# Домашнее задание к занятию "09.04 Teamcity"

## Подготовка к выполнению

1. Поднимите инфраструктуру [teamcity](./teamcity/docker-compose.yml)
![Screenshot](1-1-2.png)
2. Если хочется, можете создать свою собственную инфраструктуру на основе той технологии, которая нравится. Инструкция по установке из [документации](https://www.jetbrains.com/help/teamcity/installing-and-configuring-the-teamcity-server.html)
3. Дождитесь запуска teamcity, выполните первоначальную настройку
![Screenshot](1-3.png)
4. Авторизуйте агент
![Screenshot](1-4.png)
5. Сделайте fork [репозитория](https://github.com/aragastmatb/example-teamcity)
![Screenshot](1-5.png)

## Основная часть

1. Создайте новый проект в teamcity на основе fork
![Screenshot](2-1.png)
2. Сделайте autodetect конфигурации
![Screenshot](2-2.png)
3. Сохраните необходимые шаги, запустите первую сборку master'a
![Screenshot](2-3.png)
4. Поменяйте условия сборки: если сборка по ветке `master`, то должен происходит `mvn clean package`, иначе `mvn clean test`
![Screenshot](2-4-1.png)
![Screenshot](2-4-2.png)
5. Мигрируйте `build configuration` в репозиторий
![Screenshot](2-5-1.png)
![Screenshot](2-5-2.png)
6. Создайте отдельную ветку `feature/add_reply` в репозитории
![Screenshot](2-6.png)
7. Напишите новый метод для класса Welcomer: метод должен возвращать произвольную реплику, содержащую слово `hunter`
![Screenshot](2-7.png)
8. Дополните тест для нового метода на поиск слова `hunter` в новой реплике
![Screenshot](2-8.png)
9. Сделайте push всех изменений в новую ветку в репозиторий
![Screenshot](2-9-1.png)
![Screenshot](2-9-2.png)
10. Убедитесь что сборка самостоятельно запустилась, тесты прошли успешно
![Screenshot](2-10.png)
11. Внесите изменения из произвольной ветки `feature/add_reply` в `master` через `Merge`
![Screenshot](2-11-1.png)
![Screenshot](2-11-2.png)
12. Убедитесь, что нет собранного артефакта в сборке по ветке `master`
13. Настройте конфигурацию так, чтобы она собирала `.jar` в артефакты сборки
![Screenshot](2-13.png)
14. Проведите повторную сборку мастера, убедитесь, что сбора прошла успешно и артефакты собраны
![Screenshot](2-14.png)
15. Проверьте, что конфигурация в репозитории содержит все настройки конфигурации из teamcity
16. В ответ предоставьте ссылку на репозиторий
https://github.com/AlexanderSpitsyn07/teamcity


