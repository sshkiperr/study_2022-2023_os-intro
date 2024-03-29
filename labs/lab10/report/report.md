---
## Front matter
title: "Отчёт по лабораторной работе №10"
subtitle: "Программирование в командной процессоре ОС UNIX. Командные файлы"
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

## Цель работы

Цель работы — изучить основы программирования в командной оболочке OS Unix. 

# Выполнение лабораторной работы

1. Написать скрипт, который при запуске будет делать резервную копию самого себя (то есть файла, в котором содержится его исходный код) в другую директорию backup в вашем домашнем каталоге. При этом файл должен архивироваться одним из архиваторов на выбор zip, bzip2 или tar. Способ использования команд архивации необходимо узнать, изучив справку.

![Программа №1](image/1.png){#fig:001 width=70%}


2. Написать пример командного файла, обрабатывающего любое произвольное число аргументов командной строки, в том числе превышающее десять. Например, скрипт может последовательно распечатывать значения всех переданных аргументов.

![Программа №2](image/2.png){#fig:001 width=70%}

3. Написать командный файл — аналог команды ls (без использования самой этой команды и команды dir). Требуется, чтобы он выдавал информацию о нужном каталоге и выводил информацию о возможностях доступа к файлам этого каталога.

![Программа №3](image/3.png){#fig:001 width=70%}

4. Написать командный файл, который получает в качестве аргумента командной строки формат файла (.txt, .doc, .jpg, .pdf и т.д.) и вычисляет количество таких файлов в указанной директории. Путь к директории также передаётся в виде аргумента командной строки.

![Программа №4](image/4.png){#fig:001 width=70%}


## Ответы на контрольные вопросы

1. Объясните понятие командной оболочки. Приведите примеры командных оболочек. Чем они отличаются?

_Ответ_: командная оболочка позволяет исполнять команды.

2. Что такое POSIX?

_Ответ_: POSIX — набор стандартов описания интерфейсов взаимодействия операционной системы и прикладных программ.

3. Как определяются переменные и массивы в языке программирования bash?

_Ответ_: через равно.

4. Каково назначение операторов let и read?

_Ответ_: let позволяет выполнять арифметические операции при задании переменных, read считывает стандартный поток вывода.

5. Какие арифметические операции можно применять в языке программирования bash?

_Ответ_: стандартные.

6. Что означает операция (( ))?

_Ответ_: (( )) вычисляют логические условные выражения.

7. Какие стандартные имена переменных Вам известны?

_Ответ_: PATH, ENV, TERM.

8. Что такое метасимволы?

_Ответ_: специальные символы.

9. Как экранировать метасимволы?

_Ответ_: как угодно, но можно через \.

10. Как создавать и запускать командные файлы?

_Ответ_: для создания файла применить команду `touch <file> && chmod +x <file>`. Для запуска ввести `./<file>`

11. Как определяются функции в языке программирования bash?

_Ответ_: при помощи ключевого слова `function`.

12. Каким образом можно выяснить, является файл каталогом или обычным файлом?

_Ответ_: ls -l <file> выведет дополнительную информацию.

13. Каково назначение команд set, typeset и unset?

_Ответ_: таково: изменение значения внутренних переменных сценария, наложение ограничений на переменные, удаление переменной.

14. Как передаются параметры в командные файлы?

_Ответ_: через пробел при запуске программы.

15. Назовите специальные переменные языка bash и их назначение.

_Ответ_: см. вопрос 7.

## Выводы

В ходе выполнения лабораторной работы были изучены основы программирования в командной оболочке OS Unix. Цель работы была достигнута.


