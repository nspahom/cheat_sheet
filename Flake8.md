<h1 style="text-align:center"> FLAKE8 </h1>

**В новом проекте создать `setup.cfg`, `tox.ini`, или `.flake8` файл для настроек**

    # Например файл tox.ini
    touch tox.ini

**В файле настроек объявить секцию flake8**

    [flake8]

**Указать список кодов, которые следует игнорировать**

    ignore = 
        # Line break occurred before a binary
        W503,
        # Missing Docstrings
        D10

**Указать какой файл нужно проверять**

    filename = 
        ./main.py

или несколько

    filename = 
        ./main.py,
        ./module.py

или папка с файлами

    filename = 
        ./src

**Максимально допустимое значение сложности Маккейба для блока кода**

    max-complexity = 10

**Установить максимальную длину строки**

    max-line-length = 79

**Добавить в список исключений по умолчанию папки и файлы**

    extend-exclude =
        legacy/,
        vendor/

**Мой базовый конфигурационный файл**

    [flake8]
    ignore = 
        # Line break occurred before a binary
        W503,
        # Missing Docstrings
        D10
    max-complexity = 10
    max-line-length = 79

<br>

[Официальная документация Flake8](https://flake8.pycqa.org/en/latest/)