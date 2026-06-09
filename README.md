<!DOCTYPE html>
<html lang="mn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Одод ✨</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: Georgia, serif;
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            color: #fff;
            min-height: 100vh;
            overflow-x: hidden;
        }
        .stars { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 0; }
        .star { position: absolute; background: white; border-radius: 50%; animation: twinkle 3s infinite; }
        @keyframes twinkle {
            0%, 100% { opacity: 0; transform: scale(0.5); }
            50% { opacity: 1; transform: scale(1); }
        }
        header { position: relative; z-index: 1; text-align: center; padding: 80px 20px; }
        header h1 {
            font-size: 4em;
            background: linear-gradient(45deg, #ffecd2, #fcb69f, #ff9a9e);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 20px;
            animation: glow 2s ease-in-out infinite alternate;
        }
        @keyframes glow {
            from { filter: drop-shadow(0 0 10px rgba(252, 182, 159, 0.5)); }
            to { filter: drop-shadow(0 0 30px rgba(255, 154, 158, 0.8)); }
        }
        header p { font-size: 1.3em; opacity: 0.9; font-style: italic; }
        nav { position: relative; z-index: 1; display: flex; justify-content: center; gap: 30px; padding: 20px; flex-wrap: wrap; }
        nav a { color: #fff; text-decoration: none; padding: 10px 25px; border: 2px solid rgba(255, 255, 255, 0.3); border-radius: 30px; transition: all 0.3s; }
        nav a:hover { background: rgba(255, 255, 255, 0.1); border-color: #fcb69f; transform: translateY(-3px); }
        main { position: relative; z-index: 1; max-width: 1200px; margin: 0 auto; padding: 40px 20px; }
        .section-title { text-align: center; font-size: 2.5em; margin: 60px 0 40px; color: #ffecd2; }
        .cards { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 30px; margin-top: 40px; }
        .card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 30px;
            transition: all 0.3s;
            cursor: pointer;
        }
        .card:hover { transform: translateY(-10px); background: rgba(255, 255, 255, 0.1); box-shadow: 0 20px 40px rgba(252, 182, 159, 0.2); }
        .card .icon { font-size: 3em; margin-bottom: 15px; }
        .card h3 { font-size: 1.5em; margin-bottom: 10px; color: #fcb69f; }
        .card p { opacity: 0.8; line-height: 1.6; }
        .quote-section { margin: 80px 0; text-align: center; padding: 60px 20px; background: rgba(255, 255, 255, 0.03); border-radius: 30px; border: 1px solid rgba(255, 255, 255, 0.1); }
        .quote { font-size: 1.8em; font-style: italic; color: #ffecd2; margin-bottom: 20px; }
        .quote-author { opacity: 0.7; }
        .counter-section { text-align: center; margin: 60px 0; }
        .counter { display: flex; justify-content: center; gap: 50px; flex-wrap: wrap; margin-top: 30px; }
        .counter-item { text-align: center; }
        .counter-number { font-size: 3em; font-weight: bold; color: #fcb69f; display: block; }
        .counter-label { opacity: 0.7; margin-top: 5px; }
        footer { position: relative; z-index: 1; text-align: center; padding: 40px 20px; border-top: 1px solid rgba(255, 255, 255, 0.1); margin-top: 80px; }
        .social { display: flex; justify-content: center; gap: 20px; margin-top: 20px; }
        .social a {
            display: inline-block; width: 50px; height: 50px; line-height: 50px;
            border-radius: 50%; background: rgba(255, 255, 255, 0.1);
            color: white; text-decoration: none; font-size: 1.5em; transition: all 0.3s;
        }
        .social a:hover { background: #fcb69f; transform: scale(1.1) rotate(360deg); }
        @media (max-width: 768px) {
            header h1 { font-size: 2.5em; }
            .section-title { font-size: 1.8em; }
        }
    </style>
</head>
<body>
    <div class="stars" id="stars"></div>
    <header>
        <h1>✨ Одод ✨</h1>
        <p>"Бид бүгд тэнгэрт гэрэлтэх одод мөн"</p>
    </header>
    <nav>
        <a href="#home">Нүүр</a>
        <a href="#about">Тухай</a>
        <a href="#gallery">Галерей</a>
        <a href="#contact">Холбоо барих</a>
    </nav>
    <main>
        <h2 class="section-title" id="about">Юу вэ?</h2>
        <div class="cards">
            <div class="card"><div class="icon">🌟</div><h3>Гэрэл</h3><p>Харанхуйд гэрэлтэх од бүр бидний найдвар, мөрөөдлийн бэлгэ тэмдэг юм.</p></div>
            <div class="card"><div class="icon">🌙</div><h3>Шөнө</h3><p>Шөнө тэнгэр хамгийн гоё байдаг. Одод, сар мандан баялагийг бүрдүүлнэ.</p></div>
            <div class="card"><div class="icon">🚀</div><h3>Мөрөөдөл</h3><p>Одод хүртэл хүсэл мөрөөдлөө сунга. Бүх зүйл боломжтой!</p></div>
            <div class="card"><div class="icon">💫</div><h3>Ид шид</h3><p>Амьдрал бүр ид шидийн дүүрэн. Зүгээр л нүдээ нээ.</p></div>
        </div>
        <div class="quote-section" id="gallery">
            <p class="quote">"Бид бүгд тоосонцор, гэхдээ бид одод мөн."</p>
            <p class="quote-author">— Карл Саган</p>
        </div>
        <div class="counter-section">
            <h2 class="section-title">Тоон үзүүлэлт</h2>
            <div class="counter">
                <div class="counter-item"><span class="counter-number" data-target="1000">0</span><span class="counter-label">Од</span></div>
                <div class="counter-item"><span class="counter-number" data-target="365">0</span><span class="counter-label">Өдөр</span></div>
                <div class="counter-item"><span class="counter-number" data-target="24">0</span><span class="counter-label">Цаг</span></div>
                <div class="counter-item"><span class="counter-number" data-target="∞">0</span><span class="counter-label">Мөрөөдөл</span></div>
            </div>
        </div>
    </main>
    <footer id="contact">
        <h2>Холбоо барих</h2>
        <p style="margin-top: 10px; opacity: 0.7;">Бидэнтэй холбогдоорой</p>
        <div class="social">
            <a href="#">📘</a><a href="#">📷</a><a href="#">🐦</a><a href="#">✉️</a>
        </div>
        <p style="margin-top: 30px; opacity: 0.5;">© 2025 Одод Вэбсайт. Бүх эрх хуулиар хамгаалагдсан.</p>
    </footer>
    <script>
        const starsContainer = document.getElementById('stars');
        for (let i = 0; i < 150; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            const size = Math.random() * 3 + 1;
            star.style.width = size + 'px';
            star.style.height = size + 'px';
            star.style.top = Math.random() * 100 + '%';
            star.style.left = Math.random() * 100 + '%';
            star.style.animationDelay = Math.random() * 3 + 's';
            star.style.animationDuration = (Math.random() * 2 + 2) + 's';
            starsContainer.appendChild(star);
        }
        const counters = document.querySelectorAll('.counter-number');
        const animateCounter = (counter) => {
            const target = counter.getAttribute('data-target');
            if (target === '∞') { counter.textContent = '∞'; return; }
            const targetNum = parseInt(target);
            let current = 0;
            const increment = targetNum / 60;
            const timer = setInterval(() => {
                current += increment;
                if (current >= targetNum) { counter.textContent = targetNum + '+'; clearInterval(timer); }
                else { counter.textContent = Math.floor(current); }
            }, 30);
        };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => { if (entry.isIntersecting) { animateCounter(entry.target); observer.unobserve(entry.target); } });
        });
        counters.forEach(counter => observer.observe(counter));
    </script>
</body>
</html>
