---
## Front matter
title: "Отчёта по лабораторной работе 7"
subtitle: "Операционные системы"
author: "Гомес Лопес Теофания"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

# Задание

1. Команды для работы с файлами и каталогами
2. Анализ файловой системы Linux.

# Выполнение лабораторной работы

## Команды для работы с файлами и каталогами

Создаю файл abc1 с помощью touch и копирую его с новыми именами april и may исползуя cp:

![Создание файлов abc1, april e may](image/1.png){#fig:001 width=70%}

Создаю каталог monthly и копирую april и may в нем исползуя cp. Проверяю с ls:

![Создание файлa monthly](image/2.png){#fig:002 width=70%}

В каталоге monthly копирую файл may с именем june исползуя cp:

![копирование файла may](image/3.png){#fig:003 width=70%}

Копирую каталог monthly в каталог monthly.00 с помощью опции cp -r:

![копирование каталога monthly](image/4.png){#fig:004 width=70%}

Копирую каталог monthly.00 в каталог /tmp:

![копирование каталога monthly.00](image/5.png){#fig:005 width=70%}

Изменяю название файла april на july в домашнем каталоге и перемещаю файл july в каталог monthly.00:

![перемещение файла july](image/6.png){#fig:006 width=70%}

Переименовываю каталог monthly.00 в monthly.01. Перемещаю каталог monthly.01 в каталог reports:

![перемещение и Переименование каталога monthly.00](image/7.png){#fig:007 width=70%}

Переименовываю каталог reports/monthly.01 в reports/monthly:

![переименование каталога reports/monthly.01](image/8.png){#fig:008 width=70%}

Копирую файл /usr/include/sys/io.h в домашний каталог и назову его equipment:

![Создание equipment](image/9.png){#fig:009 width=70%}

В домашнем каталоге создаю директорию ~/ski.plases с помощью mkdir:

![Проверка создания ski.plases](image/10.png){#fig:0010 width=70%}

 Перемещаю файл equipment в каталог ~/ski.plases:

![Перемещение файла equipment](image/11.png){#fig:0011 width=70%}

Переименую файл ~/ski.plases/equipment в ~/ski.plases/equiplist и копирую abc1 в каталог ~/ski.plases, назову его equiplist2:

![Переименование файла /equipment](image/12.png){#fig:0012 width=70%}

Создаю каталог с именем equipment в каталоге ~/ski.plases и перемещаю файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment:

![Создание каталога equipment, перемещение файлов ](image/13.png){#fig:0013 width=70%}

Создаю и перемещаю каталог ~/newdir в каталог ~/ski.plases и назову его plans:

![Создание и перемещение каталога newdir](image/14.png){#fig:0014 width=70%}

Создаю каталог australia. Удаляю права на исполнение для группы (g-x) и владелца(u-x):

![Создание australia](image/15.png){#fig:0015 width=70%}

![Удаление права](image/16.png){#fig:0016 width=70%}

Изменяю права доступа к каталогу play и проверяю:

![Измениеие прав](image/17.png){#fig:0017 width=70%}

![Проверка изменений](image/18.png){#fig:0018 width=70%}

Изменяю права доступа к файлу feathers и проверяю:

![Измениеие прав к файлу feathers](image/19.png){#fig:0019 width=70%}

 Смотрю содержимое файла /etc/passwd:

![команда cat](image/20.png){#fig:0020 width=70%}

Копирую файл ~/feathers в файл ~/file.old, перемещаю файл ~/file.old в каталог ~/play и копирую каталог ~/play в каталог ~/fun:

![Перемещение и копирование файлов и каталогов](image/21.png){#fig:0021 width=70%}

Перемещаю каталог ~/fun в каталог ~/play и назову его games

![Перемещение каталога fun](image/22.png){#fig:0022 width=70%}

Лишаю пользователя файла ~/feathers права на чтение:

![Лишение права на читение](image/23.png){#fig:0023 width=70%}

Когда я попытаюсь просмотреть файл ~/feathers командой cat, система запрешает мне:

![Посмотра файла feathers](image/24.png){#fig:0024 width=70%}

Лишаю владельца каталога ~/play права на выполнение. Когда я попробую перейти в этот же каталог, система запрешает мне:

![Лишение права на выполнение](image/25.png){#fig:0025 width=70%}

Даю владельцу каталога ~/play право на выполнение:

![Название рисунка](image/26.png){#fig:0026 width=70%}

С помощью man прочитаю по следующим командам:
mount — утилита командной строки в UNIX-подобных операционных системах. Применяется для монтирования файловых систем.

![mount](image/27.png){#fig:0027 width=70%}

fsck (проверка файловой системы) - это утилита командной строки, которая позволяет выполнять проверки согласованности и интерактивное исправление в одной или нескольких файловых системах Linux. Он использует программы, специфичные для типа файловой системы, которую он проверяет.

![fsck](image/28.png){#fig:0028 width=70%}

mkfs используется для создания файловой системы Linux на некотором устройстве, обычно в разделе жёсткого диска. В качестве аргумента filesys для файловой системы может выступать или название устройства

![mkfs](image/29.png){#fig:0029 width=70%}

Команда Kill посылает указанный сигнал указанному процессу. Если не указано ни одного сигнала, посылается сигнал SIGTERM. Сигнал SIGTERM завершает лишь те процессы, которые не обрабатывают его приход. Для других процессов может быть необходимым послать сигнал SIGKILL, поскольку этот сигнал перехватить невозможно.

![kill](image/30.png){#fig:0030 width=70%}

# Выводы

При выполнении данной лабораторной работы я ознакомилась с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобрела практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.
