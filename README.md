В данном разделе представлена моя итоговая аттестационная работа на тему: "Тестовая документация и тестирование функционала регистрации на сайте Habr.com"

В рамках данной работы были поставлены следующие ключевые задачи:
* определить стратегию тестирования функционала регистрации сайта Habr.com;
* определить список требований к тестовой среде;
* спроектировать и написать тест-кейсы для проверки функционала регистрации;
* провести тестирование, согласно написанным тест-кейсам;
* составить баг-репорты в случае обнаружения дефектов;
* подвести итоги по результатам тестирования, вычислить метрики оценки качества программного продукта и составить список замечаний и предложений на улучшение по результатам прогона тестов.

С целью решения поставленных задач мной было проведено исследование производительности сайта https://habr.com за май – июль 2022г. (3 месяца) с целью выявления степени его актуальности по всему миру и в частности в РФ, построения стратегии тестирования данного ресурса.
Руководствуясь полученными статистическими данными, выстроена стратегия тестирования функционала регистрации данного ресурса.

Необходимо:
* Включить тестирование локализации в общий объём работ.
* Протестировать функционал регистрации, как на ПК, так и на мобильных устройствах.
* Протестировать функционал регистрации на различных браузерах, определив список требований к среде, исходя из географии пользователей и статистических данных о наиболее популярных браузерах в той или иной локали.

Объём проекта ограничен функциональным тестированием и тестированием user интерфейса с применением методов ручного тестирования.
Статистические данные о наиболее популярных браузерах в России и в мире получены путём анализа доли рынка топ браузеров на ПК и мобильных устройствах с помощью платформы SimilarWeb.
По результатам исследования определён список требований к тестовой среде. 

В рамках проекта было разработано 6 тест-кейсов и запущено (Executed Test Cases) 36 тестов. Результаты тестирования показали, что число успешных тестов (Passed Test Cases) в количественном и процентном соотношении составило – 14 (38.89%), а упавших тестов (Failed Test Cases) – 22 (61.11%).
Полученное соотношение успешных тестов к проваленным обусловлено спецификой итоговой аттестационной работы, в объём работ включены только те тестовые случаи, которые привели к обнаружению дефектов, либо успешно пройдены, но в ходе проверки возникли предложения по улучшению работы той или иной функциональности.

По результатам тестирования было выявлено 4 дефекта и составлены соответственно баг-репорты. Большинство найденных дефектов имеют среднюю степень серьёзности и оказывают влияние на удобство использования формы регистрации на сайте.
Один дефект имеет высокую степень серьёзности, т.к. оказывает влияние на ключевой функционал. Регистрация в системе пользователей с электронной почтой с несуществующими доменными именами приводит к захламлению базы данных, кроме того если на сайте существует рассылка писем клиентам, то вся та часть писем с некорректных e-mail будет возвращена отправителю.
Регистрация множества подобных пользователей в системе, затрудняет прохождение регистрации реальным посетителям сайта, т.к. входные данные для регистрации (например, никнейм пользователя) уже могут быть заняты.

Впоследствии, уже после успешного завершения курса, по мере изучения мной дополнительных инструментов тестировщика, в частности tms систем, работа была дополнена. Тест-кейсы занесены в TestRail, созданы Test Runs - тестовые прогоны, сформированные под каждую определённую требованиями тестовую среду, получены результаты запуска тестов, метрики в виде круговых диаграмм. 
