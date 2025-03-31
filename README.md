<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Портфолио Дизайнера</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: #f4f4f4;
            overflow-x: hidden;
        }
        .hero {
            text-align: center;
            padding: 100px 20px;
            background: linear-gradient(135deg, #ff7eb3, #ff758c);
            color: white;
            position: relative;
        }
        .scroll-down {
            margin-top: 20px;
            font-size: 18px;
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
        }
        .scroll-down:hover {
            transform: translateY(5px);
        }
        .portfolio {
            text-align: center;
            padding: 50px 20px;
            background: white;
        }
        .gallery {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            justify-content: center;
        }
        .item {
            width: 250px;
            height: 200px;
            background-size: cover;
            background-position: center;
            transition: transform 0.3s, filter 0.3s;
            border-radius: 10px;
            cursor: pointer;
        }
        .item:hover {
            transform: scale(1.1);
            filter: brightness(1.2);
        }
        .about, .contact {
            text-align: center;
            padding: 50px 20px;
            background: #f8f8f8;
        }
        form input, form textarea, form button {
            display: block;
            width: 80%;
            margin: 10px auto;
            padding: 10px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
        }
        form input, form textarea {
            background: white;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        form button {
            background: #ff758c;
            color: white;
            cursor: pointer;
            transition: background 0.3s;
        }
        form button:hover {
            background: #ff5771;
        }
        footer {
            text-align: center;
            padding: 20px;
            background: #333;
            color: white;
        }
    </style>
</head>
<body>
    <header class="hero">
        <h1>Привет, я Дизайнер</h1>
        <p>Создаю уникальные интерьеры и экстерьеры</p>
        <div class="scroll-down">⮟ Прокрутите вниз ⮟</div>
    </header>

    <section class="portfolio">
        <h2>Мои работы</h2>
        <div class="gallery">
            <div class="item" style="background-image: url('interior1.jpg');"></div>
            <div class="item" style="background-image: url('exterior1.jpg');"></div>
            <div class="item" style="background-image: url('interior2.jpg');"></div>
            <div class="item" style="background-image: url('exterior2.jpg');"></div>
        </div>
    </section>

    <section class="about">
        <h2>Обо мне</h2>
        <p>Я создаю стильные и функциональные пространства, вдохновляя людей на перемены.</p>
    </section>

    <section class="contact">
        <h2>Свяжитесь со мной</h2>
        <form>
            <input type="text" placeholder="Ваше имя" required>
            <input type="email" placeholder="Ваш email" required>
            <textarea placeholder="Ваше сообщение" required></textarea>
            <button type="submit">Отправить</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Все права защищены</p>
    </footer>
</body>
</html>
