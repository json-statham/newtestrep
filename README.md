# newtestrep
Linux terminal (GitBash) commands
1) Посмотреть где я - ```pwd```
2) Создать папку - ```mkdir testf```
3) Зайти в папку - ```cd testf```
4) Создать 3 папки - ```mkdir testf1 testf2 testf3```
5) Зайти в любоую папку - ```cd testf1```
6) Создать 5 файлов (3 txt, 2 json) - ```touch one.txt two.txt three.txt one.json two.json```
7) Создать 3 папки - ```mkdir {newfold1, newfold2, newfold3}```
8) Вывести список содержимого папки - ```ls``` **(отображаются папки, которые были созданные выше и 5 файлов: 3txt и 2json)**
9) Открыть любой txt файл - ```vim one.txt```
10) написать туда что-нибудь, любой текст - **hello there guys**
11) сохранить и выйти. - ```Клавиша ESC > :wq```
12) Выйти из папки на уровень выше ```cd ..```
**Перемещаемся к нашим файлам cd testf1 > ls -la**
13) переместить любые 2 файла, которые вы создали, в любую другую папку - ```mv one.json two.json newfold1```
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. ```cp one.txt two.txt newfold2/```
15) Найти файл по имени ```find -name one.json```
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. ```- tail -f one.txt```
17) вывести несколько первых строк из текстового файла ```cat one.txt | head -n1 -n2```
18) вывести несколько последних строк из текстового файла ```cat one.txt | head -n3 | tail -n2```
19) просмотреть содержимое длинного файла (команда less) изучите как она работает. ```less one.txt```
20) вывести дату и время - ```date```

1) Отправить http запрос на сервер. - ```curl http://162.55.220.72:5005/terminal-hw-request```
```curl http://162.55.220.72:5005/get_method?name="Rakhim&age=25"```
2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

=====================
```sh 
#!/bin/bash
cd script
mkdir papka1 papka2 papka3
cd papka1
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir p1papka1 p2papka1 p3papka1
ls -la
mv file1.txt file2.txt ~/Desktop/testf/script/papka2
```
