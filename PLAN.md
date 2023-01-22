# План автоматизации


## Перечень автоматизируемых сценариев

### Оплата по одобренной карте
1. нажать на кнопку Купить;
2. ввести в поле "Номер карты" номер карты 4444 4444 4444 4441;
3. заполнить поле "Месяц";
4. заполнить поле "Год";
5. заполнить поле "Владелец";
6. заполнить поле "CVC/CVV";
7. нажать на кнопку Продолжить.
Ожидаемый результат: появление сообщения "Операция одобрена банком."

### Оплата по отклоненной карте
1. нажать на кнопку Купить;
2. ввести в поле "Номер карты" номер карты 4444 4444 4444 4442;
3. заполнить поле "Месяц";
4. заполнить поле "Год";
5. заполнить поле "Владелец";
6. заполнить поле "CVC/CVV";
7. нажать на кнопку Продолжить.
Ожидаемый результат: появление сообщения "Ошибка! Банк отказал в проведении операции."

### Покупка в кредит по одобренной карте
1. нажать на кнопку Купить;
2. ввести в поле "Номер карты" номер карты 4444 4444 4444 4441;
3. заполнить поле "Месяц";
4. заполнить поле "Год";
5. заполнить поле "Владелец";
6. заполнить поле "CVC/CVV";
7. нажать на кнопку Продолжить.
Ожидаемый результат: появление сообщения "Операция одобрена банком."

### Покупка в кредит по отклоненной карте
1. нажать на кнопку Купить;
2. ввести в поле "Номер карты" номер карты 4444 4444 4444 4442;
3. заполнить поле "Месяц";
4. заполнить поле "Год";
5. заполнить поле "Владелец";
6. заполнить поле "CVC/CVV";
7. нажать на кнопку Продолжить.
Ожидаемый результат: появление сообщения "Ошибка! Банк отказал в проведении операции."

### Проверка полей формы
1. поле "Номер карты" заполняется цифрами в количестве 16-ти символов;
2. поле "Месяц" заполняется цифрами в количестве 2-х символов в диапазоне от 01 до 12;
3. поле "Год" заполняется цифрами в количестве 2-х символов в диапазоне от 23 до 28;
4. поле "Владелец" заполняется латинскими буквами в количестве 64-х символов. Допускается использование пробела и дефиса. 
5. поле "CVC/CVV" заполяется цифрами в количестве 3-х символов.


## Перечень используемых инструментов

* Java 11 - язык программирования для написания автоматизированных тестов.
* IntelliJ IDEA - интегрированная среда разработки программного обеспечения языков программирования, в частности Java.
* Docker - система контейнеров для запуска эмуляторов MySQL и PostgreSQL для воссоздания работы банковского сервиса и подключения к нему через Node js.
* Gradle - система автоматической сборки, используемая для подключения зависимостей, которые выкачивают нужные библиотеки. По сравнению с Maven считается более удобным, т.к. многие конструкции в нем выглядят короче. Также используется для настройки CI (в моём аккаунте на GitHub не запускается Appveyor, использую Gradle как альтернативу)
* JUnit5 - платформа для написания автотестов и их запуска.
* Git и GitHub — хранение кода, в том числе автотестов.
* Faker - библиотека для генерирования фейковых данных, используемых для прогона тестов.
* Lombok - библиотека Java, позволяющая сократить шаблонный код.
* Selenide - фреймворк для автоматизированного тестирования веб-
* приложений.
* Allure Report - система подготовки отчетов. Удобная и понятная в исполнении.


## Возможные риски при автоматизации

Сложности в написании тестов при отсутствии уникальных css-селекторов;
Ошибки в изначальном коде, влекущие за собой некорректность работы приложения и падение теста;


## Интервальная оценка с учетом рисков в часах

1. Планирование автоматизации тестирования - 3 часа;
2. Написание кода тестов - 20 часов;
3. Подготовка отчетных документов по итогам автоматизированного тестирования - 3 часа;
4. Подготовка отчётных документов по итогам автоматизации - 3 часа.


## План сдачи работ

Автотесты и отчеты до 01.02.2023. 