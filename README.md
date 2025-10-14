<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Чат-бот про школы и администрацию ALMAU!</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background: #f7f9fc;
            margin: 0;
            color: #222;
        }
        header {
            background: #1746a0;
            color: #fff;
            padding: 24px 0 10px 0;
            text-align: center;
            box-shadow: 0 2px 8px rgba(23,70,160,0.07);
        }
        nav {
            margin-top: 16px;
        }
        .tab-btn {
            background: #fff;
            color: #1746a0;
            border: 1px solid #1746a0;
            border-radius: 20px;
            padding: 8px 18px;
            margin: 4px 2px;
            cursor: pointer;
            font-size: 1em;
            transition: background 0.2s, color 0.2s;
        }
        .tab-btn:hover, .tab-btn.active {
            background: #1746a0;
            color: #fff;
        }
        main {
            max-width: 800px;
            margin: 32px auto 0 auto;
            background: #fff;
            border-radius: 18px;
            box-shadow: 0 4px 24px rgba(23,70,160,0.08);
            padding: 32px 24px 24px 24px;
        }
        h2 {
            color: #1746a0;
            margin-top: 0;
            margin-bottom: 10px;
            font-size: 2em;
            font-weight: 700;
            letter-spacing: 1px;
        }
        h3 {
            margin-top: 18px;
            color: #222;
        }
        ul {
            margin-top: 8px;
            margin-bottom: 18px;
        }
        section.tab-section {
            animation: fadeIn 0.4s;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px);}
            to { opacity: 1; transform: translateY(0);}
        }
        img {
            display: block;
            margin-bottom: 10px;
        }
        footer {
            text-align: center;
            padding: 18px 0 10px 0;
            color: #1746a0;
            background: #f0f4fa;
            font-size: 1em;
            margin-top: 32px;
            border-radius: 0 0 18px 18px;
        }
        a {
            color: #1746a0;
            text-decoration: underline;
        }
        hr {
            margin: 24px 0;
            border: none;
            border-top: 1px solid #e0e6f6;
        }
    </style>
