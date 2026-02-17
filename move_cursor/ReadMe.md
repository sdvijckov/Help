# Для чего

Этот скрипт предназначен для помощи в вертикальной навигации в командной строке (особенно актуально для cLI-агентов).

# Как установить

Скачать репозиторий https://github.com/sdvijckov/Help, нажав нв зелёёную кнопку  "Code" и выюрав "Downlod ZIP".
Распаковать в удобную папку.
Не нужно создавать окружение.
В командной строке (cmd) набрать букву раздела,куда распаковали репозиторий, поставить двоеточие  и нажать enter
Затем cd путь/к/папке/Help-main/move_cursor, enter. pip install -r requirements.txt,enter.
**Например** Если вы распаковали аръив в D:/Projects python, пишите в командной строке:
D: (если папка в разделе С, то нужно два раза ввполнить cd..)
cd Projects python/Help-main/move_cursor
pip install -r requirements.txt

# Как исполльзовать

Скопировать скрипт move_cursor.py в папку с проектм.
В командной строке запустить:
start "MyScrollScript" pythonw move_cursor.py
**Например** Если вы работаете над проектом в D:/Projects python/Dog_wisdom, копируйте в папку Dog_wisdom.
После чего выыполните в командной строке:
D:
cd Projects python/Dog_wisdom
start "MyScrollScript" pythonw move_cursor.py
gemini



