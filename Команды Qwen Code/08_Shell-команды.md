# 08_Shell-команды (!)

> Выполнение системных команд напрямую из Qwen Code

---

## Что такое Shell-команды?

Shell-команды позволяют выполнять команды операционной системы напрямую из сессии Qwen Code, используя символ `!`.

**Синтаксис:**
```
!<команда операционной системы>
```

**Пример:**
```
!git status
```

---

## Основные возможности

| Возможность | Описание |
|------------|----------|
| 🖥️ Выполнение команд | Запуск любых команд терминала/CMD |
| 📁 Работа с файлами | Создание, удаление, перемещение файлов |
| 🔧 Управление процессами | Запуск скриптов, серверов, тестов |
| 📊 Получение информации | Просмотр состояния системы, проектов |
| 🔄 Автоматизация | Комбинирование с другими командами Qwen |

---

## Базовые команды

### Просмотр содержимого директорий

**Windows (CMD/PowerShell):**
```
!dir
!dir /a
!dir /b
!tree /F
```

**Linux/Mac (Bash/Zsh):**
```
!ls
!ls -la
!ls -lh
!tree
```

**Результат:**
```
D:\Projects python\Help> !dir

 Том в папке D:\Projects python\Help

06.02.2026  10:30    <DIR>          .
06.02.2026  10:30    <DIR>          ..
06.02.2026  10:30               123 main.py
06.02.2026  10:30               456 config.json
```

---

### Навигация по директориям

**Windows:**
```
!cd
!cd ..
!cd src
!cd D:\Projects\myapp
```

**Linux/Mac:**
```
!pwd
!cd ..
!cd src
!cd /home/user/projects
```

**Важно:** Команда `cd` меняет директорию только для текущей команды. Для постоянной смены используйте `/directory`.

---

### Работа с файлами

**Создание файлов:**

**Windows:**
```
!type nul > newfile.txt
!echo Hello > file.txt
!echo World >> file.txt
```

**Linux/Mac:**
```
!touch newfile.txt
!echo "Hello" > file.txt
!echo "World" >> file.txt
```

**Копирование:**

**Windows:**
```
!copy source.txt destination.txt
!xcopy /E /I src/ backup/
```

**Linux/Mac:**
```
!cp source.txt destination.txt
!cp -r src/ backup/
```

**Перемещение:**

**Windows:**
```
!move old_path.txt new_path.txt
!ren old_name.txt new_name.txt
```

**Linux/Mac:**
```
!mv old_path.txt new_path.txt
!mv old_name.txt new_name.txt
```

**Удаление:**

**Windows:**
```
!del file.txt
!rmdir folder
!rmdir /S /Q folder
```

**Linux/Mac:**
```
!rm file.txt
!rm -rf folder
```

⚠️ **Внимание:** Удаление через `!` необратимо!

---

## Работа с Git

### Проверка состояния

```
!git status
!git log --oneline -5
!git branch -a
!git remote -v
```

**Результат:**
```
D:\Projects python\Help> !git status

On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  modified:   src/main.py
  modified:   README.md

Untracked files:
  new_feature.py
```

### Изменения

```
!git diff
!git diff HEAD
!git diff --staged
```

### Добавление и коммит

```
!git add .
!git add src/main.py
!git commit -m "Fix bug in auth module"
!git commit -am "Quick fix"
```

### Отправка и получение

```
!git push
!git push origin main
!git pull
!git fetch
```

---

## Работа с Python

### Запуск скриптов

```
!python script.py
!python -m http.server
!python -m pytest tests/
!python -m unittest discover
```

### Управление зависимостями

```
!pip install package_name
!pip install -r requirements.txt
!pip uninstall package_name
!pip list
!pip freeze > requirements.txt
```

### Виртуальные окружения

**Создание:**
```
!python -m venv venv
```

**Активация (Windows):**
```
!venv\Scripts\activate
```

**Активация (Linux/Mac):**
```
!source venv/bin/activate
```

**Проверка:**
```
!which python
!python --version
```

---

## Работа с Node.js

### Запуск и управление

```
!node app.js
!npm start
!npm run dev
!npm run build
!npm run test
```

### Управление зависимостями

```
!npm install package_name
!npm install -D dev_package
!npm uninstall package_name
!npm list
!npm update
```

### Инициализация

```
!npm init -y
!npx create-react-app my-app
!npx tsc --init
```

---

## Работа с Docker

### Управление контейнерами

```
!docker ps
!docker ps -a
!docker images
!docker run -it ubuntu bash
!docker stop container_id
!docker rm container_id
```

### Сборка и запуск

```
!docker build -t myapp .
!docker-compose up
!docker-compose up -d
!docker-compose down
```

---

## Сетевые команды

### Проверка соединения

```
!ping google.com
!ping 8.8.8.8
```

### Информация о сети

**Windows:**
```
!ipconfig
!ipconfig /all
!netstat -an
```

**Linux/Mac:**
```
!ifconfig
!ip addr
!netstat -tulpn
```

### DNS и маршруты

```
!nslookup google.com
!tracert google.com      # Windows
!traceroute google.com   # Linux/Mac
```

---

## Системная информация

### ОС и версия

**Windows:**
```
!ver
!systeminfo
!wmic os get Caption,Version
```

**Linux/Mac:**
```
!uname -a
!cat /etc/os-release
!hostname
```

