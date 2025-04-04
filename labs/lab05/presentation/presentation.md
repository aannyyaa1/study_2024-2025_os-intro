---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Операционные системы
author:
  - Ермакова А. А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 15 марта 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Ермакова Анастасия Алексеевна, НКАбд-02-24
  * студентка факультета физико-математических и естественных наук
  * Российский университет дружбы народов
  * [1132246718@rudn.ru](mailto:1132246718@rudn.ru)
  * <https://aannyyaa1.github.io/ru/>

:::
::: {.column width="30%"}

:::
::::::::::::::

## Цель работы

Познакомиться с pass, gopass, native messaging, chezmoi. Научиться пользоваться этими утилитами, синхронизировать их с гит.

## Задание

1. Установить и настроить pass
2. Настроить интерфейс с браузером
3. Сохранить пароль
4. Установить и настроить chezmoi
5. Настроить chezmoi на новой машине
6. Выполнить ежедневные операции с chezmoi

## Теоретическое введение

Менеджер паролей pass — программа, сделанная в рамках идеологии Unix.
Также носит название стандартного менеджера паролей для Unix (The standard Unix password manager).

Основные свойства:
Данные хранятся в файловой системе в виде каталогов и файлов.
Файлы шифруются с помощью GPG-ключа.

Структура базы паролей:
Структура базы может быть произвольной, если Вы собираетесь использовать её напрямую, без промежуточного программного обеспечения. Тогда семантику структуры базы данных Вы держите в своей голове.
Если же необходимо использовать дополнительное программное обеспечение, необходимо семантику заложить в структуру базы паролей.

# Выполнение лабораторной работы
## Установка и настройка pass

Устанавливаю  pass.

![](image/1.png)

## Установка и настройка pass

Устанавливаю gopass.

![](image/2.png)

## Установка и настройка pass

Переходим к настройкам. Просматриваю список ключей.

![](image/3.png)

Инициализирую хранилище.

![](image/4.png)

## Установка и настройка pass

Теперь синхронизирую с git. Создам структуру git.

![](image/5.png)

## Установка и настройка pass

Задаю адрес репозитория на хостинге, предварительно создав приватный репозиторий pass на GitHub.

![](image/6.png)

## Установка и настройка pass

Для синхронизации выполняю следующие команды: pass git pull...

![](image/7.png)

А так же pass git push.

## Установка и настройка pass

![](image/8.png)

## Установка и настройка pass

Проверяю статус синхронизации следующей командой.

![](image/9.png)

## Настройка интерфейса с браузером

Для начала устанавливаю плагин с браузером (фаерфокс).

![](image/10.png)

## Настройка интерфейса с браузером

Интерфейс для взаимодействия с браузером (native messaging).

![](image/11.png)

## Настройка интерфейса с браузером

![](image/12.png)

## Сохранение пароля

Добавляю новый пароль.

![](image/13.png)

## Сохранение пароля

Отображаю пароль для указанного файла, предварительно перехожу в нужный каталог.

![](image/14.png)

## Сохранение пароля

Заменяю существующий пароль.

![](image/15.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Устанавливаю дополнительное программное обеспечение.

![](image/16.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Устанавливаю шрифты.

![](image/17.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

![](image/18.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

![](image/19.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Устанавливаю бинарный файл. Скрипт определяет архитектуру процессора и операционную систему и скачивает необходимый файл:

![](image/20.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Буду использовать утилиты командной строки для работы с github. Для начала залогинюсь на гитхаб.

![](image/21.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Создам свой репозиторий для конфигурационных файлов на основе шаблона.

![](image/22.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Инициализирую chezmoi с моим репозиторием dotfiles.

![](image/23.png)

## Установка и настройка chezmoi. Управление файлами конфигурации

Проверяю, какие изменения внесёт chezmoi в домашний каталог, запускаю.

![](image/24.png)

Меня устраивают изменения, поэтому запускаю следующую команду.

![](image/25.png)

## Настройка chezmoi на новой машине

Перехожу на другую виртуальную машиу, открываю терминал, устанавливаю бинарный файл и инициализирую chezmoi с моим репозиторием dotfiles.

![](image/26.png)

## Настройка chezmoi на новой машине

Проверяю, какие изменения внесёт chezmoi в домашний каталог, запускаю chezmoi diff, и принимаю изменения.

![](image/27.png)

## Настройка chezmoi на новой машине

При существующем каталоге chezmoi можно получить и применить последние изменения из моего репозитория.

![](image/28.png)

## Настройка chezmoi на новой машине

Устанавливаю мои dotfiles на новый компьютер с помощью одной команды.

![](image/29.png)

## Ежедневные операции с chezmoi

Извлекаю последние изменения из репозитория и применяю их с помощью одной команды.

![](image/30.png)

# Выводы

В ходе выполнения данной лабораторной работы я научилась устанавливать, настраивать и пользоваться основными возможностями менеджера паролей.






































