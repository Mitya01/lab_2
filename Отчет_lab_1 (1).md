## Лабораторная работа №1

Сначала я скачал дистрибутив Linux Ubuntu, а затем открыл его в виртуальной машине Virtual Box.

Далее я запустил Терминал и начал выполнять лабораторную работу:

1. Создал новый файл с именем `script.bash`

```bash
touch script.bash
```

2. Открыл созданный файл `script.bash` для редактирования, выполнил:

```bash
gedit script.bash
```

3. Вписал в файл следующий скрипт

```bash
#!/bin/bash

echo "Welcome to ITMO University"
```

![image](https://github.com/user-attachments/assets/43d6ebe6-3ecf-445d-8717-0d0dddce8371)

4. Сохранил файл. Закрыл текстовый редактор `gedit`. Запустил bash-скрипт, выполнив в терминале

```bash
bash script.bash
```

5. В терминале отобразилась строка `Welcome to ITMO University`.

![image](https://github.com/user-attachments/assets/269b6b89-4586-4157-84a3-2b0ee758ad61)

## Задача

Затем я приступил к задаче модифицирования файла `script.bash` так, чтобы при его запуске в терминале в виде

```bash
bash script.bash Vasya Pupkin
```

Вывод был

`Welcome, Vasya Pupkin`

Для выполнения задачи я обратился к Интернету, изучил, как работать с параметрами в командной строке, и нашел подходящий метод:

* Переменная `$*` содержит все параметры, введённые в командной строке, в виде единого «слова».

Тогда в файл я вписал следующий скрипт:

```bash
#!/bin/bash

echo "Welcome, $*"
```

И вывелось то, что и требовалось:

![image](https://github.com/user-attachments/assets/452c4d54-4173-4202-a38e-50db7738a7a4)

Скрипт работал для других имен тоже:

![image](https://github.com/user-attachments/assets/91b12a67-0224-492f-9b90-fda91644fbcf)

## Вывод

Я получил базовые знания о том, как работать в Linux Ubuntu, в особенности в его Терминале и текстовом редакторе.  
