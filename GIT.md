<h1 align="center"> GIT </h1>

**Создание ssh-ключей**

    ssh-keygen
    cat .ssh/id_rsa.pub


**Настроить имя пользователя и e-mail**

    git config --global user.name "Стас Басов"
    git config --global user.email "stas.basov@whatever.com"

<br>

**Клонрование репозитория**

    git clone git@github.com:ваш-аккаунт-на-гитхабе/backend_test_homework.git 

<br>

**Добавление файлов**

    # добавили файл "program.py"
    git add program.py

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

<br>

**Просмотр истории коммитов**

    git log

**Вывести на экран последний коммит**

    git show HEAD 

**Просмотр изменений в указанном коммите**

    git show c952d96

<br>

**Откат изменений во всех файлах до предыдущего коммита**

    git reset HEAD

**Откат изменения конкретного файла до предыдушего коммита**

    git reset HEAD program.py

**Откат до указанного коммита**
    
    git reset 97a25f7 
