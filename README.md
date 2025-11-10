<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>ALMAU — ONE UNIVERSITY, ONE COMMUNITY</title>
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <style>
        :root{
            --brand:#1746a0;
            --bg:#f7f9fc;
            --card:#fff;
            --muted:#6b7280;
        }
        html,body{height:100%;margin:0;font-family:'Segoe UI',Arial,sans-serif;background:var(--bg);color:#222}
        header{background:var(--brand);color:#fff;padding:20px 12px 12px;text-align:center;box-shadow:0 2px 8px rgba(23,70,160,0.07)}
        header h1{margin:6px 0 0;font-size:1.5rem;letter-spacing:1px}
        header .slogan{color:#cfe0ff;margin-top:6px;font-weight:600}
        nav{margin:14px auto 0;display:flex;flex-wrap:wrap;justify-content:center;gap:8px;padding:8px;max-width:1100px}
        .tab-btn{background:var(--card);color:var(--brand);border:1px solid var(--brand);border-radius:20px;padding:8px 14px;cursor:pointer;transition:200ms;font-size:0.95rem}
        .tab-btn:hover,.tab-btn.active{background:var(--brand);color:#fff}
        main{max-width:980px;margin:22px auto;padding:28px;border-radius:14px;background:var(--card);box-shadow:0 6px 24px rgba(23,70,160,0.08)}
        h2{color:var(--brand);margin:0 0 8px;font-size:1.4rem;display:flex;align-items:center;gap:10px}
        .info{position:relative;display:inline-flex;align-items:center;justify-content:center;width:20px;height:20px;border-radius:50%;background:#e8f0ff;color:var(--brand);font-weight:700;font-size:0.85rem;cursor:default}
        .tooltip{position:absolute;left:28px;top:-6px;width:240px;background:var(--brand);color:#fff;padding:8px;border-radius:8px;box-shadow:0 8px 22px rgba(23,70,160,0.14);opacity:0;visibility:hidden;transform:translateY(6px);transition:200ms}
        .info:hover .tooltip,.info:focus .tooltip{opacity:1;visibility:visible;transform:translateY(0)}
        h3{margin-top:14px}
        ul{margin-top:8px;margin-bottom:18px}
        .meta{margin-top:6px;font-size:0.95rem}
        .muted{color:var(--muted);font-size:0.94rem}
        footer{text-align:center;padding:16px 0;color:var(--brand);background:#f0f4fa;border-radius:0 0 14px 14px;margin-top:18px}
        a{color:var(--brand)}
        @media(max-width:640px){.tooltip{left:0;top:28px;width:calc(100vw - 60px)}nav{gap:6px;padding:6px}main{margin:12px;padding:18px}}
    </style>
</head>
<body>
    <header>
        <h1>AlmaU: школы</h1>
        <div class="slogan">ALMAU — ONE UNIVERSITY, ONE COMMUNITY.</div>
        <nav aria-label="Школы AlmaU">
            <button class="tab-btn" onclick="showTab('institute')">Институт предпринимательства</button>
            <button class="tab-btn" onclick="showTab('hsb')">Высшая школа бизнеса</button>
            <button class="tab-btn" onclick="showTab('mgmt')">Школа менеджмента и туризма</button>
            <button class="tab-btn" onclick="showTab('digital')">School of Digital Technologies & Economics</button>
            <button class="tab-btn" onclick="showTab('humanities')">Transformative Humanities & Education</button>
            <button class="tab-btn" onclick="showTab('media')">Школа медиа и кино</button>
            <button class="tab-btn" onclick="showTab('contacts')">Контакты</button>
        </nav>
    </header>

    <main>
        <section id="institute" class="tab-section" style="display:none">
            <h2>Институт предпринимательства
                <span class="info" tabindex="0">i
                    <span class="tooltip">Поддержка стартапов, акселераторы и практическое развитие предпринимательских навыков.</span>
                </span>
            </h2>
            <div class="meta"><strong>Директор:</strong> Медетов Данияр</div>
            <p class="muted">Программы института направлены на практическое развитие предпринимательских компетенций.</p>
        </section>

        <section id="hsb" class="tab-section" style="display:none">
            <h2>Высшая школа бизнеса
                <span class="info" tabindex="0">i
                <span class="tooltip">Карьера и лидерство: кейсы, менторство и профессиональное развитие.</span>
                </span>
            </h2>
            <div class="meta"><strong>Руководитель:</strong> Южанинова-Караденизли Ксения Сергеевна</div>
            <p class="meta"><strong>Часы приёма студентов и абитуриентов:</strong> в любое время по записи</p>
            <p class="meta"><strong>Email:</strong> <a href="mailto:k.yuzhaninova@almau.edu.kz">k.yuzhaninova@almau.edu.kz</a></p>
            <p class="meta"><strong>Кабинет:</strong> идет ремонт, 4 этаж</p>
        </section>

        <section id="mgmt" class="tab-section" style="display:none">
            <h2>Школа менеджмента и туризма
                <span class="info" tabindex="0">i
                    <span class="tooltip">Менеджмент и гостеприимство — практика, маркетинг и сервисное мышление.</span>
                </span>
            </h2>
            <div class="meta"><strong>Руководитель:</strong> Ауезханулы Азамат</div>
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

        <section id="digital" class="tab-section" style="display:none">
            <h2>School of Digital Technologies & Economics
                <span class="info" tabindex="0">i
                    <span class="tooltip">IT и экономика: подготовка специалистов для цифровой трансформации.</span>
                </span>
            </h2>
            <div class="meta"><strong>Руководитель:</strong> Комекбаев Арман Ерманатович</div>
            <h3>Специальности / Specialties:</h3>
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

        <section id="humanities" class="tab-section" style="display:none">
            <h2>School of Transformative Humanities & Education
                <span class="info" tabindex="0">i
                    <span class="tooltip">Гуманитарные и образовательные практики, ориентированные на трансформацию общества.</span>
                </span>
            </h2>
            <div class="meta"><strong>Руководитель:</strong> Сапаргалиева Айжан Жанисовна</div>
            <p class="muted">Программы в области образования и гуманитарных наук публикуются по мере обновления.</p>
        </section>

        <section id="media" class="tab-section" style="display:none">
            <h2>Школа медиа и кино
                <span class="info" tabindex="0">i
                    <span class="tooltip">Творчество и индустрия: медиа, кино и практические проекты.</span>
                </span>
            </h2>
            <div class="meta"><strong>Руководитель:</strong> Секеева Анара Маратовна</div>
            <h3>Специальности:</h3>
            <ul>
                <li>6B03201 – Связь с общественностью</li>
                <li>6B03203 – New Media</li>
                <li>6B03204 – Content, Marketing and Data Analysis</li>
                <li>6В02103 – Digital Filmmaking</li>
                <li>6В02104 – Acting for Film</li>
            </ul>
        </section>

        <section id="contacts" class="tab-section" style="display:none">
            <h2>Контакты AlmaU</h2>
            <p><strong>Адрес:</strong> г. Алматы, Республика Казахстан, ул.Розыбакиева 227</p>
            <p><strong>Email:</strong> <a href="mailto:admission@almau.edu.kz">admission@almau.edu.kz</a></p>
            <p><strong>Соцсети:</strong> <a href="https://t.me/almau_edu" target="_blank" rel="noopener noreferrer">@almau_edu</a></p>
            <p><strong>Номер для консультаций:</strong> <a href="tel:+77750061606">+7 775 006 1606</a></p>
            <hr>
        </section>
    </main>

    <footer>&copy; 2025 AlmaU</footer>

    <script>
        function showTab(tabId){
            document.querySelectorAll('.tab-section').forEach(s=>s.style.display='none');
            const t=document.getElementById(tabId);
            if(t) t.style.display='block';
            document.querySelectorAll('.tab-btn').forEach(b=>b.classList.remove('active'));
            document.querySelectorAll('nav .tab-btn').forEach(b=>{
                if(b.getAttribute('onclick') && b.getAttribute('onclick').includes(tabId)) b.classList.add('active');
            });
            if(t){ setTimeout(()=>{ const h=t.querySelector('h2'); if(h) h.scrollIntoView({behavior:'smooth',block:'start'}); },80); }
        }
        document.addEventListener('DOMContentLoaded',()=>showTab('institute'));
    </script>
</body>
</html>
