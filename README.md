# QA_My_Portfolio
QA Portfolio: test cases, bug reports, API &amp; SQL testing
## Приклади тест-кейсів

Нижче — кілька прикладів із файлу `test_cases.xlsx` (повний список — у самому файлі).

Test case 1:PUT-запит з невалідним ID (ID 4, якого немає в БД) — очікували 404, тест FAILED (знайдено баг)
https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-case1.1.png?raw=true
https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-case1.png?raw=true


Test case 13:PUT-запит з ID "abc" (некоректний формат) — очікували і отримали 400 Bad Request, тест PASSED

Повний список тест-кейсів — у файлі [test_cases.xlsx](посилання_на_файл).

## Приклади баг-репортів

Нижче — приклади оформлення багів із файлу `bug_reports.xlsx`.

**Баг 1: [короткий опис бага]**
![Bug report 1](сюди_посилання_на_скрін_1.png)

**Баг 2: [короткий опис бага]**
![Bug report 2](сюди_посилання_на_скрін_2.png)

Повний список — у файлі [bug_reports.xlsx](посилання_на_файл).
