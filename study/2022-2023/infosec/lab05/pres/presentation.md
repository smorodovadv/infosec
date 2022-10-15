---
# Front matter
lang: ru-RU
title: Защита лабораторной работы №5. Дискреционное разграничение прав в Linux. Исследование влияния дополнительных атрибутов
author: "Смородова Дарья Владимировна"
group: НФИбд-01-19
institute: RUDN University, Moscow, Russian Federation
date: 2022  Oct 8th

# Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true

---

# Цель выполнения лабораторной работы 

Изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов. Получение практических навыков работы в консоли с дополнительными атрибутами. Рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

# Результаты выполнения лабораторной работы

## Проверка установки компилятора gcc

![Проверка установки компилятора gcc](pics/1.png){ #fig:001 width=70% }

## Отключение системы запретов

![Отключение системы запретов](pics/2.png){ #fig:002 width=70% }

## Проверка компиляторов

![Проверка компиляторов](pics/3.png){ #fig:003 width=70% }

## Содержимое файла simpleid.c

![Содержимое файла simpleid.c](pics/5.png){ #fig:005 width=70% }

## Компиляция и запуск файла simpleid.c

![Компиляция и запуск файла simpleid.c ](pics/6.png){ #fig:006 width=70% }

## Команда id

![Команда id](pics/7.png){ #fig:007 width=70% }

## Содержимое файла simpleid2.c

![Содержимое файла simpleid2.c](pics/8.png){ #fig:008 width=70% }

## Компиляция и запуск файла simpleid2.c

![Компиляция и запуск файла simpleid2.c](pics/9.png){ #fig:009 width=70% }

## Команды chown и chmod

![Команды chown и chmod](pics/10.png){ #fig:010 width=70% }

## Проверка правильности установки новых атрибутов

![Проверка правильности установки новых атрибутов](pics/11.png){ #fig:011 width=70% }

## Запуск simpleid2 и id

![Запуск simpleid2 и id](pics/12.png){ #fig:012 width=70% }

## Сравнение SetGID-бита

![Сравнение SetGID-бита](pics/13.png){ #fig:013 width=70% }

## Содержание файла readfile.c

![Содержание файла readfile.c](pics/14.png){ #fig:014 width=70% }

## Компиляция файла readfile.c

![Компиляция файла readfile.c](pics/15.png){ #fig:015 width=70% }

## Смена владельца и прав у файла readfile.c 

![Смена владельца и прав у файла readfile.c ](pics/16.png){ #fig:016 width=70% }

## Проверка возможности прочитать файл readfile.c  

![Проверка возможности прочитать файл readfile.c ](pics/17.png){ #fig:017 width=70% }

## Смена у программы readfile владельца и установка SetU’D-бит 

![Смена у программы readfile владельца и установка SetU’D-бит](pics/18.png){ #fig:018 width=70% }

## Проверка возможности прочитать файл readfile.c

![Проверка возможности прочитать файл readfile.c ](pics/19.png){ #fig:019 width=70% }

## Проверка возможности прочитать файл /etc/shadow 

![Проверка возможности прочитать файл /etc/shadow ](pics/20.png){ #fig:020 width=70% }

## Проверка установки атрибута Sticky на директории /tmp

![Проверка установки атрибута Sticky на директории /tmp ](pics/21.png){ #fig:021 width=70% }

## Создание файла file01.txt в директории /tmp со словом test 

![Создание файла file01.txt в директории /tmp со словом test ](pics/22.png){ #fig:022 width=70% }

## Просмотр атрибутов и разрешение чтения и записи для категории пользователей «все остальные»  

![Просмотр атрибутов и разрешение чтения и записи для категории пользователей «все остальные» ](pics/23.png){ #fig:023 width=70% }

## Попытка прочитать файл /tmp/file01.txt от пользователя guest2 

![Попытка прочитать файл /tmp/file01.txt от пользователя guest2 ](pics/24.png){ #fig:024 width=70% }

## Попытка дозаписать в файл /tmp/file01.txt слово test2 от пользователя guest2  

![Попытка дозаписать в файл /tmp/file01.txt слово test2 от пользователя guest2 ](pics/25.png){ #fig:025 width=70% }

## Попытка перезаписать файл /tmp/file01.txt словом test3 от пользователя guest2 

![Попытка перезаписать файл /tmp/file01.txt словом test3 от пользователя guest2 ](pics/26.png){ #fig:026 width=70% }

## Попытка удалить файл /tmp/file01.txt от пользователя guest2 

![Попытка удалить файл /tmp/file01.txt от пользователя guest2 ](pics/27.png){ #fig:027 width=70% }

## Снятие атрибута t с директории /tmp 

![Снятие атрибута t с директории /tmp](pics/28.png){ #fig:028 width=70% }

## Проверка снятия атрибута t с директории /tmp

![Проверка снятия атрибута t с директории /tmp](pics/29.png){ #fig:029 width=70% }

## Повтор предыдущих шагов

![Повтор предыдущих шагов](pics/30.png){ #fig:030 width=70% }

## Возвращение атрибута t директории /tmp

![Возвращение атрибута t директории /tmp](pics/31.png){ #fig:031 width=70% }

# Выводы   

-  Изучили механизмы изменения идентификаторов, применения SetUID- и Sticky-битов;

- Получили практические навыки работы в консоли с дополнительными атрибутами;

- Рассмотрели работу механизма смены идентификатора процессов пользователей и влияние бита Sticky на запись и удаление файлов.