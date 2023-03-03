---
## Front matter
title: "Лаборная работа №4"
subtitle: "Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки"
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
biblatex: false
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

Приобрести практические навыки взаимодействия с системой посредством командной строки.


# Выполнение лабораторной работы

1. Определим полное имя домашнего каталога.

![Имя домашнего каталога](ос41.png){ #fig:001 width=70% }

2. Перейдите в каталог /tmp и выведем на экран содержимое каталога с помощью команды ls.

![Переход в каталог и его содержимое](ос42.png){ #fig:001 width=70% }

Применим команду ls с опцией -a, с ее помощью выведем скрытые каталоги.

![Скрытые каталоги](ос43.png){ #fig:001 width=70% }

Применим команду ls с опцией -l, с ее помощью вывели подробную информацию о файлах и каталогах.

![Информация о файлах и каталогах](ос44.png){ #fig:001 width=70% }

3. Определим, есть ли в каталоге /var/spool подкаталог с именем cron? Он там есть

![Файлы каталога в тч cron](ос45.png){ #fig:001 width=70% }

4. Перейдем в Ваш домашний каталог и выведем на экран его содержимое. Определим, кто является владельцем файлов и подкаталогов?

![Содержимое каталога и имя владельца](ос46.png){ #fig:001 width=70% }

5. В домашнем каталоге создадим новый каталог с именем newdir.

![Создание каталога newdir](ос47.png){ #fig:001 width=70% }

6. В каталоге ~/newdir создадим новый каталог с именем morefun.

![Содание каталога morefun](ос48.png){ #fig:001 width=70% }

7. В домашнем каталоге создадим одной командой три новых каталога с именами letters, memos, misk. Затем удалим эти каталоги одной командой.

![Создание каталогов и их удаление](ос49.png){ #fig:001 width=70% }

8. Попробуем удалить ранее созданный каталог ~/newdir командой rm. Проверим, был ли каталог удалён.
Без -r мы бы не смогли удалить не пустые каталоги.

![Попытка удаления каталога](ос410.png){ #fig:001 width=70% }

10. С помощью команды man определим, какую опцию команды ls нужно использовать для просмотра содержимого не только указанного каталога, но и подкаталогов, входящих в него.

![Команда ls -R](manlsr.png){ #fig:001 width=70% }

11. С помощью команды man определим набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов.

![Команда ls -c](manlsc.png){ #fig:001 width=70% }

12. Далее c помощью команды man выведем несколько команд.
cd-отвечает за переходы между каталогами
pwd-вывод нахождения на данный момент
mkdir-создание каталогов
rmdir-удаление пустых каталогов
rm-удаление файлов и директорий

![mancd](mancd.png){ #fig:001 width=70% }
![manpwd](manpwd.png){ #fig:001 width=70% }
![manmkdir](manmkdir.png){ #fig:001 width=70% }
![manrmdir](manrmdir.png){ #fig:001 width=70% }
![manrm](manrm.png){ #fig:001 width=70% }

13. Используя информацию, полученную при помощи команды history, выполним модификацию и исполнение нескольких команд из буфера команд.

![Модификация команд](ос411.png){ #fig:001 width=70% }

# Контрольные вопросы

1. Что такое командная строка? Термина для работы с файлами, каталогами.
2. При помощи какой команды можно определить абсолютный путь текущего каталога?  pwd
3. При помощи какой команды и каких опций можно определить только тип файлов и их имена в текущем каталоге? Приведите примеры. ls -l
4. Каким образом отобразить информацию о скрытых файлах? Приведите примеры. ls -a
5. При помощи каких команд можно удалить файл и каталог? Можно ли это сделать одной и той же командой? Приведите примеры. rm/rmdir рм не удалит не пустой каталог.
6. Каким образом можно вывести информацию о последних выполненных пользователем командах? работы? history
7. Как воспользоваться историей команд для их модифицированного выполнения? Приведите примеры. !<номер команды>:s/чтоменяем/начтоменяем
8. Приведите примеры запуска нескольких команд в одной строке.
9. Дайте определение и приведите примера символов экранирования. символы замены стандартных слов ~=home
10. Охарактеризуйте вывод информации на экран после выполнения команды ls с опцией
l. Вывод расширенной информации о файле-вес, название, защита.
11. Что такое относительный путь к файлу? Приведите примеры использования относительного и абсолютного пути при выполнении какой-либо команды.
12. Как получить информацию об интересующей вас команде? man
13. Какая клавиша или комбинация клавиш служит для автоматического дополнения вводимых команд? Ctrl+R
# Выводы

В данной лабораторной работе мы познакомились с командной строкой, научились простейшим командам.

:::