# Урок по работе с метаданными и SEO в HTML: `<meta>`. Теория: ключевые слова, описание, фавикон. Практика: добавление метаданных.

---

## 🎯 Цель урока

Познакомиться с основами использования метаданных в HTML, изучить атрибуты `<meta>`, их влияние на SEO и способы добавления ключевых элементов для оптимизации страницы.

---

## 📜 **Теория**

### Что такое метаданные в HTML?

Метаданные — это информация о веб-странице, которая не отображается напрямую на странице, но важна для поисковых систем и браузеров. Они содержат информацию о названии страницы, ключевых словах, описании и других элементах.

---

## 🔹 **Основные элементы метаданных**

---

### **1. Тег `<meta>`**

Тег `<meta>` используется для добавления метаданных в HTML-документ.

**Атрибуты `<meta>`:**

- **`name`**: Позволяет указать тип метаданных (например, `description`, `keywords`).
- **`content`**: Содержит значения для соответствующего `name`.

#### Примеры:

**Описание страницы (description):**

```html
<meta name="description" content="Учебный урок по HTML и метаданным.">
```
Ключевые слова `(keywords)`:

```html
<meta name="keywords" content="HTML, SEO, метаданные, веб-разработка">
```
Указание кодировки страницы:

```html
<meta charset="UTF-8">
```

2. Фавикон
Фавикон — это маленькая иконка, отображаемая в вкладке браузера рядом с названием сайта.

Добавление фавикона:

```html
<link rel="icon" href="favicon.ico" type="image/x-icon">
```

📝 Практика

🧩 Добавление метаданных и фавикона

Создайте файл index.html и вставьте следующий код:

```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Урок по метаданным и SEO в HTML">
    <meta name="keywords" content="HTML, SEO, метаданные, веб-разработка">
    <meta name="author" content="Ваше Имя">
    <title>Метаданные и SEO в HTML</title>
    <link rel="icon" href="favicon.ico" type="image/x-icon">
</head>
<body>

    <h1>Метаданные и SEO в HTML</h1>
    <p>Эта страница демонстрирует добавление метаданных и фавикона.</p>

</body>
</html>
```
Объяснение кода:

`<meta charset="UTF-8">` — указывает кодировку страницы.
`<meta name="description">` — описание страницы для поисковых систем.
`<meta name="keywords">` — ключевые слова для SEO.
`<link rel="icon">` — добавляет иконку в вкладку браузера.