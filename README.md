<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>UFC 343 - Мобильная версия</title>
<style>
* { margin:0; padding:0; box-sizing:border-box; font-family:Arial, sans-serif; }
body { background:#111; color:#fff; line-height:1.5; padding:10px; }

/* HEADER */
.header-inner {
    display:flex;
    justify-content:space-between;
    align-items:center;
    margin-bottom:15px;
}

.header-inner h1 {
    font-size:22px;
    color:red;
}

.ufc-link {
    background:red;
    color:white;
    text-decoration:none;
    padding:6px 12px;
    border-radius:20px;
    font-size:14px;
    font-weight:600;
    transition:0.2s;
}

.ufc-link:hover { background:#ff3b3b; }

/* FIGHT CARD */
.fight-card {
    background:#1a1a1a;
    border:2px solid red;
    border-radius:12px;
    padding:15px;
    margin-bottom:15px;
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

.photo {
    width:100px;
    height:100px;
    border-radius:50%;
    border:4px solid red;
    overflow:hidden;
    margin-bottom:5px;
}

.photo.winner {
    border-color:limegreen;
}

.photo img {
    width:100%;
    height:100%;
    object-fit:cover;
}

.name { font-weight:600; font-size:16px; }

.vs {
    font-size:24px;
    font-weight:700;
    color:red;
    margin:0 10px;
}

.weight {
    font-size:14px;
    color:#ccc;
    text-align:center;
    margin-top:5px;
    width:100%;
}

/* FOOTER */
footer {
    text-align:center;
    padding:15px;
    background:#1a1a1a;
    border-top:2px solid red;
    color:#ccc;
    font-size:12px;
}

/* Мобильная адаптация */
@media screen and (max-width:480px){
    .photo { width:80px; height:80px; }
    .name { font-size:14px; }
    .vs { font-size:20px; margin:0 5px; }
    .weight { font-size:12px; }
    .ufc-link{ font-size:12px; padding:5px 10px; }
    .fight-card { flex-wrap:wrap; gap:10px; justify-content:center; }
}
</style>
</head>

<body>

<div class="header-inner">
    <h1>UFC 343</h1>
    <a class="ufc-link" href="https://AlishkaNepo.github.io/UFC-S/" target="_blank">UFC 344</a>
</div>

<!-- Бой 1 -->
<div class="fight-card">
    <div class="fighter">
        <div class="photo winner">
            <img src="ali.jpg" alt="Али">
        </div>
        <div class="name">Али</div>
    </div>

    <div class="vs">VS</div>

    <div class="fighter">
        <div class="photo">
            <img src="beka2.jpg" alt="Бексултан">
        </div>
        <div class="name">Бексултан</div>
    </div>

    <div class="weight">Полулегкий вес • Главный бой<br><span style="color:limegreen;font-weight:bold;">Судейское решение Р5 05:00</span></div>
</div>

<!-- Бой 2 -->
<div class="fight-card">
    <div class="fighter">
        <div class="photo winner">
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

    <div class="weight">Легкий вес • Со-главный бой<br><span style="color:limegreen;font-weight:bold;">Добровольная сдача Р2 02:34</span></div>
</div>

<footer>
© 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
