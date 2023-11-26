Скачать образ postgres c docker.hub
	
	- docker pull postgres:latest

1. Cпособ без модификации образа

Запустить контейнер с помощью команды в makefile (в интсрукции make содержаться шаги для создания пользователя и бд с именем"test")

	- make postgres 

2. Способ с модификацией базового образа

Собрать новый образ на основе базового с приложенным sql файлом с основными стартовыми запросами(создание пользователя и бд)

	- docker build -t test-postgres-image .

Запустить контейнер

    - docker run -p 5432:5432 -e POSTGRES_PASSWORD=pass --name pg-container test-postgres-image	


3. Проверка

Зайти в контейнер под пользователем test и в базу test для создания запросов

	- make postgres-cli