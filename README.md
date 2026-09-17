# QA Portfolio: REST API & SQL Testing

Tech Stack & Tools:** Postman, REST API, SQL, Chrome DevTools,MS Excel

---

Приклади тест-кейсів
Повний список доступний у файлі [test_cases.xlsx](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-cases.xlsx)*

| ID | Опис тест-кейсу | Очікуваний результат | Статус | Докази |
| :--- | :--- | :--- | :--- | :--- |
| **TC-1** | PUT-запит з невалідним ID (ID 4, якого немає в БД) | 404 Not Found | **FAILED** | [Скріншот 1](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-case1.png?raw=true), [Скріншот 2](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/test-case1.1.png?raw=true) |
| **TC-13** | PUT-запит з ID "abc" (некоректний формат) | 400 Bad Request | **PASSED** | [Скріншот](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/Portfolio-2.png?raw=true),[Скріншот 2](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/Portfolio-3.png?raw=true)|

---

Приклади баг-репортів
Повний список доступний у файлі [bug_reports.xlsx](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/bug-reports.xlsx)

| ID | Короткий опис (Summary) | Severity | Priority | Докази |
| :--- | :--- | :--- | :--- | :--- |
| **BR-1** | GET-запит з неіснуючим ID повертає 400 Bad Request замість 404 | Minor | High | [Скріншот](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/bug-report.1.png?raw=true) |
| **BR-3** | PUT-запит з невалідним значенням gender повертає 200 OK замість 400 | Major | High | [Скріншот](https://github.com/strangefaux780-cmd/QA_My_Portfolio/blob/main/bug-report.3.png?raw=true) |

---

Приклади SQL-запитів
Практика створення схем БД, маніпуляції даними (DDL/DML) та вибірки:

```sql
-- Пошук конкретного користувача за ім'ям та прізвищем
SELECT * FROM PEOPLE 
WHERE FIRST_NAME = 'Олексій' AND LAST_NAME = 'Марченко';

-- Отримання списку прізвищ за алфавітом
SELECT * FROM PEOPLE 
ORDER BY LAST_NAME ASC;

-- Об'єднання даних користувача з його контактами (JOIN)
SELECT 
    p.FIRST_NAME, 
    p.LAST_NAME, 
    pb.PHONE_NUMBER, 
    pb.EMAIL_TEXT
FROM PEOPLE p
JOIN PHONE_BOOK pb ON p.PEOPLE_ID = pb.PEOPLE_ID;
