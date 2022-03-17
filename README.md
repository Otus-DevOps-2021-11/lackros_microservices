# lackros_microservices
lackros microservices repository

# Выполнено ДЗ по Лекции №15: Технология контейнеризации. Введение в Docker

 - [X] Основное ДЗ
 - [X] Задание со *

## В процессе сделано:
 - Установлен докер на локальную машину
 - Запущены докер-контейнеры для ознакомления с технологией
 - Сохранен собственный тестовый образ
 - Описана разница между образом и контейнером :)


# Выполнено ДЗ по Лекции №16: Docker контейнеры. Docker под капотом

 - [X] Основное ДЗ
 - [ ] Задание со *

## В процессе сделано:
 - Изучена работа с технологией docker-machine
 - Собран образ с reddit и отправлен в docker-hub
 - docker run --name reddit -d -p 9292:9292 lackros/otus-reddit:1.0

# Выполнено ДЗ по Лекции №17: Docker образы. Микросервисы

## В процессе сделано:
 - Заново создана ВМ и развернут на ней docker-machine
 - Написаны новые Docker файлы и собраны образы
 - Создана новая докер-сеть reddit
 - Запущены контейнеры в этой сети
 - Задание со звездочкой - запущены контейнеры, с другими нетворк интерфейсами
 - Оптимизирован контейнер с UI
 - Создан и подключен docker volume reddit_db - для хранения базы данных

# Выполнено ДЗ по Лекции №18: Сетевое взаимодействие Docker контейнеров. Docker Compose. Тестирование образов
 - Поработал с сетями докера none, host и bridge
 - Создал новую сеть back_net и front_net и запущены контейнеры с этими сетями
 - Установлен docker-compose, запущены контейрены через него, и потом файл docker-compose.yml параметризирован
 - Параметры указаны в файле lackros.env и lackros.env.example
 - Базовое имя образуется из имени папки с проектом src_***. Изменить можно добавив параметр -p, --project-name NAME
 - Запускается например вот так: docker-compose -p LALALA up -d
 - new line

# Выполнено ДЗ по Лекции №20: Устройство Gitlab CI. Построение процесса непрерывной интеграции
 - Развернута тестовая среда в облаке 2 ядра, 8гб оперативной памяти и 50гб hdd
 - Запущен гитлаб в докере
 - Запушен учебный гит репозиторий в гитхаб репозиторий
 - Добавлен пайплайн, указаны стадии, добавлены окружения

# Выполнено ДЗ по Лекции №22: Введение в мониторинг. Модели и принципы работы систем мониторинга
 - Развернута тестовая среда в облаке 2 ядра, 8гб оперативной памяти и 50гб hdd
 - Развернут docker-machine
 - Запущен контейнер с Prometheus, изучен интерфейс, посмотрели на метрики, посмотрели на таргеты
 - Остановили контейнер с Prometheus, навели порядок с файлами в корне дирректории с домашками
 - Собрали свой образ Prometheus с нужными нам метриками
 - Собрали наши сервисы с добавлением halthcheck'ами
 - С помощью docker-compose  запустили наше приложение и мониторинг
 - Добавили в конфиг docker-compose еще и контейнер с node_explorer
 - Отправили последние образы докер контейнеров в свой репозиторий
 - Докер хаб с моей репозиторией https://hub.docker.com/repository/docker/lackros/prometheus
