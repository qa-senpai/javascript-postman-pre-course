# Урок 6: Об'єкти

## Відео

- [Об'єкти. Основи](https://youtu.be/45b3A6L60Hw?si=YK_x9JlAPGpLSuAx)

---

## Статті

- [Об'єкти](https://uk.javascript.info/object)
- [Копіювання об'єктів і посилання](https://uk.javascript.info/object-copy)
- [Методи об'єкта, "this"](https://uk.javascript.info/object-methods)

---

## Завдання

### 1. Створення об'єкта

Створи об'єкт `user` із властивостями:

- `name` (ім'я)
- `age` (вік)
- `city` (місто)
- `isAdmin` (чи є адміном - boolean)

### 2. Зміна властивостей

- Зміни значення `age` в об'єкті `user`.
- Додай нову властивість `email`.
- Видали властивість `city`.
  Виведи оновлений об'єкт у консоль.

### 3. Функція для створення об'єктів

Напиши функцію `makeUser(name, age)`, яка приймає два параметри та повертає об'єкт із полями `name` і `age`.

```javascript
let user1 = makeUser("Ivan", 30);
console.log(user1); // { name: "Ivan", age: 30 }
```

### 4. Метод об'єкта

Додай до об'єкта `user` (із першого завдання) метод `sayHi()`, який виводить:
`"Привіт, мене звати [name]!"`.
Використовуй ключове слово `this`.

### 5. Перебір властивостей

Використовуй цикл `for..in`, щоб вивести всі ключі та значення об'єкта `user`.

---

> **Час проходження:** 2 дні

## Мої ресурси:

- [Сайт](https://qa-senpai.github.io/dojo/details-e2e.html)
- [YouTube](https://www.youtube.com/@qa_senpai)
- [Telegram](https://t.me/qa_advice)
