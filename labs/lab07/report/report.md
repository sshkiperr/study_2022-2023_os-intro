---
## Front matter
title: "Лабораторная работа №7."
subtitle: "Командная оболочка Midnight Commander."
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

Освоить основные возможности командной оболочки Midnight Commander. Приобрести навыки практической работы по просмотру каталогов и файлов, а также манипуляций с ними.

# Задание

Выполнить задания по mc

Создать отчет и презентацию в md

Загрузить скринкасты

# Теоретическое введение

Функционоальные клавиши mc:

F1 Вызов контекстно-зависимой подсказки
F2 Вызов пользовательского меню с возможностью создания и/или допол-
нения дополнительных функций
F3 Просмотр содержимого файла, на который указывает подсветка в ак-
тивной панели (без возможности редактирования)
F4 Вызов встроенного в mc редактора для изменения содержания файла,
на который указывает подсветка в активной панели
F5 Копирование одного или нескольких файлов, отмеченных в первой
(активной) панели, в каталог, отображаемый на второй панели
F6 Перенос одного или нескольких файлов, отмеченных в первой (актив-
ной) панели, в каталог, отображаемый на второй панели
F7 Создание подкаталога в каталоге, отображаемом в активной панели
F8 Удаление одного или нескольких файлов (каталогов), отмеченных в пер-
вой (активной) панели файлов
F9 Вызов меню mc
F10 Выход из mc

# Выполнение лабораторной работы

![Изучим информацию о mc, вызвав в командной строке man mc](image/1.png)

![Запустим из командной строки mc, изучим его структуру и меню](image/2.png)

Выполним несколько операций в mc, используя управляющие клавиши:

![В разделе меню "Левая панель" выбрали режим Дерево](image/4.png)

![Посмотрели информацию о каталоге выбрав режим Информация](image/5.png)

![Выбрали формат списка укроченный](image/6.png)

![В результате имена файлов помещаются в две колонки](image/7.png)

![Выбрали порядок сортировки по Размеру](image/8.png)

![Выбрали фильрт, показывающий файлы только с расширением *.pub и каталоги, в которых они находятся](image/10.png)

![В результате большинство скрытых файлов и все текстовые файлы в поле видения исчезли](image/11.png)

![Возможности подменю файл](image/13.png)

![Копирование файла в каталог](image/14.png)

![Поиск с заданными условиями](image/15.png)

![Выбор и повторение одной из предыдущих команд](image/16.png)

![Анализ файла расширений](image/17.png)

![Анализ файла меню](image/18.png)

![Вызвали подменю Настройки](image/19.png)

![Создали файл text.txt, откроем его F4](image/20.png)

![Вставим небольшой фрагмент текста](image/21.png)

![Удалим строку текста](image/22.png)

![Перенесем текст на новую строку F3, F5](image/23.png)

![Копируем текст на новую строку F3, F5](image/24.png)

![Сохраним изменения клавишей F2](image/25.png)

![Отменим последнее действие CTRL+U](image/26.png)

![Перейдем в начало файла и вконец файла, добавим еще текст](image/27.png)

![Откроем файл на некотором языке программирования](image/29.png)

![Используя меню редактора, включим подсветку синтаксиса](image/28.png)


# Выводы

Я освоила основные возможности командной оболочки Midnight Commander и приобрела навыки практической работы по просмотру каталогов и файлов, а также манипуляций с ними.


