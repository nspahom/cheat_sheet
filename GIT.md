<h1 align="center"> GIT </h1>

**Создание ssh-ключей**

    ssh-keygen
    cat .ssh/id_rsa.pub


**Настроить имя пользователя и e-mail**

    git config --global user.name "Qui-Gon Jinn"
    git config --global user.email "qgj@empire.net"

<br>

**Клонрование репозитория**

    git clone git@github.com:nspahom/cheat_sheet.git 

<br>

**Добавление одного файла**

    git add main.py

**Добавить все файлы**

    git add --all

или

    git add .  

<br>

**Проверка статуса**
    
    git status

**Коммит**
    
    # Коммит с сообщением "My first commit"
    git commit -m "My first commit"

**Пуш**
    
    git push

**Пулл**
    
    git pull

<br>

**Просмотр истории коммитов**

    git log

**Вывести на экран последний коммит**

    git show HEAD 

**Просмотр изменений в указанном коммите**

    git show a123456

<br>

**Откат изменений во всех файлах до предыдущего коммита**

    git reset HEAD

**Откат изменения конкретного файла до предыдушего коммита**

    git reset HEAD main.py

**Откат до указанного коммита**
    
    git reset a123456
