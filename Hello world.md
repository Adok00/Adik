<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Аренда строительного оборудования</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        /* Шапка */
        .header {
            height: 100vh;
            position: relative;
            overflow: hidden;
        }

        .slider {
            width: 100%;
            height: 100%;
            position: absolute;
            animation: slide 12s infinite; /* 4 картинки × 3 секунды = 12 секунд */
            background-size: cover;
            background-position: center;
        }

        @keyframes slide {
            0% {
                background-image: url('https://bigfoto.top/uploads/posts/2022-10/1666461540_11-bigfoto-top-p-spetstekhniki-kartinki-18.jpg');
            }
            25% {
                background-image: url('https://transline.kz/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fabout.b94115df.webp&w=3840&q=75');
            }
            50% {
                background-image: url('https://assets-global.website-files.com/621f30168f38525d6967fb5f/624ef8b734b4a81a5e3e5eb0_construction.png');
            }
            75% {
                background-image: url('https://i.artfile.me/wallpaper/26-08-2017/1920x1080/tehnika-stroitelnaya-tehnika-case-1216675.jpg');
            }
            100% {
                background-image: url('https://vegas-dev.com/system/App/Models/Portfolio/259/cover/back/original/hv-market-internet-magazin-back.jpg');
            }
        }

        /* Навигация */
        .nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(0,0,0,0.8);
            padding: 20px;
            z-index: 1000;
        }

        .nav a {
            color: white;
            text-decoration: none;
            margin: 0 20px;
            font-size: 18px;
        }

        /* Общие стили секций */
        section {
            padding: 80px 20px;
            max-width: 1400px;
            margin: 0 auto;
        }

        h2 {
            text-align: center;
            margin-bottom: 50px;
            font-size: 40px;
            color: #333;
        }

        /* Оборудование */
        .equipment-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .equipment-item {
            text-align: center;
            padding: 25px;
            border: 1px solid #ddd;
            border-radius: 10px;
        }

        .equipment-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 5px;
        }

        .equipment-item h3 {
            margin: 15px 0;
            color: #2c3e50;
            font-size: 24px;
        }

        .equipment-item p {
            color: #666;
            font-size: 18px;
        }

        /* История */
        .history {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .history img {
            width: 50%;
            height: 450px;
            object-fit: cover;
            border-radius: 10px;
        }

        .history p {
            font-size: 18px;
            line-height: 1.6;
        }

        /* Гарантия */
        .guarantee-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 30px;
        }

        .guarantee-item {
            text-align: center;
        }

        .guarantee-item img {
            width: 120px;
            height: 120px;
            margin-bottom: 15px;
        }

        .guarantee-item h3 {
            font-size: 20px;
            margin-bottom: 10px;
        }

        .guarantee-item p {
            font-size: 16px;
        }

        /* Прайс */
        .price-grid {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }

        .price-item {
            width: 280px;
            height: 280px;
            border-radius: 50%;
            background: #f8f9fa;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 30px;
        }

        .price-item img {
            width: 100px;
            height: 100px;
            margin-bottom: 15px;
        }

        .price-item p {
            font-size: 18px;
        }

        /* Форма */
        .contact-form {
            max-width: 700px;
            margin: 0 auto;
        }

        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 15px;
            margin: 15px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }

        .contact-form textarea {
            height: 150px;
        }

        .contact-form button {
            padding: 15px 30px;
            background: #2c3e50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 18px;
        }

        /* Футер */
        .footer {
            background: #2c3e50;
            color: white;
            padding: 50px 20px;
            text-align: center;
        }

        .footer p {
            margin: 10px 0;
            font-size: 18px;
        }

        .social-links a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <!-- Шапка -->
    <header class="header">
        <div class="slider"></div>
    </header>

    <!-- Навигация -->
    <nav class="nav">
        <a href="#equipment">Оборудование</a>
        <a href="#history">О нас</a>
        <a href="#guarantee">Гарантия</a>
        <a href="#price">Прайс</a>
        <a href="#contact">Связаться</a>
    </nav>

    <!-- Оборудование -->
    <section id="equipment">
        <h2>Наше оборудование</h2>
        <div class="equipment-grid">
            <div class="equipment-item">
                <img src="https://a.allegroimg.com/s720/0304fc/5741888a4a8786dc57b61dbc3913/Oplatek-na-tort-KOPARKI-SPYCHACZE-DZWIGI-mocne-kol" alt="Экскаватор">
                <h3>Экскаватор</h3>
                <p>Мощность: 150 л.с.</p>
                <p>Применение: крупные земляные работы, строительство дорог.</p>
                <p>Цена: 1600 ₽/час</p>
            </div>
            <div class="equipment-item">
                <img src="https://ticargo-rent.ru/upload/iblock/345/gv1gbl1314qipro9g1qq4nzjd1c0wdle.png" alt="Бульдозер">
                <h3>Бульдозер</h3>
                <p>Мощность: около 108 кВт</p>
                <p>Масса: около 16 тонн</p>
                <p>Цена: 2000 ₽/час</p>
            </div>
            <div class="equipment-item">
                <img src="https://xn----7sbabaammi9c1ahkuj3a.xn--80adxhks/img/crane_Image_17.png" alt="Кран">
                <h3>Кран</h3>
                <p>Грузоподъемность: 25 т</p>
                <p>Цена: 2000 ₽/час</p>
            </div>
             <div class="equipment-item">
                <img src="https://artbudtrading.com.ua/image/cache/catalog/beton/abc-9-bez-fona-1500x1500.jpg" alt="Бетономешалка">
                <h3>Бетономешалка</h3>
                 <p>Объём: 300–500 литров</p>
                <p>Мощность: 1.5–3 кВт</p>
                <p>Цена: 3000 ₽/час</p>
            </div>
             <div class="equipment-item">
                <img src="https://asfalta-ukladka.ru/img/%D0%9A%D0%B0%D1%82%D0%BE%D0%BA%20(2).png" alt="Катки">
                <h3>Катки</h3>
                 <p>Масса: 8–10 тонн</p>
                <p>Мощность: 25–35 кВт</p>
                <p>Цена: 10000 ₽/8 часов</p>
            </div>
            <div class="equipment-item">
                <img src="https://avatars.mds.yandex.net/i?id=c7dfba7e0cd43ccfbda871243b591986_l-10638416-images-thumbs&n=13" alt="Самосвал">
                <h3>Самосвал</h3>
                 <p>Масса: 25 тонн</p>
                <p>Мощность: 300–350 л.с. (220–260 кВт).</p>
                <p>Цена: 2550 ₽/час</p>
            </div>
            <div class="equipment-item">
                <img src="https://sc04.alicdn.com/kf/H3c29947e8a11490faf9061910c432ad3N/Crawler-mounted-soil-boring-hydraulic-well-drilling-rig-machine.png" alt="Сваебойные машины">
                <h3>Сваебойные машины</h3>
                <p>Мощность: 260 кВт.</p>
                <p>Цена: 2000 ₽/час</p>
            </div>
        </div>
    </section>

    <!-- История -->
    <section id="history">
        <h2>Наша история</h2>
        <div class="history">
            <img src="https://ideogram.ai/assets/image/lossless/response/B4WkV8zvQl--w1gkkMyqVw" alt="Компания">
            <p>Мы работаем с 2010 года, предоставляя качественное строительное оборудование в аренду. Более 1000 довольных клиентов и 500+ единиц техники в нашем парке.</p>
        </div>
    </section>

    <!-- Гарантия -->
    <section id="guarantee">
        <h2>Наши гарантии</h2>
        <div class="guarantee-grid">
            <div class="guarantee-item">
                <img src="https://kmfin.ru/storage/images/mcWDruNwGzLHqG9eyG90.png" alt="Качество">
                <h3>Качество</h3>
                <p>Только проверенная техника</p>
            </div>
            <div class="guarantee-item">
                <img src="pngwing2.com.png" alt="Скорость">
                <h3>Скорость</h3>
                <p>Доставка в день заказа</p>
            </div>
            <div class="guarantee-item">
                <img src="pngwing3.com.png" alt="Поддержка">
                <h3>Поддержка</h3>
                <p>24/7 сервис</p>
            </div>
            <div class="guarantee-item">
                <img src="https://avatars.mds.yandex.net/i?id=cfe44647dab73facfc354a6f2963c932_sr-4414558-images-thumbs&n=13" alt="Цена">
                <h3>Цена</h3>
                <p>Лучшие условия</p>
            </div>
        </div>
    </section>

    <!-- Прайс -->
    <section id="price">
        <h2>Специальные предложения</h2>
        <div class="price-grid">
            <div class="price-item">
                <img src="https://iheschool.com/wp-content/uploads/2024/03/Excavator.png" alt="Акция">
                <p>Аренда на неделю<br>Скидка 20%</p>
            </div>
            <div class="price-item">
                <img src="pngwing.com.png" alt="Акция">
                <p>2+1 бесплатно<br>На выходные</p>
            </div>
            <div class="price-item">
                <img src="https://avatars.mds.yandex.net/get-altay/7730813/2a0000018469a30e5318d56ef55aee2f1f3e/XXL_height" alt="Акция">
                <p>Комплексная аренда<br>Скидка 15%</p>
            </div>
        </div>
    </section>

    <!-- Форма -->
    <section id="contact">
        <h2>Свяжитесь с нами</h2>
        <form action="https://api.web3forms.com/submit" method="POST" style="max-width: 500px; margin: 0 auto; padding: 30px; background-color: #f8f9fa; border-radius: 10px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
            <input type="hidden" name="access_key" value="34aad382-8a3f-4940-b92b-8c0e9f4fc7b5">
            <div style="margin-bottom: 20px;">
                <label for="name" style="display: block; margin-bottom: 8px; font-weight: 500; color: #333;">Name</label>
                <input type="text" name="name" id="name" required style="width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 6px; font-size: 16px; box-sizing: border-box; transition: border-color 0.3s;">
            </div>
            <div style="margin-bottom: 20px;">
                <label for="email" style="display: block; margin-bottom: 8px; font-weight: 500; color: #333;">Email</label>
                <input type="email" name="email" id="email" required style="width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 6px; font-size: 16px; box-sizing: border-box; transition: border-color 0.3s;">
            </div>
            <div style="margin-bottom: 30px;">
                <label for="message" style="display: block; margin-bottom: 8px; font-weight: 500; color: #333;">Message</label>
                <textarea name="message" id="message" required style="width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 6px; min-height: 120px; font-size: 16px; box-sizing: border-box; transition: border-color 0.3s; resize: vertical;"></textarea>
            </div>
            <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
            <button type="submit" style="background-color: #444444; color: white; border: none; padding: 14px 24px; font-size: 16px; font-weight: 600; border-radius: 6px; cursor: pointer; transition: background-color 0.3s; width: 100%;">Submit Form</button>
        </form>
    </section>

    <!-- Футер -->
    <footer class="footer">
        <p>© 2025 Аренда строительного оборудования</p>
        <p>+7 (999) 123-45-67 | info@rentconstruction.ru</p>
        <div class="social-links">
            <a href="#">VK</a>
            <a href="#">Telegram</a>
            <a href="#">WhatsApp</a>
            <a href="#">Instagram</a>
        </div>
    </footer>

    <script>
        document.querySelectorAll('.nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
