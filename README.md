# Домашнее задание к лекции «Docker»
Инструкцию по выполнению домашних работ вы найдете на главной странице репозитория.

Задание 1
Аналогично данному уроку создайте свой образ docker с http-сервером nginx. Заменить страницу приветсвия Nginx на свою (изменить текст приветствия на той же странице).

Подсказки:
Для проверки присылается GitHub-репозиторий с Dockerfile и статичными файлами для него.

Для пользовательского html можно использовать пример в каталоге с ДЗ.

Задание 2
Создайте контейнер для сервера REST API для любого проекта из курса на Django (например, CRUD: Склады и запасы ).

ВАЖНО : поменяйте БД с postgresql на sqlite3. Чтобы ваш контейнер мог работать независимо от postgres (с этим мы разберемся на следующей занятии).

Проверьте конфигурацию Django при использовании среды окружения.

Приложите репозиторий Dockerfile и файлы приложения.
В README.md описаны типовые команды для запуска контейнера c backend-сервером.



### Сборка образа
docker build . --tag=f1:v1

### Запуск контейнера
docker run --name my_dockers -d -p 8000:8000 f1:v1 
