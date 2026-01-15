Простое веб-приложение, доступное пользователю через
nginx, запущенные в Docker-контейнерах.

Краткая схема:
  
Client -> nginx(:80) -> PythonBackend(:8080) 

Как запустить:

#Клонируем репо

git clone (repo_url)

cd test-task-devops

#Запуск

docker-compose up --build

#Запуск в фоне

docker-compose up -d --build

Проверка : curl http://localhost | Ожидаемый ответ: Hello from Effective Mobile! Made by Kirill Tolmachev

Автор: Kirill Tolmachev |
Тестовое задание для Effective Mobile

