---
## Front matter
title: "Лабораторная работа №6"
subtitle: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
author: "Кучеренко София"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Ознакомиться с инструментами поиска файлов и фильтрации текстовых данных. Приобрести практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Выполнение лабораторной работы

![Запишем в файл file.txt названия файлов, содержащихся в каталоге /etc](image/1.png){#fig:001 width=70%}

![Вывод файлов №1](image/1_1.png){#fig:001 width=70%}

![Допишем в этот же файл названия файлов, содержащихся в домашнем каталоге](image/2.png){#fig:001 width=70%}

![Вывод файлов №2](image/2_1.png){#fig:001 width=70%}

![С помощью команды cat проверим, что в файле содержатся названия файлов как каталога /etc, так и домашнего каталога](image/3.png){#fig:001 width=70%}

![Выведем имена всех файлов из file.txt, имеющих расширение .conf](image/4.png){#fig:001 width=70%}

![Запишем их в новый текстовой файл conf.txt](image/5.png){#fig:001 width=70%}

![Определим, какие файлы в домашнем каталоге имеют имена, начинающиеся с символа h](image/6.png){#fig:001 width=70%}

![Запустим в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log](image/8.png){#fig:001 width=70%}

![С помощью команды jobs проверим, что процесс работает в фоновом режиме](image/9.png){#fig:001 width=70%}

![С помощью команды cat проверим, что в файле содержатся названия файлов, начинающихся на log](image/610.png){#fig:001 width=70%}

![Проверим, что созданный файл logfile находится в домашнем каталоге](image/611.png){#fig:001 width=70%}

![После удаления файла ~/logfile с помощью команды jobs увидим, что процесс всё ещё запущен](image/612.png){#fig:001 width=70%}

![Запустим из консоли в фоновом режиме редактор gedit](image/614.png){#fig:001 width=70%}
![С помощью команды jobs проверим, что процесс работает в фоновом режиме](image/615.png){#fig:001 width=70%}

![Определим идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep](image/616.png){#fig:001 width=70%}

![Прочтем справку (man) команд df](image/mandf.png){#fig:001 width=70%}

![Прочтем справку (man) команд du](image/mandu.png){#fig:001 width=70%}

![Завершим процесс с помощью команды kill, посылая сигнал SIGKILL, имеющий номер 9, процессу 3439](image/618.png){#fig:001 width=70%}

![Выполним команду df](image/619.png){#fig:001 width=70%}

![Выполним команду du](image/620.png){#fig:001 width=70%}

![Воспользовавшись справкой команды find, выведем имена всех директорий, имеющихся в домашнем каталоге](image/621.png){#fig:001 width=70%}

С помощью type d мы попросили команду find искать только каталоги. С помощью maxdepth 1 мы попросили команду find сохранить поиск только на текущем уровне (и не заходить в подкаталоги). Введёная команда также показывает скрытые каталоги.

# Контрольные вопросы
    1. В системе по умолчанию открыто три специальных потока: – stdin — стандартный поток ввода (по умолчанию: клавиатура), файловый дескриптор 0 – stdout — стандартный поток вывода (по умолчанию: консоль), файловый дескриптор 1 – stderr — стандартный поток вывод сообщений об ошибках (по умолчанию: консоль), файловый дескриптор 2
    2. Операция > создаёт операция >> дополняет
    3. Конвейер (pipe) служит для объединения простых команд или утилит в цепочки, в которых результат работы предыдущей команды передаётся последующей.
    4. Компьютерная программа сама по себе — лишь пассивная последовательность инструкций. В то время как процесс — непосредственное выполнение этих инструкций
    5. PID - идентификатор процесса, уникальный номер процесса в многозадачной операционной системе. GID - идентификатор группы
    6. Запущенные фоном программы называются задачами (jobs). Ими можно управлять с помощью команды jobs, которая выводит список запущенных в данный момент задач
    7. Top (table of processes) — консольная команда, которая выводит список работающих в системе процессов и информацию о них. Htop – хорошо известная утилита для мониторинга, аналог top
    8. Команда find используется для поиска и отображения на экран имён файлов, соответствующих заданной строке символов. Формат команды: find (путь) (опции) Пример: Вывести на экран имена файлов из вашего домашнего каталога и его подкаталогов, начинающихся на f: find ~ -name “f*” -print
    9. Файл можно найти по контексту. Показать строки во всех файлах, в которых есть слово begin: grep begin
    10. Определить объем свободной памяти на жёстком диске можно с помощью команды df
    11. Команда du показывает число килобайт, используемое каждым файлом или каталогом. Чтобы найти объём домашнего каталога надо ввести команду du ~ в терминал
    12. Зависший процесс можно завершить с помощью команды kill, указав опцию -9 и номер процесса
    
# Выводы

Я ознакомилась с инструментами поиска файлов и фильтрации текстовых данных. Приобрести практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.
