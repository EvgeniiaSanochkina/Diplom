# План автоматизации


## Перечень автоматизируемых сценариев

### Оплата по одобренной карте
1. нажать на кнопку Купить;
2. ввести номер карты 4444 4444 4444 4441;
3. ввести месяц;
4. ввести год;
5. ввести cvc/cvv;
6. нажать на кнопку Продолжить.

### Оплата по отклоненной карте
1. нажать на кнопку Купить;
2. ввести номер карты 4444 4444 4444 4442;
3. ввести месяц;
4. ввести год;
5. ввести cvc/cvv;
6. нажать на кнопку Продолжить.

### Покупка в кредит по одобренной карте
1. нажать на кнопку Купить;
2. ввести номер карты 4444 4444 4444 4441;
3. ввести месяц;
4. ввести год;
5. ввести cvc/cvv;
6. нажать на кнопку Продолжить.

### Покупка в кредит по отклоненной карте
1. нажать на кнопку Купить;
2. ввести номер карты 4444 4444 4444 4442;
3. ввести месяц;
4. ввести год;
5. ввести cvc/cvv;
6. нажать на кнопку Продолжить.

### Оплата по неиспользуемой карте
1. нажать на кнопку Купить;
2. ввести случайный 16-значный номер карты;
3. ввести месяц;
4. ввести год;
5. ввести cvc/cvv;
6. нажать на кнопку Продолжить.

### Покупка в кредит по неиспользуемой карте
1. нажать на кнопку Купить;
2. ввести случайный 16-значный номер карты;
3. ввести месяц;
4. ввести год;
5. ввести cvc/cvv;
6. нажать на кнопку Продолжить.


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

1. Планирование автоматизации тестирования - 1 час;
2. Написание кода тестов - 3 часа;
3. Подготовка отчетных документов по итогам автоматизированного тестирования - 1 час;
4. Подготовка отчётных документов по итогам автоматизации - 1 час.


## План сдачи работ

Автотесты и отчеты в течение недели после согласования и утверждения плана. 
