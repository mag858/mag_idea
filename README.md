
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Glushnev Mikhail Alekseevich">
    <meta name="description" content="MAG Industries – предлагайте свои идеи по автомобилям и устройствам">
    <meta name="keywords" content="MAG industries, идеи, предложения, стартап, автомобили, технологии, будущее">
    <title>MAG Industries | Ваши идеи</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Roboto:wght@300;400&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #F3A000;
            --red: #FF0000;
            --bg: #CCE1FE;
            --text: #222;
            --shadow: 0 4px 15px rgba(0,0,0,0.1);
            --input-bg: #ffffff;
            --border: #ddd;
        }
        
        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
            animation: fadeIn 1.5s ease-out;
        }
        
        .back-btn {
            position: fixed;
            top: 15px;
            left: 15px;
            padding: 10px 18px;
            background: rgba(255,255,255,0.9);
            color: var(--text);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            border-radius: 30px;
            box-shadow: var(--shadow);
            transition: all 0.3s ease;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }
        
        .back-btn:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }
        
        .hero {
            text-align: center;
            padding: 80px 20px 40px;
        }
        
        .logo {
            max-width: 320px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            margin-bottom: 20px;
            transition: transform 0.5s ease;
            animation: slideUp 1s ease-out;
        }
        
        .logo:hover {
            transform: scale(1.05);
        }
        
        h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 3rem;
            color: var(--primary);
            margin: 0 0 10px 0;
            animation: slideUp 1.2s ease-out;
        }
        
        .subtitle {
            font-size: 1.6rem;
            color: #333;
            font-weight: 500;
            margin-bottom: 50px;
            animation: slideUp 1.4s ease-out;
        }
        
        .ideas-section {
            max-width: 800px;
            margin: 60px auto;
            padding: 40px;
            background: rgba(255,255,255,0.9);
            border-radius: 20px;
            box-shadow: var(--shadow);
            text-align: center;
            animation: fadeInUp 1.5s ease-out;
        }
        
        .ideas-section h3 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.2rem;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .ideas-section p {
            font-size: 1.1rem;
            margin-bottom: 40px;
            color: #444;
        }
        
        form {
            text-align: left;
        }
        
        input[type="text"],
        input[type="email"],
        input[type="number"],
        textarea {
            width: 100%;
            padding: 14px 16px;
            margin-bottom: 20px;
            border: 2px solid var(--border);
            border-radius: 12px;
            font-size: 1rem;
            background: var(--input-bg);
            transition: all 0.3s ease;
            opacity: 0;
            animation: fadeInUp 1s ease-out forwards;
        }
        
        input[type="text"]:focus,
        input[type="email"]:focus,
        input[type="number"]:focus,
        textarea:focus {
            border-color: var(--primary);
            outline: none;
            box-shadow: 0 0 15px rgba(243,160,0,0.3);
            transform: scale(1.02);
        }
        
        textarea {
            min-height: 180px;
            resize: vertical;
        }
        
        input:nth-of-type(1) { animation-delay: 0.2s; }
        input:nth-of-type(2) { animation-delay: 0.4s; }
        input:nth-of-type(3) { animation-delay: 0.6s; }
        textarea { animation-delay: 0.8s; }
        
        input[type="submit"] {
            display: block;
            width: 200px;
            margin: 30px auto 0;
            padding: 14px;
            background: var(--primary);
            color: white;
            font-size: 1.2rem;
            font-weight: 600;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.4s ease;
            box-shadow: var(--shadow);
            animation: fadeInUp 1.2s ease-out;
        }
        
        input[type="submit"]:hover {
            background: var(--red);
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 10px 25px rgba(255,0,0,0.3);
        }
        
        .privacy {
            margin-top: 40px;
            font-size: 0.9rem;
            color: #666;
            animation: fadeIn 2s ease-out;
        }
        
        footer {
            text-align: center;
            padding: 40px;
            background: rgba(255,255,255,0.9);
            font-size: 0.9rem;
            color: #666;
            margin-top: 80px;
        }
        
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes slideUp { from { opacity: 0; transform: translateY(50px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
        
        @media (max-width: 768px) {
            .back-btn { top: 10px; left: 10px; padding: 8px 14px; font-size: 0.9rem; }
            .hero { padding-top: 70px; }
            h1 { font-size: 2.4rem; }
            .subtitle { font-size: 1.4rem; }
            .ideas-section { margin: 40px 20px; padding: 30px; }
            .ideas-section h3 { font-size: 2rem; }
            input[type="submit"] { width: 100%; max-width: 300px; }
            .logo { max-width: 280px; }
        }
    </style>
</head>
<body>

    <a href="https://mag858.github.io/MAG-industries/" class="back-btn">← На главную</a>

    <section class="hero">
        <img src="sait/logo_2.jpeg" alt="Логотип MAG Industries" class="logo">
        <h1>future - right now</h1>
        <div class="subtitle">(будущее - прямо сейчас)</div>
    </section>

    <section class="ideas-section">
        <h3>Ваши идеи</h3>
        <p>Здесь вы можете предлагать свои идеи по разработке часов или других устройств. Мы будем рады увидеть любые ваши идеи и предложения — даже если они кажутся сложными или невозможными.</p>
        
        <form action="https://api.web3forms.com/submit" method="POST">
            <input type="hidden" name="access_key" value="cabd165b-582a-434a-8aec-d05523b4c7f7">
            
            <input type="text" name="имя" placeholder="Ваше Имя" required>
            
            <input type="number" name="возраст" placeholder="Сколько вам лет" min="1" max="120">
            
            <input type="email" name="email" placeholder="Ваш email" required>
            
            <textarea name="идеи и предложения" placeholder="Напишите сюда ваши идеи и пожелания..." required></textarea>
            
            <input type="submit" value="Отправить">
        </form>
        
        <div class="privacy">
            Все ваши данные нужны исключительно для анализа нашей аудитории и не передаются третьим лицам.
        </div>
    </section>

    <footer>
        обновление 3.1 &emsp; январь 2026 г.
    </footer>

</body>
</html>
