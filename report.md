---
# Front matter
title: "Отчёт по лабараторной работе №3"
author: "Кучен Ирзилей Сайын"

# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
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
## Misc options
indent: true
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получение практических навыков работы в консоли с атрибутами файлов для групп пользователей.

# Задание

Выполнить все пункты, занося ваши ответы на поставленные вопросы и замечания в отчёт.

# Выполнение лабораторной работы

1. 1. В установленной операционной системе создайте учётную запись пользователя guest (использую учётную запись администратора):

![Создание учетной записи](image/1.jpg){ #fig:001 width=70% }

3. Аналогично создайте второго пользователя guest2.

![Создание второго пользователя guest2.](image/3.jpg){ #fig:001 width=70% }

4. Добавьте пользователя guest2 в группу guest:

![Добавление пользователя guest2 в группу guest](image/4.jpg){ #fig:001 width=70% }

5. Осуществите вход в систему от двух пользователей на двух разных консолях: guest на первой консоли и guest2 на второй консоли.

![Вход в систему](image/5.jpg){ #fig:001 width=70% }

6. Для обоих пользователей командой pwd определите директорию, в которой вы находитесь. Сравните её с приглашениями командной строки.

![Определение директории](image/6.jpg){ #fig:001 width=70% }

7. . Уточните имя вашего пользователя, его группу, кто входит в неё
и к каким группам принадлежит он сам. Определите командами
groups guest и groups guest2, в какие группы входят пользователи guest и guest2. Сравните вывод команды groups с выводом команд
id -Gn и id -G.

![Уточнение имени пользователя](image/7.jpg){ #fig:001 width=70% }

8. Сравните полученную информацию с содержимым файла /etc/group.
Просмотрите файл командой:

![Сравнение](image/8.jpg){ #fig:001 width=70% }

9. От имени пользователя guest2 выполните регистрацию пользователя
guest2 в группе guest командой:

![Регистрация](image/9.jpg){ #fig:001 width=70% }

10. От имени пользователя guest измените права директории /home/guest,
разрешив все действия для пользователей группы:

![Изменение прав](image/10.jpg){ #fig:001 width=70% }

11. От имени пользователя guest снимите с директории /home/guest/dir1
все атрибуты командой.

![Создание](image/11.jpg){ #fig:001 width=70% }

12. Таблица 1.

![Таблица 1](image/12.jpg){ #fig:001 width=70% }

13. Таблица 2.

![Таблица 2](image/13.jpg){ #fig:001 width=70% }

# Выводы

Таким образом, в данной лабараторной работе мы научились управлять группами пользователей и задавать права, узнали какие права нужны чтобы создавать, читать и редактировать файлы для групп пользователей.