### Ресурсы

**Windows:**
```
!tasklist
!taskmgr
```

**Linux/Mac:**
```
!top
!htop
!ps aux
```

### Дисковое пространство

**Windows:**
```
!wmic logicaldisk get size,freespace,caption
```

**Linux/Mac:**
```
!df -h
!du -sh *
```

---

## Продвинутое использование

### Конвейеры (Pipes)

**Linux/Mac:**
```
!ls -la | grep ".py"
!ps aux | grep python | wc -l
!cat file.txt | sort | uniq
```

**Windows (PowerShell):**
```
!dir | findstr ".py"
!Get-Process | Where-Object {$_.CPU -gt 100}
```

### Перенаправление вывода

**В файл:**
```
!dir > file_list.txt
!pip list > requirements.txt
!git log > changelog.md
```

**Добавление в файл:**
```
!echo "New line" >> file.txt
!git log --oneline >> changelog.md
```

### Комбинирование команд

**Windows (CMD):**
```
!cd src && python main.py
!mkdir backup && copy *.txt backup\
```

**Linux/Mac:**
```
!cd src && python main.py
!mkdir -p backup && cp *.txt backup/
```

**Последовательное выполнение:**
```
!npm install && npm run build && npm start
```

---

## Практические примеры

### 1. Инициализация проекта

```
# Python проект
!python -m venv venv
!venv\Scripts\activate
!pip install flask
!pip freeze > requirements.txt

# Node.js проект
!npm init -y
!npm install express
!npm install -D nodemon
```

### 2. Git рабочий процесс

```
!git status
!git add .
!git commit -m "Add new feature"
!git push origin main
```

### 3. Запуск тестов

```
# Python
!pytest tests/ -v
!python -m unittest discover

# Node.js
!npm test
!npx jest
```

### 4. Сборка проекта

```
# TypeScript
!npx tsc

# Python (создание дистрибутива)
!python setup.py sdist bdist_wheel

# Docker
!docker build -t myapp:latest .
```

### 5. Развёртывание

```
!git pull origin main
!pip install -r requirements.txt
!python migrate.py
!systemctl restart myapp
```

### 6. Резервное копирование

```
# Windows
!mkdir backup_%date:~0,10%
!xcopy /E /I src backup_%date:~0,10%\

# Linux/Mac
!mkdir backup_$(date +%Y%m%d)
!cp -r src backup_$(date +%Y%m%d)/
```

---

## Комбинация с другими командами Qwen

### С File-командами (@)

```
!ls src/
@src/main.py  # Открыть найденный файл
```

```
!git diff HEAD
@src/changed_file.py  # Проанализировать изменения
```

### С `/memory`

```
!python --version
/memory add Проект использует Python 3.11
```

### С `/tools`

```
!ls -la
/tools  # Проверить доступные инструменты для работы с файлами
```

---

## Советы по использованию

### ✅ Лучшие практики

1. **Проверяйте команды перед запуском** — особенно удаляющие.
   ```
   !rm -rf folder/  ❌ (опасно без проверки)
   !ls folder/      ✅ (проверка сначала)
   !rm -rf folder/  ❌ (только если уверены)
   ```

2. **Используйте относительные пути** — для переносимости.
   ```
   !cd src && python main.py  ✅
   !cd D:\Projects\...\src    ❌
   ```

3. **Комбинируйте с Git** — всегда коммитьте перед изменениями.
   ```
   !git add . && git commit -m "Before major changes"
   ```

4. **Проверяйте вывод** — смотрите на результат команд.

5. **Используйте `&&` для цепочек** — но не переусердствуйте.
   ```
   !npm install && npm run build  ✅
   !cmd1 && cmd2 && cmd3 && ...   ❌ (слишком длинно)
   ```

---

### ⚠️ Предостережения

**Опасные команды:**
```
!rm -rf /              # Удалит всё на Linux/Mac
!del /S /Q C:\*        # Удалит всё на Windows
!format C:             # Отформатирует диск
```

**Всегда проверяйте:**
- Путь перед удалением
- Флаги команд (особенно `-f`, `-rf`)
- Текущую директорию (`!pwd` или `!cd`)

---

### 🔐 Безопасность

1. **Не выполняйте команды из непроверенных источников.**

2. **Не копируйте слепо команды из интернета.**

3. **Проверяйте каждую команду перед запуском.**

4. **Используйте `/approval-mode plan`** для проверки.

5. **Делайте бэкапы** перед крупными изменениями.

---

## Решение проблем

### Команда не найдена

**Ошибка:**
```
❌ 'python' is not recognized as an internal or external command
```

**Решение:**
1. Проверьте установку программы
2. Добавьте в PATH
3. Используйте полный путь
   ```
   !C:\Python39\python.exe script.py
   ```

---

### Отказано в доступе

**Ошибка:**
```
❌ Access is denied.
❌ Permission denied
```

**Решение:**
1. Запустите терминал от имени администратора
2. Проверьте права на файл/папку
3. Используйте `sudo` (Linux/Mac)
   ```
   !sudo command
   ```

---

### Неправильный синтаксис

**Ошибка:**
```
❌ The syntax of the command is incorrect.
```

**Решение:**
1. Проверьте синтаксис для вашей ОС
2. Windows и Linux имеют разные команды
3. Используйте `!help` для справки

---

