# Урок по семантическим элементам HTML: `<header>`, `<footer>`, `<section>`, `<article>`. Практика: макет страницы новостей.

---

## 🎯 Цель урока

Познакомиться с основами семантических элементов HTML и научиться создавать макет страницы новостей с использованием элементов `<header>`, `<footer>`, `<section>`, `<article>`.

---

## 📜 **Теория**

### Что такое семантические элементы HTML?

**Семантические элементы** в HTML используются для того, чтобы сделать структуру веб-страницы более понятной и доступной для поисковых систем и экранных технологий. Они описывают смысловую структуру контента, а не только его оформление.

---

## 🔹 **Основные семантические элементы HTML**

---

### **1. `<header>`**

Тег `<header>` содержит вводный контент или навигацию для документа или секции. Обычно в нем располагаются:

- Название сайта
- Логотипы
- Навигационные ссылки
- Заголовки страницы

**Пример:**

```html
<header>
    <h1>Мой новостной сайт</h1>
    <nav>
        <a href="#">Главная</a> | <a href="#">О нас</a> | <a href="#">Контакты</a>
    </nav>
</header>
```
### **2. `<footer>`**
Тег `<footer>` представляет нижнюю часть документа или секции. Обычно в нем содержится:

Информация об авторских правах
Контактная информация
Дополнительные ссылки и навигация
Пример:

```html
<footer>
    <p>&copy; 2024 Мой новостной сайт. Все права защищены.</p>
</footer>
```

### **3. `<section>`**
Тег `<section>` используется для создания логически обособленных частей контента. Обычно он содержит заголовки и подзаголовки.

Пример:

```html

Копировать код
<section>
    <h2>Спорт</h2>
    <p>Последние новости о футболе и теннисе.</p>
</section>
```
### **4. `<article>`**
Тег `<article>` используется для создания независимого и самостоятельно понимаемого контента. Часто используется для:

Статей
Блогов
Новостей

Пример:

```html
<article>
    <h2>Заголовок новости</h2>
    <p>Текст новости, автор, дата и другие детали.</p>
</article>
```

📝 Практика

🧩 Создание макета страницы новостей

Создайте файл index.html и напишите следующий код:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Новостной сайт</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
        header, footer { background-color: #f4f4f4; padding: 1em; text-align: center; }
        nav a { text-decoration: none; color: #333; margin: 0 10px; }
        section { padding: 20px; }
        article { padding: 15px; border: 1px solid #ddd; margin-bottom: 15px; }
        article h2 { margin-top: 0; }
    </style>
</head>
<body>

    <!-- Верхняя часть страницы -->
    <header>
        <h1>Мой новостной сайт</h1>
        <nav>
            <a href="#">Главная</a>
            <a href="#">О нас</a>
            <a href="#">Контакты</a>
        </nav>
    </header>

    <!-- Основной контент -->
    <section>
        <h2>Технологии</h2>

        <article>
            <h2>Обновления в мире IT</h2>
            <p>Сегодня в мире технологий произошли важные события...</p>
        </article>

        <article>
            <h2>Развитие искусственного интеллекта</h2>
            <p>Искусственный интеллект стремительно развивается и внедряется...</p>
        </article>
    </section>

    <!-- Нижняя часть страницы -->
    <footer>
        <p>&copy; 2024 Мой новостной сайт. Все права защищены.</p>
    </footer>

</body>
</html>
```