</head>
<body>
    <header>
        <h1>AlmaU: школы</h1>
        <nav>
            <button class="tab-btn" onclick="showTab('school1')">Школа менеджмента</button>
            <button class="tab-btn" onclick="showTab('school2')">Школа экономики и финансов</button>
            <button class="tab-btn" onclick="showTab('school3')">Школа политики и права</button>
            <button class="tab-btn" onclick="showTab('school4')">School of Digital Technologies</button>
            <button class="tab-btn" onclick="showTab('school5')">Sharmanov School of Health Sciences</button>
            <button class="tab-btn" onclick="showTab('school6')">Школа медиа и кино</button>
            <button class="tab-btn" onclick="showTab('school7')">Школа предпринимательства и инноваций</button>
            <button class="tab-btn" onclick="showTab('school8')">Школа гостеприимства и туризма</button>
            <button class="tab-btn" onclick="showTab('school9')">School of Transformative Humanities</button>
            <button class="tab-btn" onclick="showTab('contacts')">Контакты</button>
        </nav>
    </header>
    <main>
        <section id="school1" class="tab-section">
            <h2>Школа менеджмента</h2>
            <img src="logo-manager.png" alt="Логотип школы менеджмента" style="max-width:120px;">
            <h3>Специальности:</h3>
            <ul>
                <li>6B04101 – Менеджмент</li>
                <li>6B11303 – Digital logistics</li>
                <li>6B04104 – Маркетинг</li>
                <li>6B04120 – Content, Marketing and Data Analysis</li>
                <li>6B11301 – Логистика</li>
                <li>6B04124 – Digital marketing</li>
            </ul>
        </section>
        <section id="school2" class="tab-section" style="display:none;">
            <h2>Школа экономики и финансов</h2>
            <img src="logo-econ.png" alt="Логотип школы экономики и финансов" style="max-width:120px;">
            <h3>Специальности:</h3>
            <ul>
                <li>6B04190 – Бизнес-аналитика и экономика</li>
                <li>6В04106 – Учет и аудит</li>
                <li>6B04105 – Финансы</li>
                <li>6B04125 – FinTech and Artificial Intelligence</li>
            </ul>
        </section>
        <section id="school3" class="tab-section" style="display:none;">
            <h2>Школа политики и права</h2>
            <img src="logo-law.png" alt="Логотип школы политики и права" style="max-width:120px;">
            <h3>Специальности:</h3>
            <ul>
                <li>6B04201 – Юриспруденция (Бизнес-право)</li>
                <li>6В03088(1) – Международные отношения и экономика</li>
            </ul>
        </section>
        <section id="school4" class="tab-section" style="display:none;">
            <h2>School of Digital Technologies</h2>
            <img src="logo-digital.png" alt="Logo School of Digital Technologies" style="max-width:120px;">
            <h3>Specialties:</h3>
            <ul>
                <li>6B06101 – Информационные системы</li>
                <li>6B06103 – Software Engineering</li>
                <li>6B06104 – Data Science</li>
                <li>6B06105 – Product Management</li>
                <li>6B06088 – Content, Marketing, Data Analysis</li>
                <li>6B06108 – City Management and Data Analysis</li>
                <li>6B06106 – FinTech and Artificial Intelligence</li>
                <li>6B06107 – Travel Management and Data Analysis</li>
                <li>6B06109 – Software engineering and information protection</li>
            </ul>
        </section>
        <section id="school5" class="tab-section" style="display:none;">
            <h2>Sharmanov School of Health Sciences</h2>
            <img src="logo-health.png" alt="Logo Sharmanov School of Health Sciences" style="max-width:120px;">
            <h3>Специальности:</h3>
            <ul>
                <li>6B03104 – Психология</li>
            </ul>
        </section>
        <section id="school6" class="tab-section" style="display:none;">
            <h2>Школа медиа и кино</h2>
            <img src="logo-media.png" alt="Логотип школы медиа и кино" style="max-width:120px;">
            <h3>Специальности:</h3>
            <ul>
                <li>6B03201 – Связь с общественностью</li>
                <li>6B03203 – New Media</li>
                <li>6B03204 – Content, Marketing and Data Analysis</li>
                <li>6В02103 – Digital Filmmaking</li>
                <li>6В02104 – Acting for Film</li>
            </ul>
        </section>
        <section id="school7" class="tab-section" style="display:none;">
            <h2>Школа предпринимательства и инноваций</h2>
            <img src="logo-entrepreneur.png" alt="Логотип школы предпринимательства и инноваций" style="max-width:120px;">
            <p>Информация о специальностях появится позже.</p>
        </section>
        <section id="school8" class="tab-section" style="display:none;">
            <h2>Школа гостеприимства и туризма</h2>
            <img src="logo-hospitality.png" alt="Логотип школы гостеприимства и туризма" style="max-width:120px;">
            <h3>Специальности:</h3>
            <ul>
                <li>6B11101 – Ресторанное дело и гостиничный бизнес</li>
                <li>6B11188 – Tourism and Event Management</li>
            </ul>
        </section>
        <section id="school9" class="tab-section" style="display:none;">
            <h2>School of Transformative Humanities</h2>
            <img src="logo-humanities.png" alt="Logo School of Transformative Humanities" style="max-width:120px;">
            <p>Информация о специальностях появится позже.</p>
        </section>


<section id="school10" class="tab-section" style="display:none;">
            <h2>Высшая школа бизнеса</h2>
            <img src="logo-business.png" alt="Логотип высшей школы бизнеса" style="max-width:120px;">
            <p>Информация о специальностях появится позже.</p>
        </section>
        <section id="contacts" class="tab-section" style="display:none;">
            <h2>Контакты AlmaU</h2>
            <p><b>Адрес:</b> г. Алматы, Республика Казахстан, ул. Розыбакиева 227</p>
            <p><b>Email:</b> <a href="mailto:admission@almau.edu.kz">admission@almau.edu.kz</a></p>
            <p><b>Соцсети:</b> <a href="https://t.me/almau_edu" target="_blank">@almau_edu</a></p>
            <p><b>Номер для консультаций:</b> <a href="tel:+77750061606">+7 775 006 1606</a></p>
            <hr>
            <p><b>Я — чат-бот AlmaU в Telegram!</b><br>
            Помогаю узнать всё о школах, поступлении и жизни в университете.<br>
            Если возникнут вопросы — просто напишите в чат, и я с радостью помогу вам!</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 AlmaU</p>
    </footer>
    <script>
        function showTab(tabId) {
            const sections = document.querySelectorAll('.tab-section');
            const buttons = document.querySelectorAll('.tab-btn');
            sections.forEach(sec => sec.style.display = 'none');
            document.getElementById(tabId).style.display = 'block';
            buttons.forEach(btn => btn.classList.remove('active'));
            const navBtns = document.querySelectorAll('nav .tab-btn');
            navBtns.forEach(btn => {
                if (btn.getAttribute('onclick').includes(tabId)) {
                    btn.classList.add('active');
                }
            });
        }
        document.addEventListener('DOMContentLoaded', function() {
            showTab('school1');
        });
    </script>
</body>
</html>
