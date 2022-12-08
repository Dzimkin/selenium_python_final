# selenium_python_final
Полноценный тестовый проект

base_page.py - тут мы храним методы которые применяются по всему проекту вообще, всё завернуто в класс, чтобы было удобно импортировать.

locators.py - тут мы храним локаторы, в виде констант. Локаторы каждой отдельной страницы завёрнуты в класс, чтобы было удобно импортировать

main_page.py - тут мы храним методы по конкретной странице, завернутые в класс этой странице. Класс этот - условный MainPage - наследник класса BasePage, чтобы можно было пользоваться методами, описанными в base_page.py

И вот тут ступор. Файл test_main_page.py - тут мы выполняем сами тесты? по префиксу "test_" я понимаю что это для PyTest. Тут вызванные функции будут запускаться.

Здесь мы будем создавать функции, которым:

выдаём нужный для проверки линк
создаём в функции переменную page, которой передаём браузер из base_page.py(класс BasePage) и линк из шага №1
следом говорим "page, откройся", но методом из base_page.py(класс BasePage)
добавляем проверки, которые создавали методами в main_page.py
<div class="badge-base LI-profile-badge" data-locale="ru_RU" data-size="large" data-theme="light" data-type="VERTICAL" data-vanity="guzich" data-version="v1"><a class="badge-base__link LI-simple-link" href="https://pl.linkedin.com/in/guzich?trk=profile-badge">Dmitry G.</a></div>
              
