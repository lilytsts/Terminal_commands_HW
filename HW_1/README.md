# HW_1 Linux terminal (GitBash) commands

 *1. Посмотреть где я.* 

  
   + `pwd`
   
 *2. Создать папку.*

  
   + `mkdir dir`
 
 *3. Зайти в папку.*

  
   + `cd dir`
   
*4. Создать 3 папки.*


   + `mkdir dir{1..3}`
  
*5. Зайти в любую папку.*

  
   + `cd dir1`
  
 *6. Создать 5 файлов (3 txt, 2 json).*

  
   + `touch file1.txt file2.txt file3.txt file1.json file2.json`
  
 *7. Создать 3 папки.*

  
   + `mkdir diradd{1..3}`
  
 *8. Вывести список содержимого папки.*

  
   + `ls -la` (вывод всех данных, в т.ч. скрытых)

 *9. Открыть любой txt файл(для редактирования).*

  
   + `vim file1.txt`

 *10. Написать туда что-нибудь, любой текст.*

  
   + нажать `"i"` (режим редактирования)

   + `ввести текст`

   + нажать `"esc"`
  
 *11. Сохранить и выйти.*

  
   + `:wq`
  
 *12. Выйти из папки на уровень выше.*

  
   + `cd ..`(выйти на 1 уроверь выше)

   + `cd ../..` (выйти на 2 уровня выше)
  
 *13. Переместить любые 2 файла, которые вы создали, в любую другую папку.*

  
   + `mv diradd1/file1.txt diradd1/file2.txt diradd2 `
    
 *14. Скопировать любые 2 файла, которые вы создали, в любую другую папку.*

  
   + `cp diradd2/file1.txt diradd2/file2.txt diradd1`
  
 *15. Найти файл по имени.*

  
   + `find . -name "file3.txt"`
  
 *16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает.*

  
   + `tail -f file_1.txt`


 *17. Вывести несколько первых строк из текстового файла.*

  
   + `head -3 file1.txt`

 *18. Вывести несколько последних строк из текстового файла.*

  
   + `tail -3 file1.txt`
  
 *19. Просмотреть содержимое длинного файла (команда less) изучите как она работает.*

  
   + `less file1.txt`

   + нажать `"q"`

 *20. Вывести дату и время.*

  
   + `date`

*Задание **
*1. Отправить http запрос на сервер*
http://162.55.220.72:5005/terminal-hw-request

+ `curl  "http://162.55.220.72:5006/terminal-hw-request"`

+ `{
  "Intro": "Hello!! This is your the first response from server", 
  "Tasks": {
    "Task_1": "Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)", 
    "result": [
      "Your_String", 
      "Your_number"
    ]
  }
}`

+ `curl "http://162.55.220.72:5005/get_method?name=lily&age=33"`

+ `[
  "lily", 
  "33"
]`

*2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13*

*2.1 Создать файл с расширением myscript.sh*

+ `touch myscript.sh`

*2.2 Открыть его для редактирования*

+ `vim myscript.sh`

*2.3 Записать туда команды из пунктов 3, 4, 5, 6, 7, 8, 13*
+ `i`

+ `cd 1606`
+ `mkdir dirsh{1..3}`
+ `cd dirsh1`
+ `touch file1.txt file2.txt file3.txt file1.json file2.json`
+ `mkdir diradd{1..3}`
+ `ls -la`
+ `cd`
+ `mv diradd1/file1.txt diradd1/file2.txt diradd2`



*2.4 Сохранить файл и записать файл и выйти из vim*
+ `control + D`
+ `:wq`

  
*2.5 Запустить скрипт*
+ `sh myscript.sh`




