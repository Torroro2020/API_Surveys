# API_Surveys
Тестовое задание для компании "Фабрика Решений"
# Необходимые действия перед началом
cd API_Surveys
pip install -r requirements.txt
cd Questionnaire
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
Создаём супер-юзера с именем admin и паролем admin. Это имя и пароль будут использоваться в тестах (см. tests/settings.py).

Запуск сервера
cd API_Surveys/Questionnaire
python manage.py runserver
Запуск тестов
Тесты следует запускать при работающем сервере.

cd API_Surveys/tests
pytest
