<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>UFC 343 - Мобильная версия</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; font-family:'Inter', sans-serif; }
    body { background-color:#111; color:#fff; line-height:1.5; padding:10px; }

    header { 
      text-align:center; 
      padding:15px; 
      background-color:#1a1a1a; 
      border-bottom:2px solid #e60000; 
      position:relative;
    }

    header .logo { 
      font-size:22px; 
      font-weight:700; 
      color:#e60000; 
    }

    /* КНОПКА ССЫЛКА РЯДОМ С UFC 343 */
    .link-btn{
      position:absolute;
      right:15px;
      top:50%;
      transform:translateY(-50%);
      background:#e60000;
      color:#fff;
      text-decoration:none;
      padding:5px 12px;
      border-radius:15px;
      font-size:13px;
      font-weight:600;
    }

    .event-header { margin:20px 0; text-align:center; }
    .event-header h1 { font-size:20px; margin-bottom:5px; }
    .event-header p { font-size:14px; color:#ccc; }

    /* Измененный fight-card для лучшего контроля содержимого */
    .fight-card {
      background-color:#1a1a1a;
      border:2px solid #e60000;
      border-radius:12px;
      padding:15px;
      margin-bottom:20px;
      display:flex;
      flex-direction:column; /* Устанавливаем вертикальный поток по умолчанию */
      align-items:center;
    }

    /* Новый контейнер для ряда бойцов и статуса */
    .fight-row {
      display:flex;
      justify-content:space-around;
      align-items:center;
      width:100%;
      margin-bottom:10px; /* Отступ между бойцами и весовой категорией */
    }

    .fighter {
      display:flex;
      flex-direction:column;
      align-items:center;
      text-align:center;
      position:relative; /* Важно для позиционирования галочки */
    }

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
    
    /* Новый стиль для зеленой рамки победителя */
    .winner-frame .photo {
      border:5px solid #34a853; /* Зеленая рамка */
    }

    .name { font-weight:600; font-size:16px; }

    .vs {
      font-size:24px;
      font-weight:700;
      color:#e60000;
      margin:0 10px;
      display:flex;
      flex-direction:column;
      align-items:center;
    }

    /* Новый стиль для текста результата */
    .result-text {
      font-size:13px;
      font-weight:600;
      color:#34a853;
      white-space:nowrap;
      order: -1; /* Помещает текст над VS */
      margin-bottom: 5px;
    }

    /* Новый стиль для галочки */
    .winner-icon {
      width:25px;
      height:25px;
      position:absolute;
      bottom: 5px; /* Сдвигаем вниз от имени бойца */
      z-index: 10;
    }
    
    /* Позиция галочки для левого бойца (в классе fighter) */
    .fight-row > .fighter:first-child .winner-icon {
        left: 70px; 
        right: auto;
    }
    
    /* Позиция галочки для правого бойца (в классе fighter) */
    .fight-row > .fighter:last-child .winner-icon {
        left: auto;
        right: 70px;
    }

    .weight {
      font-size:14px;
      color:#ccc;
      text-align:center;
      margin-top:5px;
      width:100%;
    }

    /* Старые стили с абсолютным позиционированием удалены */

    footer { 
      text-align:center; 
      padding:15px; 
      background-color:#1a1a1a; 
      border-top:2px solid #e60000; 
      color:#ccc; 
      font-size:12px; 
    }

    @media screen and (max-width:400px){
      .photo {
        width:80px;
        height:80px;
      }
      .name { font-size:14px; }
      .vs { font-size:20px; margin:0 5px; }
      .result-text { font-size:12px; }
      .weight { font-size:12px; }
      
      .winner-icon {
          width: 20px;
          height: 20px;
          bottom: 5px; 
      }
      
      .fight-row > .fighter:first-child .winner-icon {
          left: 60px;
      }
      
      .fight-row > .fighter:last-child .winner-icon {
          right: 60px;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">UFC 343</div>
  <a class="link-btn" href="https://AlishkaNepo.github.io/UFC-S/" target="_blank">UFC 344</a>
</header>

<div class="event-header">
  <h1>Главный кард — 6 Февраля 2025</h1>
  <p>Место проведения: Москва, Россия</p>
</div>

<div class="fight-card">
  <div class="fight-row">
    <div class="fighter winner-frame">
      <div class="photo">
        <img src="ali.jpg" alt="Али">
      </div>
      <div class="name">Али</div>
      <img src="galochka.png" class="winner-icon" alt="Победитель">
    </div>

    <div class="vs">
      <div class="result-text">Судейское Решение Р5 05:00</div>
      VS
    </div>

    <div class="fighter">
      <div class="photo">
        <img src="beka.jpg" alt="Бексултан">
      </div>
      <div class="name">Бексултан</div>
    </div>
  </div>
  <div class="weight">Полулёгкий вес • Главный бой</div>
</div>

<div class="fight-card">
  <div class="fight-row">
    <div class="fighter winner-frame">
      <div class="photo">
        <img src="roma.jpg" alt="Роман">
      </div>
      <div class="name">Роман</div>
      <img src="galka.png" class="winner-icon" alt="Победитель">
    </div>

    <div class="vs">
      <div class="result-text">Добровольная сдача Р2 02:34</div>
      VS
    </div>

    <div class="fighter">
      <div class="photo">
        <img src="alikh.jpg" alt="Алихан">
      </div>
      <div class="name">Алихан</div>
    </div>
  </div>
  <div class="weight">Легкий вес • Со-главный бой</div>
</div>

<footer>
  © 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
