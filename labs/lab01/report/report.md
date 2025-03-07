---
## Front matter
title: "Отчет по лабораторной работе №1"
subtitle: "Операционные системы"
author: "Ермакова Анастасия Алексеевна"

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

# Цель работы

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых
для дальнейшей работы сервисов.

# Задание

1. Установка Linux на Virtualbox
2. Работа с операционной системой после установки
3. Настройка раскладки клавиатуры
3. Установка программного обеспечения для создания документации
4. Домашнее задание

# Выполнение лабораторной работы
## Установка Linux на Virtualbox

Устанавливаю Линукс на виртуальную машину (рис. [-@fig:001]).

![Установка виртуальной машины](image/4.png){#fig:001 width=70%}

У меня она имеет следующие характеристики (рис. [-@fig:002]).

![Характеристики виртуальной машины](image/5.png){#fig:002 width=70%}

## Работа с операционной системой после установки

Вхожу в ОС, нажимаю комбинацию Win+Enter для запуска терминала и переключаюсь на роль супер-пользователя (рис. [-@fig:003]).

![Переключение на роль супер-пользователя](image/6.png){#fig:003 width=70%}

Устанавливаю средства разработки (рис. [-@fig:004]).

![Установка средств разработки](image/7.png){#fig:004 width=70%}

Обновляю пакеты (рис. [-@fig:005]).

![Обновление пакетов](image/8.png){#fig:005 width=70%}

Устанавливаю программу для удобства работы в консоли (рис. [-@fig:006]).

![Установки программы для консоли](image/9.png){#fig:006 width=70%}

Устанавливаю программное обеспечение для автоматического обновления (рис. [-@fig:007]).

![Установка программы для авто обновления](image/10.png){#fig:007 width=70%}

Запускаю таймер (рис. [-@fig:008]).

![Запуск таймера](image/11.png){#fig:008 width=70%}

Для отключение SELinux необходимо использовать Midnight Commander, установлю его с помощью команды sudo dnf install mc (рис. [-@fig:009]).

![Установка mc](image/12.png){#fig:009 width=70%}

После установки перехожу в каталог selinux и захожу в mc (рис. [-@fig:010]).

![Перемещение по каталогам](image/13.png){#fig:010 width=70%}

Открываю файл и вношу в него изменения (рис. [-@fig:011]-[-@fig:012]).

![Перемещение по каталогам](image/14.png){#fig:011 width=70%}

![Название рисунка](image/15.png){#fig:012 width=70%}

Перезапускаю виртуальную машину (рис. [-@fig:013]).

![Название рисунка](image/19.png){#fig:013 width=70%}

## Настройка раскладки клавиатуры

Снова захожу в ОС, запускаю терминал и запускаю терминальный мультиплексор tmux (рис. [-@fig:014]).

![Название рисунка](image/2.png){#fig:014 width=70%}

Создаю конфигурационный файл и перехожу в mc для его дальнейшей редакции (рис. [-@fig:015]).

![Название рисунка](image/3.png){#fig:015 width=70%}

Вношу изменения в файл (рис. [-@fig:016]).

![Название рисунка](image/16.png){#fig:016 width=70%}

Переключаюсь на роль супер-пользователя и снова захожу в mc (рис. [-@fig:017]).

![Название рисунка](image/17.png){#fig:017 width=70%}

Редактирую другой конфигурационный файл (рис. [-@fig:018]).

![Название рисунка](image/18.png){#fig:018 width=70%}

Перезагружаю виртуальную машину (рис. [-@fig:019]).

![Название рисунка](image/1.png){#fig:019 width=70%}

## Установка программного обеспечения для создания документации

Запускаю терминальный мультиплексор, переключаюсь на роль супер-пользователя и устанавливаю pandoc (рис. [-@fig:020]).

![Название рисунка](image/20.png){#fig:020 width=70%}

Затем устанавливаю texlive (рис. [-@fig:021]).

![Название рисунка](image/21.png){#fig:021 width=70%}

Устанавливаю пакеты pandoc и pandoc-crossref с github (рис. [-@fig:022]).

![Название рисунка](image/22.png){#fig:022 width=70%}

Через mc копирую файлы в нужный каталог (рис. [-@fig:023]). Все готово.

![Название рисунка](image/23.png){#fig:023 width=70%}

## Домашнее задание 

Открываю терминал, выполняю команду dmesg | less (рис. [-@fig:024]).

![Название рисунка](image/24.png){#fig:024 width=70%}

Далее получаю с помощью этой информации необходимую информацию (рис. [-@fig:025]-[-@fig:026]).

![Название рисунка](image/25.png){#fig:025 width=70%}

![Название рисунка](image/26.png){#fig:026 width=70%}


# Выводы

В ходе выполнения данной лабораторной работы я преобрела практиические навыки установки
операционной системв на виртуальную машину, настройки минимально необходимых для 
дальнейшей работы серверов. 

# Список литературы

::: {#refs}
::: 

























