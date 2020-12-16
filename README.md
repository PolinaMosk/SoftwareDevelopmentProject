# Проект "S4S - Students4Students"

Целью данного проекта является разработка сайта, который решает проблему связи абитуриентов и студентов университета. В популярных социальных сетях сложно найти человека, готового проконсультировать школьника по поводу интересующего его направления. Проект позволяет школьникам и абитуриентам узнать необходимую информацию от людей из конкретных университетов, обучающихся по конкретным образовательным программам.

## Участники

Проект выполнили студенты:
* Московская П.А. (гр.3530904/80102)
* Шредер А.Д.     (гр.3530904/80102)
* Лукина В.А.     (гр.3530904/80101)

## Требования

Требования представлены в формате UML-диаграммы:
![UML-diagram](https://yadi.sk/i/LYxx9935X6OIKw)

## Диаграммы

1. System Context diagram
![System Context Diagram](https://yadi.sk/i/7iYsmpzzsd3mLA)
2. Container diagram
![System Container Diagram](https://yadi.sk/i/2tlgk2AXNN_FJw)

## Кодирование и отладка

Серверная часть сайта написана на языке Java, был также использован фреймворк Java Spring Framework. В качестве системы управления базами данных был выбран PostgreSQL. 

Клиентская часть реализована с помощью React — JavaScript-библиотеки с открытым исходным кодом для разработки пользовательских интерфейсов.

## Тестирование

Для серверной части были написаны Unit-тесты для тестирования всех эндпоинтов, для чего была использована мок-библиотека Mockito и фреймворк Spring MVC Test.

Интеграционные тесты были написаны для основных пунктов из требований: регистрация пользователя, редактирование профиля, добавление интересующих предметов, поиск подходящих студентов или старшеклассников. Для тестирования API был использован TestRestTemplate, а также дополнительная база данных PostgreSQL.Для клиентской части были реализованы тесты с использованием фреймворка Jest

## Команды запуска и тестирования

1.Серверная часть

Сборка: gradle build

Запуск: gradle bootRun

Запуск тестов: gradlew test (интеграционных – gradle test  - -tests IntegrationTesting)

2.Клиентская часть

Сборка: npm build

Запуск: npmstart

Запуск тестов: npmtest