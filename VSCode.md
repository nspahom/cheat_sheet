<h1 align="center"> Visual Studio Code </h1>


<h2 align="center"> Настройки текущего проекта </h2>

**Открыть json файл настроек для текущего проекта - нажать `Ctrl + Shift + P` и ввести команду:**

    Preferences: Open Workspace Settings (JSON)

**Включить flake8**

    "python.linting.flake8Enabled": true


**Включить автоматическую проверку линтерами**

    "python.linting.enabled": true

**Добавить вертикальную линию для визуального ограничения длины строки 79 символов**

    "[python]": {
        "editor.rulers": [79]
    }

**Скрыть из Explorer VS Code некоторые папки и файлы**

    "files.exclude": {
        "**/__pycache__": true,
        ".venv": true,
        ".mypy_cache": true,
        ".vscode":true
    }

<br>

**Мой итоговый файл settings.json для текущего проекта**

    {
        "python.linting.flake8Enabled": true,
        "python.linting.enabled": true,
        "[python]": {
            "editor.rulers": [79]
        },
        "files.exclude": {
            "**/__pycache__": true,
            ".venv": true,
            ".mypy_cache": true,
            ".vscode":true
        }
    }

<br>

[Официальная документация VS Code](https://code.visualstudio.com/docs)