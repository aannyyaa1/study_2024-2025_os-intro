---
## Front matter
title: "Отчет по лабораторной работе №3"
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

Научиться оформлять отчеты с помощью легкословестного языка разметки Markdown.

# Задание

- Сделать отчет по предыдущей лабораторной работе в формате Markdown.
- В качестве отчета предоставить отчеты в 3 форматах: pdf, docx и md.

# Теоретическое введение

Markdown - облегченный язык разметки, созданный с целью обозначения форматирования в простом тексте,с максимальным сохранением его читаемости 
человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций.

# Выполнение лабораторной работы

Захожу в терминал, получаю роль супер-пользователя и открываю файл с отчетом через текстовый редактор nano (рис. [-@fig:001]).

![Открытие файла](image/1.png){#fig:001 width=70%}

Начинаю работу с файлом отчета (рис. [-@fig:002]).

![Редактирование файла](image/2.png){#fig:002 width=70%}

По завершению работы над файлом сохраняю изменения в нем и в терминале перехожу в каталог с лабораторными работами и отправляю все файлы на GitHub 
(рис. [-@fig:003]).

![Отправка файлов на GitHub](image/3.png){#fig:003 width=70%}

И наконец использую git push (рис. [-@fig:004]).

![Завершение отправки файлов](image/4.png){#fig:004 width=70%}

# Выводы

В ходе выполнения данной лабораторной работы я научилась оформлять отчеты с помощью легкословестного языка разметки Markdown.

# Список литературы

::: {#refs}
:::
