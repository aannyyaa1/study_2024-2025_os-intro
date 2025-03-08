---
## Front matter
title: "Лабораторная работа №4"
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

Получение навыков правильной работы с репозиторием git.

# Задание

- Выполнить работу для тестового репозитория
- Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits

# Теоретическое введение

- Gitflow Workflow опубликована и популяризована Винсентом Дриссеном.
- Gitflow Workflow предполагает выстраивание строгой модели ветвления с учётом выпуска проекта.
- Данная модель отлично подходит для организации рабочего процесса на основе релизов.
- Работа по модели Gitflow включает создание отдельной ветки для исправлений ошибок в рабочей среде.

# Выполнение лабораторной работы
## Установка git-flow

Установка из коллекции репозиториев Corp (рис. [-@fig:001]).

![Установка git-flow](image/1.png){#fig:001 width=70%}

## Установка Node.js

Устанавливаем Node.js, на котором базируется программное обеспечение для семантического 
весионирования и общепринятых коммитов (рис. [-@fig:002]).

![Установка Node.js](image/2.png){#fig:002 width=70%}

## Настройка Node.js

Для работы добавим каталог с имполняемыми файлами. Запускаю (рис. [-@fig:003]).

![Настройка Node.js](image/3.png){#fig:003 width=70%} 

## Общепринятые коммиты

Программа commitizen используется для помощи в форматировании коммитов (рис. [-@fig:004]).

![Настройка коммитов](image/4.png){#fig:004 width=70%}

Программа standart-changelog используется для помощи в создании логов (рис. [-@fig:005]).

![Настройка коммитов](image/5.png){#fig:005 width=70%}

## Создание репозитория git

Создаю репозиторий на гитхаб (рис. [-@fig:006]).

![Создание репозитория](image/6.png){#fig:006 width=70%}

Конфигурация общепринятых коммитов.(рис. [-@fig:007]).

![Конфигурация коммитов](image/7.png){#fig:007 width=70%}

Заполняю несколько параметров пакета (рис. [-@fig:008]).

![Конфигурация коммитов](image/8.png){#fig:008 width=70%}

Захожу в mc и редактирую файл (рис. [-@fig:009]).

![Открытие файла](image/9.png){#fig:009 width=70%}

Получившийся файл сохраняю и выхожу (рис. [-@fig:010]).

![Редактирование файла](image/10.png){#fig:010 width=70%}

Добавляю новые файлы, выполняю коммит (рис. [-@fig:011]).

![Добавление файлов](image/11.png){#fig:011 width=70%}

Отпраляю на гитхаб (рис. [-@fig:012]).

![Отправление файлов](image/12.png){#fig:012 width=70%}

Инициализирую git-flow (рис. [-@fig:013]).

![Инициализация git-flow](image/13.png){#fig:013 width=70%}

Проверяю, что я в ветке develop и загружаю весь репозиторий в хранилище (рис. [-@fig:014]).

![Загрузка репозитория](image/14.png){#fig:014 width=70%}

Устанавливаю внешнюю ветку как вышестоящую для ветки (рис. [-@fig:015]).

![Работа с ветками](image/15.png){#fig:015 width=70%}

Создаю релиз с версией 1.0.0 (рис. [-@fig:016]).

![Создание релиза](image/16.png){#fig:016 width=70%}

Создаю журнал изменений (рис. [-@fig:017]).

![СОздание журнала](image/17.png){#fig:017 width=70%}

Добавляю журнал изменений в индекс (рис. [-@fig:018]-[-@fig:019]).

![Добавление журнала](image/18.png){#fig:018 width=70%}

![Добавление журнала](image/19.png){#fig:019 width=70%}

Заливаю релизную ветку в основную ветку (рис. [-@fig:020]).

![Работа с ветками](image/20.png){#fig:020 width=70%}

Отправляю данные на гитхаб (рис. [-@fig:021]).

![Отправка данных](image/21.png){#fig:021 width=70%}

Создаю релиз на гитхаб (рис. [-@fig:022]).

![Создание релиза](image/22.png){#fig:022 width=70%}

## Работа с репозиторием git

Создаю ветку для новой функциональности (рис. [-@fig:023]).

![СОздание ветки](image/23.png){#fig:023 width=70%}

Объединяю ветку feature_branch с develop (рис. [-@fig:024]).

![Объединение веток](image/24.png){#fig:024 width=70%}

Создаю релиз с версией 1.2.3 (рис. [-@fig:025]).

![СОздание релиза](image/25.png){#fig:025 width=70%}

Создаю журнал изменений (рис. [-@fig:026]).

![СОздание журнала](image/26.png){#fig:026 width=70%}

Добавляю журнал изменений в индекс (рис. [-@fig:027]-[-@fig:028]).

![Добавление журнала в индекс](image/27.png){#fig:027 width=70%}

![Добавление журнала в индекс](image/28.png){#fig:028 width=70%}

Заливаю релизную ветку в основную ветку (рис. [-@fig:029]).

![Работа с ветками](image/29.png){#fig:029 width=70%}

Отправляю данные на гитхаб (рис. [-@fig:030]-[-@fig:031]).

![Отправка данных](image/30.png){#fig:030 width=70%}

![Отправка данных](image/31.png){#fig:031 width=70%}

Создаю релиз на гитхаб с комментарием из журнала изменений (рис. [-@fig:032]).

![Создание релиза](image/32.png){#fig:032 width=70%}

# Выводы

В ходе выполнения данной лабораторной работы я получила навыки праильной работы с 
репозиториями git. 

# Список литературы

::: {#refs}
:::










