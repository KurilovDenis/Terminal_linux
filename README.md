Linux terminal (GitBash) commands

Посмотреть где я pwd

Создать папку mkdir qa_a/

Зайти в папку cd qa_a/

Создать 3 папки mkdir  g_1 g_2 g_3

Зайти в любоую папку cd g_1/

Создать 5 файлов (3 txt, 2 json) touch one.txt twoo.txt three.txt for.json five.json

Создать 3 папки mkdir s_1 s_2 s_3

Вывести список содержимого папки  ls -la

Открыть любой txt файл vim one.txt

Написать туда что-нибудь, любой текст. нажать клавишу "i" ввести текст "Hello world"

сохранить и выйти. "esc" ввести ":wq"

Выйти из папки на уровень выше cd ..

переместить любые 2 файла, которые вы создали, в любую другую папку.
mv g_1/one.txt g_2/one.txt , mv g_1/twoo.txt g_2/twoo.txt

скопировать любые 2 файла, которые вы создали, в любую другую папку. cp g_2/twoo.txt g_3/twoo.txt ,cp g_2/twoo.txt g_3/twoo.txt 

Найти файл по имени find . -name one.txt

просмотреть содержимое в реальном времени (команда grep) изучите как она работает. tail -f one.txt

вывести несколько первых строк из текстового файла head -2 one.txt

вывести несколько последних строк из текстового файла tail -2 one.txt

просмотреть содержимое длинного файла (команда less) изучите как она работает. less name_file

вывести дату и время date +"%D %T"

Задание *

Отправить http запрос на сервер. http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000
curl 'http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000'

1_1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request

curl http://162.55.220.72:5005/terminal-hw-request

приходит ответ с другим заданием.

curl "http://162.55.220.72:5005/get_method?name=(Denis)&age=(29)"


Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
Создаём файл: touch script.sh

Вносим изменения: vim script.sh

нажать клавишу "i" ввести текст

#!/bin/sh
cd terminal_linux
mkdir ww_1 ww_11 ww_22
cd ww_1
touch rr_1.txt rr_11.txt rr_22.txt jj_1.json jj_11.json
mkdir  ff_1 ff_11 ff_22
ls -la
mv rr_22.txt rr_11.txt ff_11
Cохранить и выйти: "esc" ":wq"

Выполняем скрипт: sh script.sh .
