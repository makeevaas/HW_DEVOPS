Скачать образ postgres c docker.hub
	
	- docker pull postgres:latest

Запустить контейнер с помощью команды в makefile (в инструкции make содержатся шаги для создания пользователя и бд с именем "test")

	- make postgres 

Зайти в контейнер под пользователем test в базу test для создания запросов

	- make postgres-cli
