
# Курс: Основы HTML и CSS

## Цель курса:
- Освоить базовые принципы HTML и CSS.
- Научиться создавать простые и адаптивные веб-страницы.
- Понять теоретические основы разметки и стилей.

---

## Модуль 1: Введение в HTML

### Теория:
HTML (HyperText Markup Language) — язык разметки для создания веб-страниц. Структура HTML-документа:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Моя первая страница</title>
</head>
<body>
    <h1>Добро пожаловать!</h1>
    <p>Это мой первый HTML-документ.</p>
</body>
</html>
```

### Практика:
1. Создайте файл `index.html` и напишите следующий код:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Обо мне</title>
</head>
<body>
    <h1>Привет!</h1>
    <p>Меня зовут Алексей. Я начинаю изучать веб-разработку.</p>
    <ul>
        <li>Читать книги</li>
        <li>Играть в шахматы</li>
        <li>Путешествовать</li>
    </ul>
    <a href="https://example.com">Узнать больше</a>
</body>
</html>
```

2. Откройте файл в браузере.

---

## Модуль 2: Семантические элементы HTML

### Теория:
Семантические теги делают код понятным. Например, `<header>` для шапки, `<footer>` для подвала, `<section>` для разделов.

Пример:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Семантические теги</title>
</head>
<body>
    <header>
        <h1>Добро пожаловать на мой сайт</h1>
    </header>
    <section>
        <h2>Обо мне</h2>
        <p>Я изучаю HTML и CSS.</p>
    </section>
    <footer>
        <p>&copy; 2024 Мой сайт</p>
    </footer>
</body>
</html>
```

### Практика:
Создайте страницу "Новости" с семантическими тегами:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Новости</title>
</head>
<body>
    <header>
        <h1>Новости</h1>
    </header>
    <section>
        <article>
            <h2>Новость 1</h2>
            <p>Содержание новости.</p>
        </article>
        <article>
            <h2>Новость 2</h2>
            <p>Содержание новости.</p>
        </article>
    </section>
    <footer>
        <p>Связаться с нами: <a href="mailto:info@example.com">info@example.com</a></p>
    </footer>
</body>
</html>
```

---

## Модуль 3: Основы CSS

### Теория:
CSS (Cascading Style Sheets) — язык стилей для HTML. Виды подключения:
- Встроенный:

```html
<p style="color: red;">Пример текста</p>
```

- Во внутреннем теге `<style>`:

```html
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>
```

- Через внешний файл `styles.css`:

```html
<link rel="stylesheet" href="styles.css">
```

Стили в `styles.css`:

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 0;
}

h1 {
    color: #333;
}
```

### Практика:
1. Создайте файл `styles.css` и напишите:

```css
body {
    background-color: #eaeaea;
    font-family: Arial, sans-serif;
}

h1 {
    color: #333;
    text-align: center;
}

a {
    color: blue;
    text-decoration: none;
}
```

2. Подключите файл к HTML:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Стили</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Мой стильный сайт</h1>
    <a href="#">Перейти по ссылке</a>
</body>
</html>
```

---

## Модуль 4: Flexbox

### Теория:
Flexbox помогает выравнивать элементы. Основные свойства:
- `display: flex` — превращает контейнер в flex-контейнер.
- `justify-content` — выравнивание по горизонтали.
- `align-items` — выравнивание по вертикали.

Пример:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Flexbox</title>
    <style>
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
        }

        .box {
            width: 100px;
            height: 100px;
            background-color: #007BFF;
            margin: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
    </div>
</body>
</html>
```

### Практика:
Сделайте галерею из 6 квадратов с равномерным распределением.

---
