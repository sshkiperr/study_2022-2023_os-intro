---
## Front matter
title: "Отчёт по первому этапу индивидуального проекта."
subtitle: "Размещение на Github pages заготовки для персонального сайта."
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

Целью данной работы является размещение на Github pages заготовки для персонального сайта.

# Задачи

1. Установить необходимое программное обеспечение.
2. Скачать шаблон темы сайта.
3. Разместить его на хостинге git.
4. Установить параметр для URLs сайта.
5. Разместить заготовку сайта на Github pages.

# Выполнение работы

1. Скачаем исполняемый файл hugo (hugo_extended_0.110.0_Linux-64bit.tar.gz) для генерации страниц сайта. 

![Скачивание исполняемого файла hugo](ip1.png){ #fig:001 width=70% }

2. Перейдём в "Загрузки", разархивируем файл и создадим папку "bin" с файлом hugo. 

![Создание папки bin с файлом hugo](ip2.png){ #fig:003 width=70% }

4. Создадим репозиторий blog на основе шаблона. 

![Создание репозитория](ip3.png){ #fig:004 width=70% }

5. Клонируем созданный репозиторий. 

![Клонирование репозитория](ip4.png){ #fig:005 width=70% }

6. Переходим в каталог "blog" и вводим в терминале ~/bin/hugo 

![~/bin/hugo server](ip5.png){ #fig:006 width=70% }

7. Скопируем ссылку из предыдущего пункта и вставим её в браузер. 

![Переход на сайт](ip6.png){ #fig:007 width=70% }

8. Создадим репозиторий sshkiperr.github.io. 

![Создание репозитория](ip7.png){ #fig:008 width=70% }

9. Перейдем в терминал и клонируем созданный репозиторий. 

![Клонирование репозитория](ip8.png){ #fig:009 width=70% }

10. Перейдем в созданный каталог и введем в терминале команду git checkout -b main, чтобы создать ветку. 

![Создание ветки](ip9.png){ #fig:010 width=70% }

11. Создадим файл, чтобы активировать созданный репозиторий. 

![Активация репозитория](ip10.png){ #fig:011 width=70% }

12. Убедимся в том, что файл был создан. 

![Созданный файл](ip11.png){ #fig:012 width=70% }

13. Перейдем в каталог "blog" и введем в терминале команду git submodule add -b main git@github.com:godbyy/sshkiperr.github.io.git public, чтобы созданный репозиторий подключить к папке "public" внутри каталога "blog". 

![Подключение созданного репозитория к папке public](ip12.png){ #fig:013 width=70% }

14. Откроем в mc файл .gitignore и закомментирум public, сохраним изменения. 

![Комментирование public](ip13.png){ #fig:014 width=70% }

15. Проверим изменение из предыдущего пункта.

![Проверка изменения](ip14.png){ #fig:015 width=70% }

16. Убедимся в том, что появилась папка "public".

![Папка "public"](ip15.png){ #fig:016 width=70% }

17. Введем нужную команду, находясь в каталоге "blog", чтобы появились нужные файлы в папке "public".

![Команда ~/bin/hugo](ip16.png){ #fig:017 width=70% }

18. Синхронизируем появившиеся файлы с репозиторием, перейдя в папку "public". 

![Синхронизация файлов с репозиторием](ip17.png){ #fig:018 width=70% }

19. Обновим репозиторий и проверим, что все файлы появились. 

![Появившиеся файлы](ip18.png){ #fig:019 width=70% }

# Выводы

В ходе выполнения данной работы я разместила на Github pages заготовки для персонального сайта. Первый этап индивидуального проекта завершён. 

