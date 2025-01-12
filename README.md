### Lesson 49

### Получаем ракету Django!

1. Установка Django:
    ```bash
    pip install django
    ```

2. Создание нового проекта в Django:
    ```bash
    django-admin startproject blog .
    ```
Вариант с тойчкой создаст новый проект в текущей директории, а вариант без точки создаст проект в директории с именем проекта.

3. Запуск сервера разработки:
    ```bash
    python manage.py runserver
    ```

4. Создание нового приложения в проекте:
    ```bash
    python manage.py startapp python_blog
    ```

**lesson_49: Создание проекта Blog и приложения python_Blog**

### INSTALLED_APPS

1. Добавили прилжение в ``INSTALLED_APPS`` в файле ``settings.py``:
2. Добавили функцию index в файле ``views.py`` в приложении ``python_blog``:
3. Импортировали функцию index в файле ``urls.py`` в приложении ``python_blog``:
4. Добавили путь к приложению в файле ``urls.py`` в проекте ``blog``:

INSTALLED_APPS - это списокк всех приложений, установленных в Django. При создании нового приложения, его необходимо добавить в ``INSTALLED_APPS`` в файле ``settings.py``:

```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'python_blog',
]
```
**lesson_49: Создание первого представления с HTTP-ответом**