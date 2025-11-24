<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>UFC 344 - Мобильная версия</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; font-family:'Inter', sans-serif; }
    body { background-color:#111; color:#fff; line-height:1.5; padding:10px; }

    header { text-align:center; padding:15px; background-color:#1a1a1a; border-bottom:2px solid #e60000; }
    header .logo { font-size:22px; font-weight:700; color:#e60000; }

    .event-header { margin:20px 0; text-align:center; }
    .event-header h1 { font-size:20px; margin-bottom:5px; }
    .event-header p { font-size:14px; color:#ccc; }

    .fight-card {
      background-color:#1a1a1a;
      border:2px solid #e60000;
      border-radius:12px;
      padding:15px;
      margin-bottom:20px;
      display:flex;
      justify-content:space-around;
      align-items:center;
      flex-wrap:nowrap;
    }

    .fighter {
      display:flex;
      flex-direction:column;
      align-items:center;
      text-align:center;
    }

    /* КРУГЛАЯ РАМКА ДЛЯ ФОТО */
    .photo {
      width:100px;
      height:100px;
      border-radius:50%;
      border:3px solid #e60000;
      overflow:hidden;
      margin-bottom:5px;
    }

    .photo img {
      width:100%;
      height:100%;
      object-fit:cover;
      display:block;
    }

    .name { font-weight:600; font-size:16px; }

    .vs {
      font-size:24px;
      font-weight:700;
      color:#e60000;
      margin:0 10px;
    }

    .weight {
      font-size:14px;
      color:#ccc;
      text-align:center;
      margin-top:5px;
      width:100%;
    }
    #rama{
       width:100px;
      height:100px;
      border-radius:50%;
      border:5px solid #34a853;
      overflow:hidden;
      position:absolute;
      left:26px;
      top:187px;

    }
    #rama2{
       width:100px;
      height:100px;
      border-radius:50%;
      border:5px solid #34a853;
      overflow:hidden;
      position:absolute;
      left:26px;
      top:369.5px;

    }
    #galochka{
      width:25px;
      height:25px;
      position:absolute;
      left:105px;
      top:270px;
    }
    #tekst{
      position:absolute;
      top:600px;
      left:1200px;
      color:#34a853;
    }
    #galka{
      width:25px;
      height:25px;
      position:absolute;
      left:105px;
      top:452.5px;
    }
    #tkst{
      position:absolute;
      top:472.5px;
      left:370px;
      color:#34a853;
    }
    #ssilka{
      position:absolute;
      left:1380px;
      top:32px;
      z-index: 2;
      color:white;
    
    }
    #blok{
      position:absolute;
      width:125px;
      height:45px;
      background-color:#e60000;
      left:1350px;
      top:20px;
      border-radius:15px;
      z-index:1 ;
    }
    
  

    footer { text-align:center; padding:15px; background-color:#1a1a1a; border-top:2px solid #e60000; color:#ccc; font-size:12px; }

    /* --- Адаптация под маленькие экраны --- */
    @media screen and (max-width:400px){
      .photo {
        width:80px;
        height:80px;
      }
      .name { font-size:14px; }
      .vs { font-size:20px; margin:0 5px; }
      .weight { font-size:12px; }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">UFC 343</div>
</header>

<div class="event-header">
  <h1>Главный кард — 6 Февраля 2025</h1>
  <p>Место проведения: Москва, Россия</p>
</div>
<div id="rama"></div>
<div id="rama2"></div>
<img src="galochka.png" id="galochka">
<h4 id="tekst">Судейское  Решение  Р5  05:00</h4>
<img src="galka.png" id="galka">
<h4 id="tkst">Добровольная сдача  Р2  02:34</h4>

<!-- Первый бой -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo">
      <img src="ali.jpg" alt="Али">
    </div>
    <div class="name">Али</div>
  </div>
  <a href="https://AlishkaNepo.github.io/UFC-S/" id="ssilka">UFC 344</a>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo">
      <img src="beka.jpg" alt="Бексултан">
    </div>
    <div class="name">Бексултан</div>
  </div>

  <div class="weight">Полулёгкий вес • Главный бой</div>
</div>
<div id="blok"></div>

<!-- Второй бой -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo">
      <img src="roma.jpg" alt="Роман">
    </div>
    <div class="name">Роман</div>
  </div>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo">
      <img src="alikh.jpg" alt="Алихан">
    </div>
    <div class="name">Алихан</div>
  </div>

  <div class="weight">Легкий  вес • Со-главный бой</div>
</div>

<footer>
  © 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
