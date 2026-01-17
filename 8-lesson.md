# Урок 8: Основи HTTP та API

## Відео

- [Postman для початківців (БУДЕ ДОДАНИЙ ПІЗНІШЕ]()

---

## Статті

- [Огляд протоколу HTTP](https://developer.mozilla.org/uk/docs/Web/HTTP/Overview)
- [Коди стану HTTP](https://developer.mozilla.org/ru/docs/Web/HTTP/Status) (або MDN)
- [Формат JSON](https://uk.javascript.info/json)

---

## Завдання

### 1. Робота з DevTools (Network)

1. Відкрий браузер Chrome та сайт `https://jsonplaceholder.typicode.com/`.
2. Натисни `F12` (або права кнопка -> Inspect) і перейди на вкладку **Network**.
3. Онови сторінку (`F5`).
4. Знайди найперший запит у списку.
5. Розглянь вкладку **Headers**:
   - Який `Request URL`?
   - Який `Request Method`?
   - Який `Status Code`?

### 2. Встановлення Postman

Завантаж та встанови [Postman](https://www.postman.com/downloads/). Створи безкоштовний акаунт.

### 3. Перший GET запит

Використовуючи Postman, зроби запит, щоб отримати список користувачів:

- Метод: `GET`
- URL: `https://jsonplaceholder.typicode.com/users`
- Натисни **Send**.
- Перевір, що прийшов статус **200 OK** і список користувачів у форматі JSON.

### 4. Створення ресурсу (POST)

Спробуй створити нового користувача:

- Метод: `POST`
- URL: `https://jsonplaceholder.typicode.com/users`
- Вкладка **Body** -> обери **raw** -> обери тип **JSON**.
- Встав такий JSON:
  ```json
  {
    "name": "My Name",
    "username": "tester",
    "email": "test@test.com"
  }
  ```
- Натисни **Send**.
- Перевір, що прийшов статус **201 Created**.

### 5. Отримання помилки (404)

Спробуй отримати доступ до ресурсу, якого не існує:

- Метод: `GET`
- URL: `https://jsonplaceholder.typicode.com/users/9999`
- Перевір, що сервер повернув статус **404 Not Found**.

### 6. JSON Валідація

Створи локально текстовий файл `data.json`.
Напиши в ньому структуру, що описує "Курс QA":

- Назва (string)
- Тривалість в місяцях (number)
- Список тем (array of strings)
- Чи активний зараз (boolean)
- Дані про викладача (nested object: name, surname)

Скопіюй вміст файлу та перевір його валідність на сайті [JSONLint](https://jsonlint.com/).

---

> **Час проходження:** 2 дні
