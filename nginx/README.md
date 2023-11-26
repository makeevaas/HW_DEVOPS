Собрать образ-докер

    - docker build -t test-nginx-image .

Запустить контейнер

    - docker run -d -p 80:80 test-nginx-image

Проверить через адресную строку браузера адрес

    - http://localhost:80 | http://127.0.0.1:80

    или через терминал

    - curl localhost:80 | 127.0.0.1:80