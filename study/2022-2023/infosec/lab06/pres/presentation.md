---
# Front matter
lang: ru-RU
title: Защита лабораторной работы №6.Мандатное разграничение прав в Linux
author: "Смородова Дарья Владимировна"
group: НФИбд-01-19
institute: RUDN University, Moscow, Russian Federation
date: 2022  Oct 15th

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

- Развить навыки администрирования ОС Linux;

- Получить первое практическое знакомство с технологией SELinux1;

- Проверить работу SELinx на практике совместно с веб-сервером Apache.

# Результаты выполнения лабораторной работы

## Задание параметра ServerName  

![Задание параметра ServerName](pics/1.png){ #fig:001 width=70% }

## Отключение фильтра] 

![Отключение фильтра](pics/2.png){ #fig:002 width=70% height=70% }

## Проверка режима и политики

![Проверка режима и политики](pics/3.png){ #fig:003 width=70% height=70% }

## Проверка статуса

![Проверка статуса](pics/4.png){ #fig:004 width=70% height=70% }

## Веб-сервер Apache

![Веб-сервер Apache](pics/5.png){ #fig:005 width=70% height=70% }

## Просмотр переключателей SELinux для Apache

![Просмотр переключателей SELinux для Apache](pics/6.png){ #fig:006 width=70% height=70% }

## Статистика по политике

![Статистика по политике](pics/7.png){ #fig:007 width=70% height=70% }

## Определение типов файлов и поддиректорий в директории /var/www

![Определение типов файлов и поддиректорий в директории /var/www](pics/8.png){ #fig:008 width=70% height=70% }

## Определение типов файлов  в директории /var/www/html

![Определение типов файлов  в директории /var/www/html](pics/9.png){ #fig:009 width=70% height=70% }

## Создание файла

![Создание файла](pics/10.png){ #fig:010 width=70% height=70% }

## Проверка контекста

![Проверка контекста](pics/11.png){ #fig:011 width=70% height=70% }

## Получение доступа к файлу через браузер

![Получение доступа к файлу через браузер](pics/12.png){ #fig:012  width=70% height=70%}

## Проверка контекста файла

![Проверка контекста файла](pics/13.png){ #fig:013  width=70% height=70% }

## Изменение контекста файла /var/www/html/test.html

![Изменение контекста файла /var/www/html/test.html](pics/14.png){ #fig:014  width=70% height=70% }

## Получение доступа к файлу через браузер

![Получение доступа к файлу через браузер](pics/15.png){ #fig:015  width=70% height=70% }

## Просмотр log-файла веб-сервера Apache

![Просмотр log-файла веб-сервера Apache](pics/16.png){ #fig:016  width=70% height=70%}

## Изменеие ТСР-порта с 80 на 81

![Изменеие ТСР-порта с 80 на 81](pics/17.png){ #fig:017  width=70% height=70% }

## Анализ и просмотр лог-файлов  

![Анализ и просмотр лог-файлов](pics/18.png){ #fig:018  width=70% height=70% }

## Выполнение и проверка списка портов 

![Выполнение и проверка списка портов](pics/19.png){ #fig:019  width=70% height=70% }

## Возвращение контекста

![Возвращение контекста](pics/20.png){ #fig:020  width=70% height=70% }

## Получение доступа к файлу через браузер

![Получение доступа к файлу через браузер](pics/21.png){ #fig:021  width=70% height=70% }

## Исправленный файл apache

![Исправленный файл apache](pics/23.png){ #fig:022 width=70% height=70% }

## Удаление привязки к 81 порту и удаление файла 

![Удаление привязки к 81 порту и удаление файла](pics/22.png){ #fig:023 width=70% height=70% }

# Выводы   

- Развили навыки администрирования ОС Linux;

- Получили первое практическое знакомство с технологией SELinux1;

- Проверили работу SELinx на практике совместно с веб-сервером Apache.
