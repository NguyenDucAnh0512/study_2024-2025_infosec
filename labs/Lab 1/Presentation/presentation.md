---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе №1
subtitle: Установка и конфигурация операционной системы на виртуальную машину
author:
  - Нгуен Дык Ань
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 6 сентября 2024

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 43
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Нгуен Дык Ань
  * Студенческий билет: 1032215251
  * Группа: НКНбд-01-21
  * Российский университет дружбы народов
  * <https://github.com/NguyenDucAnh0512>

:::
::: {.column width="30%"}

![](https://drive.google.com/uc?id=11Y4Td4A-5Y6xtoE88lvJLn0uziw5GhbB)

:::
::::::::::::::

# Цель работы

Получить навыки установок операционной системы на виртуальную машину и настроить минимально необходимых для дальнейшей работы сервисов.

# Установить операционную систему Linux на VirtualBox

- Создать новую виртуальную машину, укажать называние и тип операционной системы — Linux, RedHat.

- Укажать размер основной памяти виртуальной машины - 4096 МБ, и количество процессора - 2.

- Задавать размер диска — 60 ГБ.

- Добавить новый привод оптических дисков.

# Установить операционную систему Linux на VirtualBox

![](https://drive.google.com/uc?id=1h1jlRdL19VZGcLUiDxCezIA1KuDIzQRI)

![](https://drive.google.com/uc?id=1US4h11eIQ3cxZeUd38BLAf_jK1bdYCPL)

![](https://drive.google.com/uc?id=1vee94XxeN5NHtXf_dueZddLxM8hYhI_j)

![](https://drive.google.com/uc?id=1mwu0-HvMZo3HXp-WFkhDxqlo12KQLpKB)

# Настроить систему для работы сервисов

- Выбрать "Server with GUI" и "Development tool"

- Отключить KDUMP

- Включить сетевое соединение и в качестве имени узла укажать danguen.localdomain

- Установить пароль для root и пользователя с правами администратора

- Ререзапустить подключить образ диска дополнений гостевой ОС

# Настроить систему для работы сервисов

![](https://drive.google.com/uc?id=19koVVDR9E6kAwAmgo5lx2xoM3wpU4EFo)

![](https://drive.google.com/uc?id=14PEqZRdfZTLxCD7_l8-n9ePIhKePv5re)

![](https://drive.google.com/uc?id=1JMw1-mtim3WrwerHyGZaK9qCtoPxrcV6)

![](https://drive.google.com/uc?id=1WQOZIDbF3J0gEKvuOLjPTePj0QYn6apf)

![](https://drive.google.com/uc?id=164ui4Rh7OfjA4VKZW61FTLpz0zIFX8Gj)

# Познакомиться с операционной системой командой "dmesg"

- **dmesg** - команда, используемая в UNIX‐подобных операционных системах для вывода буфера сообщений ядра в стандартный поток вывода (по умолчанию на экран).

- Можно использовать поиск с помощью **grep** для получения следующей информаций:

# Познакомиться с операционной системой командой "dmesg"

![](https://drive.google.com/uc?id=1Op1gXBk8dXv09aYEJbJt2jyWRFYQ4we3)

![](https://drive.google.com/uc?id=12i3X0tDlIvkmUATB-OzulGxbBpnDXv2z)

![](https://drive.google.com/uc?id=1rnZgldQajcS-HBMviKT4nUYJNH-haxK5)

![](https://drive.google.com/uc?id=1b9xpWNR1luYNJRSPDPYb-EHv5WNIZvGT)

![](https://drive.google.com/uc?id=1UblkoNTL40cwQ7wDmhxqagD_b0Qdhzdm)

![](https://drive.google.com/uc?id=16X29qW9bAuDKizNXAzefepbSwJjtXxir)

![](https://drive.google.com/uc?id=1KyrQE5dxWP4vMjfu3N-vaAy7FwaJd39F)

# Вывод

После лаборатоной работы я получил навыки установок и настройки операционной системы на виртуальную машину для дальнейшей работы сервисов.
