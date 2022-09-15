<h1 align="center"> Poetry


<h2 align="center"> Установка </h2>

**Официальный установщик**

    curl -sSL https://install.python-poetry.org | python3 -

**или**

    pip install poetry

<br><h2 align="center" style=''> Общие настройки </h2>

**Включить автодополнение**

    poetry completions bash >> ~/.bash_completion

**Создавать папку с виртуальным окружением в папке с проектом**

    poetry config virtualenvs.in-project true

<br><h2 align="center" style=''> Первоначальная настройка проекта </h2>

**Новый проект**

    poetry new project_name

**Существующий проект, в корневой папке проекта**

    poetry init

**Если нет виртуального окружения (указать версию интерпретатора)**

    poetry env use python3.7

**Установка линтеров**

    poetry add -D flake8 mypy
	
<br>

### Установка плагинов к линтерам ###
	
**Для любого python-проеĸта**

    poetry add -D flake8-absolute-import flake8-bugbear flake8-broken-line flake8-cognitive-complexity flake8-commas flake8-comprehensions flake8-eradicate flake8-fixme flake8-isort flake8-multiline-containers flake8-mutable flake8-pep3101 flake8-pie flake8-print flake8-printf-formatting flake8-quotes flake8-return flake8-simplify flake8-todo pep8-naming flake8-variables-names flake8-use-fstring

**Если пишете доĸстринги**

    poetry add -D flake8-docstrings

**Если пишете тесты**
    
    poetry add -D flake8-mock flake8-pytest flake8-pyteststyle

**Если Python версии 3.8 и выше**

    poetry add -D flake8-walrus 

**Если django-проект**

    poetry add -D flake8-django

**Если fastapi-проект**

    poetry add -D flake8-fastapi
																						

<br><h2 align="center" style=''> Использование poetry в проекте </h2>

**Установка новых зависимостей (например Pydantic)**

    poetry add pydantic

**Установка новых DEV зависимостей (например pytest)**

    poetry add -D pytest

**Установка новых зависимостей из requirements.txt**

    poetry add `cat requirements.txt`

**Удалить зависимость (например Pydantic)**

    poetry remove pydantic


<br>


**Установить все зависимости из poetry.lock или pyproject.toml**

    poetry install

**Установить зависимости кроме DEV из poetry.lock или pyproject.toml**

    poetry install --without dev

**Синхронизировать зависимости в env**

    poetry install --sync

**Синхронизировать зависимости в env кроме DEV**

    poetry install --without dev --sync


<br>


**Запуск python файла**

    poetry run python3 main.py

**Запуск тестов (например pytest)**

    poetry run pytest

**Запуск линтеров (например flake8)**
    
    poetry run flake8 main.py

**Активация env**

    poetry shell

**Обновить зависимости проекта**

    poetry update

**Показать дерево зависимостей**

    poetry show --tree

**Показать настройки poetry**

    poetry config --list

**Показать виртуальные окружения проекта**

    poetry env list

<br>

 [Официальная документация Poetry](https://python-poetry.org/docs)
