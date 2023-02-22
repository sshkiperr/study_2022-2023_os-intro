---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Markdown"
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

Создать отчет по лабораторной работе №2.

# Задание

Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.

# Теоретическое введение

Базовые сведения о Markdown
Чтобы создать заголовок, используйте знак ( # ), например:
1. # This is heading 1
2. ## This is heading 2
3. ### This is heading 3
4. #### This is heading 4
Чтобы задать для текста полужирное начертание, заключите его в двойные звездочки:
1 This text is >**bold**.
Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки:
1 This text is *italic*.
Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные
звездочки:
1 This is text is both >***bold and italic***.

Неупорядоченный (маркированный) список можно отформатировать с помощью звез-
дочек или тире:
1 - List item 1
2 - List item 2
3 - List item 3



# Выполнение лабораторной работы

Указываем название лабораторной работы и автора:

![Название работы и имя автора](ос31.png)

Пишем цель работы и задание (каждый заголовок обозначаем решеткой):

![Цель и задание работы](ос32.png)

Поэтапно описываем выполнение лабораторной работы, прикрепляя скриншоты с подписью: 

![Этапы выполнения лабораторной работы](ос33.png)

Отвечаем по пунктам на контрольные вопросы:

![Ответ на контрольные вопросы](ос34.png)

Пишем вывод, согласно цели работы:

![Цель работы](ос35.png)

# Выводы

Я приобрела навыки создания отчетов в формате Markdown.
