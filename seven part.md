# Урок по работе с формами в HTML: `<form>`. Теория: input, textarea, кнопки отправки. Практика: форма регистрации.

---

## 🎯 Цель урока

Познакомиться с основами работы с HTML-формами, изучить теги `<form>`, элементы `<input>`, `<textarea>` и кнопки отправки, а также создать форму регистрации.

---

## 📜 **Теория**

### Что такое HTML-форма?

HTML-форма (`<form>`) используется для сбора данных от пользователей. Она позволяет отправлять информацию на сервер или обрабатывать её локально.

---

## 🔹 **Основные элементы формы в HTML**

---

### **1. `<form>`**

Тег `<form>` является контейнером для всех элементов формы.

**Атрибуты:**

- `action`: URL, на который отправляются данные.
- `method`: Метод отправки данных (`GET` или `POST`).
  - `GET`: Данные передаются в URL.
  - `POST`: Данные отправляются в теле запроса.

**Пример использования:**

```html
<form action="submit_form.php" method="POST">
    <!-- Элементы формы здесь -->
</form>
```
### **2. `<input>`**
Тег `<input>` используется для создания различных элементов формы: текстовых полей, чекбоксов, радиокнопок и других.

Атрибуты `<input>`:

type: Определяет тип элемента формы (text, password, email, submit и т.д.).
name: Имя элемента формы (используется для обработки данных).
placeholder: Подсказка для пользователя.

Примеры:

Текстовое поле:

```html
<input type="text" name="username" placeholder="Введите имя">
```

Парольное поле:

```html
<input type="password" name="password" placeholder="Введите пароль">
```

Кнопка отправки:

```html
<input type="submit" value="Отправить">
```

### **2. `<textarea>`**
Тег `<textarea>` используется для создания многострочного текстового поля.

Пример использования:

```html
<textarea name="message" rows="4" cols="50" placeholder="Напишите сообщение"></textarea>
```

### **4. Кнопки отправки и сброса**
Кнопка отправки
Тег `<input type="submit">` отправляет данные формы.

Пример:

```html
<input type="submit" value="Отправить">
```

Кнопка сброса
Тег `<input type="reset">` очищает все поля формы.

Пример:

```html
<input type="reset" value="Очистить">
```
📝 Практика

🧩 Создание формы регистрации

Создайте файл index.html и вставьте следующий код:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Форма регистрации</title>
    <style>
        body { font-family: Arial; padding: 20px; max-width: 400px; margin: 0 auto; }
        input, textarea, button { width: 100%; margin-top: 10px; padding: 10px; }
        button { cursor: pointer; background-color: #007BFF; color: white; border: none; }
        button:hover { background-color: #0056b3; }
    </style>
</head>
<body>

    <h1>Форма регистрации</h1>

    <form action="submit_form.php" method="POST">
        <label for="username">Имя пользователя</label>
        <input type="text" id="username" name="username" placeholder="Введите имя" required>

        <label for="email">Электронная почта</label>
        <input type="email" id="email" name="email" placeholder="Введите email" required>

        <label for="password">Пароль</label>
        <input type="password" id="password" name="password" placeholder="Введите пароль" required>

        <label for="message">Сообщение</label>
        <textarea id="message" name="message" rows="4" placeholder="Напишите сообщение"></textarea>

        <input type="submit" value="Отправить">
        <input type="reset" value="Очистить">
    </form>

</body>
</html>
```
