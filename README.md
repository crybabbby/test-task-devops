Простое веб-приложение, доступное пользователю через
nginx, запущенные в Docker-контейнерах.

Краткая схема:
  
  Клиент    ────▶   Nginx    ────▶   Python    
            ◀────   :80      ◀────  Backend   
                                       :8080     

Как запустить:
#Клонируем репо
git clone <repository-url>
cd test-task-devops

#Запуск
docker-compose up --build

#Запуск в фоне
docker-compose up -d --build

Проверка : curl http://localhost | Ожидаемый ответ: Hello from Effective Mobile! Made by Kirill Tolmachev

Структура проекта:

test-task-devops/
├── backend/             
│   ├── Dockerfile       # Dockerfile для Python
│   └── webapp.py        # HTTP сервер на Python
├── nginx/               
│   └── nginx.conf       # Конфиг Nginx
├── docker-compose.yml   # Docker Compose ямлик
└── README.md            # Документация

Автор: Kirill Tolmachev
Тестовое задание для Effective Mobile

