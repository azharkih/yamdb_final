![workflow](https://github.com/azharkih/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg)
# API yamdb

## Краткое описание проекта
API предназначено для обмена информацией об оценках произведений пользователями 
и комментариев этих оценок

### Запуск приложения
После запуска приложения необходимо ввести следующие команды:
```
docker-compose exec web python manage.py migrate --noinput
docker-compose exec web python manage.py collectstatic --no-input
```

### Создание суперпользователя
Для создания суперпользователя необходимо ввести следующую команду:
```
docker-compose exec web python manage.py createsuperuser
```

### Заполнение базы начальными данными
Для наполнения базы начальными данными выполнить команду:
```
docker-compose exec web python manage.py loaddata fixtures.json
```

### Рабочий проект

С примером работы проекта можно ознакомится по ссылке: http://84.252.132.252/admin/
