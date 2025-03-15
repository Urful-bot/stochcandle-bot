<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StochCandle Bot</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f4f4f4;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #007BFF;
            color: white;
            padding: 60px 20px;
            text-align: center;
        }
        header h1 {
            font-size: 3rem;
            animation: fadeIn 2s ease-in-out;
        }
        header p {
            font-size: 1.2rem;
            animation: fadeIn 3s ease-in-out;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        h2 {
            color: #007BFF;
            text-align: center;
            margin-bottom: 20px;
            font-size: 2.5rem;
        }
        .features, .how-it-works, .pricing, .testimonials, .contact, .faq {
            margin-bottom: 60px;
        }
        .features ul, .faq ul {
            list-style-type: none;
            padding: 0;
        }
        .features li, .faq li {
            background-color: white;
            margin: 20px 0;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .features li:hover, .faq li:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
        }
        .features li::before {
            content: "✔️";
            margin-right: 10px;
            color: #007BFF;
        }
        .how-it-works p {
            text-align: center;
            font-size: 1.1rem;
            line-height: 1.6;
        }
        .pricing {
            text-align: center;
        }
        .pricing .price {
            font-size: 2.5rem;
            color: #007BFF;
            font-weight: bold;
        }
        .pricing .buy-button {
            display: inline-block;
            margin-top: 20px;
            padding: 15px 30px;
            background-color: #007BFF;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-size: 1.2rem;
            transition: background-color 0.3s ease;
        }
        .pricing .buy-button:hover {
            background-color: #0056b3;
        }
        .testimonials .testimonial {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            margin: 20px 0;
        }
        .testimonials .testimonial p {
            font-style: italic;
        }
        .testimonials .testimonial .author {
            text-align: right;
            font-weight: bold;
            color: #007BFF;
        }
        .contact form {
            display: flex;
            flex-direction: column;
            max-width: 600px;
            margin: 0 auto;
        }
        .contact input, .contact textarea, .contact button {
            margin: 10px 0;
            padding: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }
        .contact button {
            background-color: #007BFF;
            color: white;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .contact button:hover {
            background-color: #0056b3;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 60px;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }
            header p {
                font-size: 1rem;
            }
            h2 {
                font-size: 2rem;
            }
            .pricing .price {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>StochCandle Bot</h1>
        <p>Автоматический торговый бот для MetaTrader 5</p>
    </header>

    <div class="container">
        <!-- Преимущества -->
        <section class="features">
            <h2>Преимущества бота</h2>
            <ul>
                <li>Использует комбинацию Stochastic и ATR для точных сигналов.</li>
                <li>Низкий риск благодаря встроенному Stop Loss и Take Profit.</li>
                <li>Простая настройка и использование.</li>
                <li>Подходит для всех валютных пар и таймфреймов.</li>
            </ul>
        </section>

        <!-- Как это работает -->
        <section class="how-it-works">
            <h2>Как это работает</h2>
            <p>
                Бот анализирует рынок с помощью индикатора Stochastic и ATR. Он автоматически открывает и закрывает сделки, 
                следуя заданной стратегии. Вы можете настроить параметры риска, размер лота и другие параметры под свои нужды.
            </p>
        </section>

        <!-- Цены -->
        <section class="pricing">
            <h2>Цены</h2>
            <p class="price">$199</p>
            <a href="#contact" class="buy-button">Купить сейчас</a>
        </section>

        <!-- Отзывы -->
        <section class="testimonials">
            <h2>Отзывы</h2>
            <div class="testimonial">
                <p>"Отличный бот! За месяц использования моя прибыль выросла на 20%."</p>
                <p class="author">— Иван Петров</p>
            </div>
            <div class="testimonial">
                <p>"Простота настройки и стабильные результаты. Рекомендую!"</p>
                <p class="author">— Анна Смирнова</p>
            </div>
        </section>

        <!-- Контакты -->
        <section class="contact" id="contact">
            <h2>Свяжитесь с нами</h2>
            <form action="pronin.68.nikolay@gmail.com" method="post" enctype="text/plain">
                <input type="text" name="name" placeholder="Ваше имя" required>
                <input type="email" name="email" placeholder="Ваш email" required>
                <textarea name="message" placeholder="Ваше сообщение" rows="5" required></textarea>
                <button type="submit">Отправить</button>
            </form>
        </section>

        <!-- FAQ -->
        <section class="faq">
            <h2>Часто задаваемые вопросы</h2>
            <ul>
                <li>
                    <strong>Как установить бота?</strong>
                    <p>После покупки вы получите файл .ex5 и подробную инструкцию по установке.</p>
                </li>
                <li>
                    <strong>Какие платформы поддерживаются?</strong>
                    <p>Бот работает на MetaTrader 5.</p>
                </li>
                <li>
                    <strong>Есть ли гарантия?</strong>
                    <p>Да, мы предоставляем 30-дневную гарантию возврата средств.</p>
                </li>
            </ul>
        </section>
    </div>

    <footer>
        <p>&copy; 2023 StochCandle Bot. Все права защищены.</p>
    </footer>
</body>
</html>
