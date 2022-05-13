Этот репозиторий — является итоговым проектом курса QA Python на платформе SkillFactory. Репозиторий был создан с использованием шаблона PageObject с Selenium и PyTest (Python). 
Проект содержит UI тесты интернет-магазина "Лабиринт": https://www.labirint.ru/.

Подготовка к запуску:

Скопируйте репозиторий на свой компьютер.

Если вы используете PyCharm, он автоматически запрашивает установку необходимых библиотек.

Если нет - установите требуемые библиотеки в файле requirements.txt.

Измените следующие данные:

В Config/config.py измените путь на (актуальный для вашей ОС и версии вашего браузера) chromedriver и/или geckodriver

для macOS:
CHROME_EXECUTABLE_PATH = "/path...to/chromedriver"

для Windows:
CHROME_EXECUTABLE_PATH = "C:\\path...to\\chromedriver.exe"

Чтобы НАЧАТЬ тест: 

для запуска всех тестов команда:

для macOS: pytest Tests/* or pytest Tests

для Windows: pytest Tests

Для запуска всех тестов и регистрации результатов в формате html:

for macOS: pytest Tests/* -v --html=./hubSpot.html

for Windows: pytest Tests -v --html=./hubSpot.html

Для запуска одного набора тестов: 

pytest Tests/test_File_Name.py 

Для запуска одного теста: 

pytest Tests/test_File_Name.py::TestClassName::test_name 

Если вы запускаете тесты с журналом в html, ДЛЯ ПОЛУЧЕНИЯ ЖУРНАЛА выполнения теста:

Щелкните правой кнопкой мыши на "hubSpot.html" (файл будет создан после выполнения теста) щелкните COPY/PATH/Reference, щелкните «Absolute Path», чтобы открыть ссылку в браузере. Для получения новых результатов после выполнения «обновите» страницу с результатами.
