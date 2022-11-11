---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Архитектура компьютеров"
author: "Кирилюк Светлана Алексеевна"

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

Освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Выполнение лабораторной работы

Сначала я создала каталог для работы с программами на языке ассемблера NASM (рис. [-@fig:fig1]) и перешла в него (рис. [@fig:fig2]).

![Создание каталога](fig1.jpg){ #fig:fig1 width=90% }

![Переход в каталог](fig2.jpg){ #fig:fig2 width=90% }

Затем создала текстовый файл с именем hello.asm (рис. [-@fig:fig3]), открыла его с помощью текстового редактора (рис. [-@fig:fig4]) и ввела следующий текст (рис. [-@fig:fig5]).

![Создание текстового файла](fig3.jpg){ #fig:fig3 width=90% }

![Открытие файла](fig4.jpg){ #fig:fig4 width=90% }

![Ввод текста](fig5.jpg){ #fig:fig5 width=90% }

Для компиляции приведённого выше текста программы «Hello World» я ввела команду (рис. [-@fig:fig6]) и проверила, что обратный файл был создан при помощи ls.

![Компиляция текста](fig6.jpg){ #fig:fig6 width=90% }

Затем я скомпилирова исходный файл hello.asm в obj.o и проверила, что все файлы были созданы (рис. [-@fig:fig7]).

![Компиляция файла](fig7.jpg){ #fig:fig7 width=90% }

При помощи команды я передала объектный файл компоновщику на обработку и проверила, что исполняемыый файл был создан (рис. [-@fig:fig8]). Выполнила команду (рис. [-@fig:fig9]).

![Обработка файла](fig8.jpg){ #fig:fig8 width=90% }

![Выполнение команды](fig9.jpg){ #fig:fig9 width=90% }

И, наконец, я запустила файл (рис. [-@fig:fig10]).

![Запуск файла](fig10.jpg){ #fig:fig10 width=90% }

#Выполнение задания для самостоятельной работы

В каталоге ~/work/arch-pc/lab05 с помощью cp я создала копию файла hello.asm с именем lab5.asm (рис. [-@fig:fig11])-(рис. [-@fig:fig12]).

![Создание копии файла](fig11.jpg){ #fig:fig11 width=90% }

![Переименуем файл](fig12.jpg){ #fig:fig12 width=90% }

С помощью текстового редактора я внесла измененияв текст программы в файле так, чтобы на экран выводилась строка с моими фамилией и именем (рис. [-@fig:fig13]), (рис. [-@fig:fig14]), (рис. [-@fig:fig15]), (рис. [-@fig:fig16]), (рис. [-@fig:fig17]), (рис. [-@fig:fig18]), (рис. [-@fig:fig19]).

![Запуск текстового редактора](fig13.jpg){ #fig:fig13 width=90% }

![Редактируем текст файла](fig14.jpg){ #fig:fig14 width=90% }

![Компиляция текста](fig15.jpg){ #fig:fig15 width=90% }

![Компиляция файла](fig16.jpg){ #fig:fig16 width=90% }

![Обработка файла](fig17.jpg){ #fig:fig17 width=90% }

![Выполнение команды](fig18.jpg){ #fig:fig18 width=90% }

![Запуск файла](fig19.jpg){ #fig:fig19 width=90% }

Затем я скопировала файлы hello.asm и lab5.asm в свой локальный репозиторий
в каталог ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc/labs/lab05/ (рис. [-@fig:fig20]), (рис. [-@fig:fig21]).

![Копируем lab5.asm](fig20.jpg){ #fig:fig20 width=90% }

![Копируем hello.asm](fig21.jpg){ #fig:fig21 width=90% }

И, наконец, загрузила файлы на Github.

# Выводы

В ходе лабораторной работы я освоила процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Список литературы{.unnumbered}

::: {#refs}
:::
