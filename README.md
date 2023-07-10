# Summary
## 1. Перечень автоматизируемых сценариев: ##
### *Перечень сценариев навигации к форме:* ###
* Со страницы курса: Тестировщик ПО-Записаться-Запишитесь на курс
* Со страницы курса: Тестировщик ПО (прокрутить страницу вниз)-Запишитесь на курс

* Главная страница-Программирование-Тестировщик ПО-Записаться-Запишитесь на курс
* Главная страница-Программирование-Тестировщик ПО (прокрутить страницу вниз)-Запишитесь на курс

* Главная страница-Каталог курсов-Программирование-Тестировщик ПО-Записаться-Запишитесь на курс
* Главная страница-Каталог курсов-Программирование-Тестировщик ПО (прокрутить страницу вниз)-Запишитесь на курс

* Главная страница-Каталог курсов-Программирование-ввести в поисковую строку Тестировщик ПО-клик на выпадающему списку-Записаться-Запишитесь на курс
* Главная страница-Каталог курсов-Программирование-ввести в поисковую строку Тестировщик ПО (прокрутить страницу вниз)-Запишитесь на курс

* Главная страница-Каталог курсов-Программирование-ввести в поисковую строку Тестировщик-найти курс-Тестировщик ПО-Записаться-Запишитесь на курс
* Главная страница-Каталог курсов-Программирование-ввести в поисковую строку Тестировщик-найти курс-Тестировщик ПО (прокрутить страницу вниз)-Запишитесь на курс

### *Перечень сценариев заполнения и отправки формы:* ###

#### *Позитивный сценарий:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Ввести валидный номер телефона в поле Телефон (пример, 89051234567)
3. Нажать Записаться
4. Ожидаемый результат: появление сообщения "Спасибо! Наш менеджер свяжется с Вами!"

#### *Негативный сценарий ввода символов в поле Имя:* ####
1. Ввести символы в поле Имя (пример, !"№;%:?*()_)
2. Ввести валидный номер телефона в поле Телефон (пример, 89051234567)
3. Нажать Записаться
4. Ожидаемый результат: под полем Имя появление сообщения об ошибке "Должно состоять из букв"

#### *Негативный сценарий ввода пробелов в поле Имя:* ####
1. Ввести цифры в поле Имя (пример, "                            ")
2. Ввести валидный номер телефона в поле Телефон (пример, 89051234567)
3. Нажать Записаться
4. Ожидаемый результат: под полем Имя появление сообщения об ошибке "Обязательное поле"

#### *Негативный сценарий отправки пустого поля Имя:* ####
1. Ввести валидный номер телефона в поле Телефон (пример, 89051234567)
2. Нажать Записаться
3. Ожидаемый результат: под полем Имя появление сообщения об ошибке "Обязательное поле"

#### *Негативный сценарий ввода английского значения в поле Телефон:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Ввести значение на английском языке в поле Телефон (пример, Qwerfghjku)
3. Нажать Записаться
4. Ожидаемый результат: под полем Телефон появление сообщения об ошибке "Номер в формате +9 (999) 999-99-99"

#### *Негативный сценарий ввода символов в поле Телефон:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Ввести символы в поле Телефон (пример, !"№;%:?*()_)
3. Нажать Записаться
4. Ожидаемый результат: под полем Телефон появление сообщения об ошибке "Номер в формате +9 (999) 999-99-99"

#### *Негативный сценарий ввода пробелов в поле Телефон:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Ввести пробелы в поле Телефон (пример, "                           ")
3. Нажать Записаться
4. Ожидаемый результат: под полем Телефон появление сообщения об ошибке "Обязательное поле"

#### *Негативный сценарий отправки пустого поля Телефон:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Нажать Записаться
3. Ожидаемый результат: под полем Телефон появление сообщения об ошибке "Обязательное поле"

#### *Негативный сценарий граничных значений поля Телефон:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Ввести 9 цифр в поле Телефон (пример, +7 (999) 999-99-9)
3. Нажать Записаться
4. Ожидаемый результат: под полем Телефон появление сообщения об ошибке "Номер в формате +9 (999) 999-99-99"

#### *Негативный сценарий граничных значений поля Телефон:* ####
1. Ввести валидное имя в поле Имя (пример, Василий)
2. Ввести 11 цифр в поле Телефон (пример, +7 (999) 999-99-999)
3. Нажать Записаться
4. Ожидаемый результат: под полем Телефон появление сообщения об ошибке "Номер в формате +9 (999) 999-99-99"

#### *Негативный сценарий отправки пустой формы:* ####                       )
1. Нажать Записаться
2. Ожидаемый результат: под полем Имя появление сообщения об ошибке "Обязательное поле", под полем Телефон появление сообщения об ошибке "Обязательное поле"

Для данной формы нет ограничения на ввод символов и допустима английская раскладка в поле Имя, поэтому эти сценарии не реализованы.

## 2. Перечень используемых инструментов с обоснованием выбора: ##
* IntelliJIDEA для написания кода тестов
* JUnit5 для юнит-тестов
* Allure для визуальной наглядности
* GitHub с CI для хранения, общего доступа и непрерывной интеграции
* Maven/Gradle системы управления проектами
* Selenium/Selenid инструменты автоматизации браузеров
* Системы виртуализации, например, Virtual Box, для кроссплатформенного тестирования
* Различные популярные браузеры (Опера, Хром, Мозила)
* Apache JMeter для нагрузочного тестирования (при необходимости)
* Postman для отправки запросов и получения ответов от сервера

## 3. Перечень необходимых разрешений, данных и доступов: ##
* Разрешение на проведение тестов, на нагрузочное тестирование (при необходимости)
* Тестовый режим (если имеется)
* Тестовые данные (имя, номер телефона) на которые операторы не будут звонить

## 4. Перечень и описание возможных рисков при автоматизации: ##
* Проблемы с идентификацией полей ввода
* Неработающий заявленный функционал
* Стоимость автоматизации

## 5. Перечень необходимых специалистов для автоматизации: ##
* Для реализации данных сценариев, предполагаю, необходим один грамотный инженер по автоматизации

## 6. Интервальная оценка с учётом рисков в часах: ##
* Планировние - 4 часа
* Установка необходимых инструментов, настройка окружения - 3 часа
* Написание кода - 20 часов
* Тестирование и написание отчетов - 10 часов\
*Итого:* 37 часов
