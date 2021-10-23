# Домашнее задание к занятию "09.01 Жизненный цикл ПО"

## Подготовка к выполнению
1. Получить бесплатную [JIRA](https://www.atlassian.com/ru/software/jira/free)
![Screenshot](1-1.png)
2. Настроить её для своей "команды разработки"
3. Создать доски kanban и scrum

## Основная часть
В рамках основной части необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить следующий жизненный цикл:
1. Open -> On reproduce
2. On reproduce <-> Open, Done reproduce
3. Done reproduce -> On fix
4. On fix <-> On reproduce, Done fix
5. Done fix -> On test
6. On test <-> On fix, Done
7. Done <-> Closed, Open
![Screenshot](2-1.png)

Остальные задачи должны проходить по упрощённому workflow:
1. Open -> On develop
2. On develop <-> Open, Done develop
3. Done develop -> On test
4. On test <-> On develop, Done
5. Done <-> Closed, Open
![Screenshot](2-2.png)

Создать задачу с типом bug,
![Screenshot](2-3-1.png)
попытаться провести его по всему workflow до Done. 
![Screenshot](2-3-2.png)
Создать задачу с типом epic, к ней привязать несколько задач с типом task, провести их по всему workflow до Done. При проведении обеих задач по статусам использовать kanban. Вернуть задачи в статус Open.
![Screenshot](2-3-3.png)
![Screenshot](2-3-3-1.png)
![Screenshot](2-3-3-2.png)
![Screenshot](2-3-3-3.png)

Перейти в scrum, запланировать новый спринт, состоящий из задач эпика и одного бага, стартовать спринт, провести задачи до состояния Closed. Закрыть спринт.
![Screenshot](2-4.png)
![Screenshot](2-5.png)
![Screenshot](2-6.png)


Если всё отработало в рамках ожидания - выгрузить схемы workflow для импорта в XML. Файлы с workflow приложить к решению задания.

К сожалению в моей JIRA не нашел способа выгрузки в XML своих workflow, нужных кнопок в настройках(которые были у преподавателя в его версии во время демонстрации) у меня не было.

---

