# Practicum28.1

Итоговый проект по автоматизации тестирования компании Ростелеком

Для тестирования сайта были использованы:
-ручные и автоматизированные тесты;
-разбиение на классы эквивалентности;
-анализ граничных значений;
-тестирование состояний и переходов;

Чек-листы, баг-репорты, тест-кейсы :  
https://docs.google.com/spreadsheets/d/1TCkstSXgQ7QR0SSTzGnFc4DJ5GE9pzme_5Sp2Cpv0fg/edit?usp=sharing


Папка tests:
test_negative_auth_page - тестируем негативные сценарии страницы авторизации
test_negative_reg_page - тестируем негативные сценарии страницы регистрации test_negative_new_pass_page - тестируем негативные сценарии страницы восстановления пароля
test_positive_auth_page - тестируем позитивные сценарии страницы авторизации
test_positive_reg_page - тестируем позитивные сценарии страницы регистрации
test_positive_new_pass_page - тестируем позитивные сценарии страницы восстановления пароля

Папка pages:
Api_RegMail - GET-запросы к виртуальному почтовому ящику (1secmail.com) для получения валидного e-mail и кода для регистрации на сайте/восстановления пароля.
locators - локаторы XPath и CSS на web-элементы сайта
auth - функции-обёртки для локаторов, распределённые по классам в зависимости от тематики тестов
base - функции для применения к локаторам явных ожиданий, получения главной страницы сайта и пути текущей страницы
config - исходные статические данные
settings - учетные данные, используемые в процессе теста
