* Проект ImageHosting *
* Проект запускается с помощью одной команды: docker compose up --build. Остановка: docker compose down

* Структура проекта:
- docker-compose.yml — конфигурация сервисов.
- app/ — код Python-бэкенда
- nginx — конфигурация Nginx.
- images — директория для хранения загруженных изображений.
-  logs — директория для хранения логов.
-  static - код фронтенда
* Описание маршрутов и их функциональности:
-  POST /upload — загрузка изображения (поддерживаемые форматы: .jpg, .png, .gif; максимальный размер: 5 МБ). 
- GET /images/<имя_файла> — доступ к загруженным изображениям через Nginx.
- DELETE /delete/<имя_файла> - удаление файла
* Используеться база данных PostgreSQLЖ
- id - уникальный номер 
- filename - имя файла 
- original_name - исходное имя 
- size - размер в байтах 
- upload_time - дата загрузки 
- file_type - тип файла

       

