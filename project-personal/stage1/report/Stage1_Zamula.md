---
## Front matter
title: "Отчёт по первому этапу индивидуального проекта"
subtitle: "дисциплина: Операционные системы"
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

Размещение на Github pages заготовки для персонального сайта.

# Задание

    - Установить необходимое программное обеспечение.
    - Скачать шаблон темы сайта.
    - Разместить его на хостинге git.
    - Установить параметр для URLs сайта.
    - Разместить заготовку сайта на Github pages.



# Выполнение лабораторной работы

1. Скачиваю исполняемый файл hugo с официаольного сайта (ссылка на сайт в туис.

![Скачиваю hugo](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-10-14.png?raw=true){#fig:001 width=70%}

2. Извлек содержимое архива в папку bin в домашней папке (заранее нужно создать)

![Распоковываю архив](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-12-08.png?raw=true){#fig:002 width=70%}

3. Создаю репозиторий на основе репозитория HugoBlox

![Создание рпеозитория](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-17-28.png?raw=true){#fig:003 width=70%}

4. Клонирую репозиторий в рабочую папку work

![Клонирую репозиторий](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-19-30.png?raw=true){#fig:004 width=70%}

5. В каталоге project устанавливаю "go"

![Устанавливаю "go"](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-20-32.png?raw=true){#fig:005 width=70%}

6. Выполняем комманду ~/bin/hugo для создания страницы сайта

![Создаем страницу](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-22-40.png?raw=true){#fig:006 width=70%}

7. Через команду mc удаляем папку public

![Удаляем папку public](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-32-05.png?raw=true){#fig:007 width=70%}

8. Получаем ссылку на наш локальный сайт

![Ссылка на локальный сайт](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-33-40.png?raw=true){#fig:008 width=70%}

9. Демонстрация демо-сайта

![Демо-сайт](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-34-51.png?raw=true){#fig:009 width=70%}

10. Создаём новый пустой репозиторий 
![Новый репозиторий](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-38-53.png?raw=true){#fig:010 width=70%}

11. Клонирпуем новый репозиторий в рабочее пространство

![Клонируем новый репозиторий](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-40-42.png?raw=true){#fig:011 width=70%}

12. Создаем пустой файл readme.md , чтобы активировать репозиторий

![Активация репозитория](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-43-15.png?raw=true){#fig:012 width=70%}

13. Комментируем строку паблик, чтобы копирование файлов происходило гладко

![Исправляем файл](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2009-50-13.png?raw=true){#fig:013 width=70%}

14. Копируем наш демой сайт из одного репозитория в другой и отпарвляем на сервер файлы

![Копируем репозитории](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2010-09-43.png?raw=true){#fig:014 width=70%}

15. Скопированные файлы в новый репозиторий для нашего сайта
![Проверка репозитория](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage1/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-26%2010-12-19.png?raw=true){#fig:015 width=70%}


# Выводы

Научились размещать на гитхаб заготовки для персонального сайта

# Список литературы{.unnumbered}

::: {#refs}
:::
