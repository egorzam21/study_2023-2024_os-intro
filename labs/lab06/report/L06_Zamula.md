---
## Front matter
title: "Отчёт по лабораторной работе №6"
subtitle: "Дисциплина : операционная система"
author: "Замула Егор Сергеевич"

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


    - Изучить идеологию и применение средств контроля версий.
    - Освоить умения по работе с git.


# Задание


    - Создать базовую конфигурацию для работы с git.
    - Создать ключ SSH.
    - Создать ключ PGP.
    - Настроить подписи git.
    - Зарегистрироваться на Github.
    - Создать локальный каталог для выполнения заданий по предмету.


# Теоретическое введение

Системы контроля версий (Version Control System, VCS) применяются при работе нескольких человек над одним проектом. Обычно основное дерево проекта хранится в локальном или удалённом репозитории, к которому настроен доступ для участников проекта. При внесении изменений в содержание проекта система контроля версий позволяет их фиксировать, совмещать изменения, произведённые разными участниками проекта, производить откат к любой более ранней версии проекта, если это требуется.

В классических системах контроля версий используется централизованная модель, предполагающая наличие единого репозитория для хранения файлов. Выполнение большинства функций по управлению версиями осуществляется специальным сервером. Участник проекта (пользователь) перед началом работы посредством определённых команд получает нужную ему версию файлов. После внесения изменений, пользователь размещает новую версию в хранилище. При этом предыдущие версии не удаляются из центрального хранилища и к ним можно вернуться в любой момент. Сервер может сохранять не полную версию изменённых файлов, а производить так называемую дельта-компрессию — сохранять только изменения между последовательными версиями, что позволяет уменьшить объём хранимых данных.

Системы контроля версий поддерживают возможность отслеживания и разрешения конфликтов, которые могут возникнуть при работе нескольких человек над одним файлом. Можно объединить (слить) изменения, сделанные разными участниками (автоматически или вручную), вручную выбрать нужную версию, отменить изменения вовсе или заблокировать файлы для изменения. В зависимости от настроек блокировка не позволяет другим пользователям получить рабочую копию или препятствует изменению рабочей копии файла средствами файловой системы ОС, обеспечивая таким образом, привилегированный доступ только одному пользователю, работающему с файлом.

Системы контроля версий также могут обеспечивать дополнительные, более гибкие функциональные возможности. Например, они могут поддерживать работу с несколькими версиями одного файла, сохраняя общую историю изменений до точки ветвления версий и собственные истории изменений каждой ветви. Кроме того, обычно доступна информация о том, кто из участников, когда и какие изменения вносил. Обычно такого рода информация хранится в журнале изменений, доступ к которому можно ограничить.

В отличие от классических, в распределённых системах контроля версий центральный репозиторий не является обязательным.

Среди классических VCS наиболее известны CVS, Subversion, а среди распределённых — Git, Bazaar, Mercurial. Принципы их работы схожи, отличаются они в основном синтаксисом используемых в работе команд.

# Выполнение лабораторной работы

1. Установка системы git в нашу ОС 

![Установка git](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2011-46-51.png?raw=true){#fig:001 width=70%}

2. Проводим базоваю настройку git

![Настройка git](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2011-50-03.png?raw=true){#fig:002 width=70%}

3. Создаем SSH ключа по алгоритму rsa с ключём размером 4096 бит

![Создание ssh ключа](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2011-50-55.png?raw=true){#fig:003 width=70%}

4. Добавляем SSH ключ на гитхаб в разеделе settings 

![Добавление SSH ключа](image/placeimg_800_600_tech.jpg){#fig:004 width=70%}

5. Создание pgp ключа

![pgp ключ](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-02-29.png?raw=true){#fig:005 width=70%}

6. Добавляем ключ на гитхаб (точно так же как и SSH)

![Добавляем pgp ключ](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-06-37.png?raw=true){#fig:006 width=70%}

7. Получение sec параметра

![sec](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-06-47.png?raw=true){#fig:007 width=70%}

8. Настройка автоматических подписей коммитов git

![Подписи](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-09-53.png?raw=true){#fig:008 width=70%}

9. Клонируем репозиторий

![Клонируем](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-23-49.png?raw=true){#fig:009 width=70%}

10. Настройка каталога курса

![Настройка каталога](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-47-10.png?raw=true){#fig:010 width=70%}

11. Отправка на сервер нашего отредактированного репозитория
![Отпрарвка на сервер](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab02/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-24%2012-50-43.png?raw=true){#fig:011 width=70%}

# Контрольные вопросы

    Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются?
    Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия.
    Что представляют собой и чем отличаются централизованные и децентрализованные VCS? Приведите примеры VCS каждого вида.
    Опишите действия с VCS при единоличной работе с хранилищем.
    Опишите порядок работы с общим хранилищем VCS.
    Каковы основные задачи, решаемые инструментальным средством git?
    Назовите и дайте краткую характеристику командам git.
    Приведите примеры использования при работе с локальным и удалённым репозиториями.
    Что такое и зачем могут быть нужны ветви (branches)?
    Как и зачем можно игнорировать некоторые файлы при commit?

# Выводы

В ходе выполнения работы изучил git

# Список литературы{.unnumbered}

::: {#refs}
:::
