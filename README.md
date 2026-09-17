# QA_My_Portfolio
QA Portfolio: test cases, bug reports, API &amp; SQL testing

Нижче — кілька прикладів із файлу `test_cases.xlsx` (повний список — у самому файлі).

Test case 1:PUT-запит з невалідним ID (ID 4, якого немає в БД) — очікували 404, тест FAILED (знайдено баг)
(https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-case1.1.png?raw=true)
(https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-case1.png?raw=true)


Test case 13:PUT-запит з ID "abc" (некоректний формат) — очікували і отримали 400 Bad Request, тест PASSED
(https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/Portfolio-2.1.png?raw=true)
(https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/Portfolio-2.1.png?raw=true)
Повний список тест-кейсів — у файлі [test_cases.xlsx](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-cases.xlsx).


Нижче — приклади оформлення багів із файлу `bug_reports.xlsx`.

Bug report 1:GET-запит з неіснуючим ID повертає 400 Bad Request замість очікуваного 404 (Severity: Minor/High)
(https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/bug-report.1.png?raw=true)

Bug report 3:PUT-запит з невалідним значенням gender повертає 200 OK замість очікуваного 400 Bad Request (Severity: Major/High)

Повний список — у файлі [bug_reports.xlsx](посилання_на_файл).
