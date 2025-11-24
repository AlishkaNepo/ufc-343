<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Fight Card</title>

<style>
body {
    margin: 0;
    background: #111;
    color: white;
    font-family: Arial, sans-serif;
}

/* Заголовок и кнопка */
.header {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    flex-wrap: wrap;
    margin: 10px 0;
}

.header h1 {
    color: red;
    font-size: 22px;
    margin: 0;
}

.ufc-link {
    background: red;
    color: white;
    text-decoration: none;
    padding: 5px 10px;
    border-radius: 8px;
    font-size: 14px;
    font-weight: bold;
    transition: 0.2s;
}

.ufc-link:hover {
    background: #ff3b3b;
}

/* Контейнер */
.container {
    padding: 0 10px 20px 10px;
}

/* Блок боя */
.fight {
    border: 2px solid red;
    border-radius: 15px;
    padding: 15px;
    margin-bottom: 20px;
    background: #1a1a1a;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
}

/* Бойцы */
.fighters {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
}

.fighter {
    text-align: center;
    flex: 1;
}

.photo {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    border: 4px solid red;
    object-fit: cover;
}

.winner {
    border-color: limegreen;
}

.vs {
    font-size: 18px;
    font-weight: bold;
    color: red;
    margin: 0 5px;
    flex-shrink: 0;
}

/* Информация о бое */
.info {
    text-align: center;
    font-size: 14px;
}

.info span {
    font-weight: bold;
    color: limegreen;
}

/* Мобильная адаптация */
@media (max-width: 480px) {
    .fighters {
        flex-direction: row;
        gap: 10px;
    }

    .photo {
        width: 70px;
        height: 70px;
    }

    .vs {
        font-size: 16px;
    }

    .info {
        font-size: 13px;
    }
}
</style>
</head>

<body>

<div class="header">
    <h1>UFC 343</h1>
    <a class="ufc-link" href="https://AlishkaNepo.github.io/UFC-S/" target="_blank">UFC 344</a>
</div>

<div class="container">

<!-- Бой 1 -->
<div class="fight">
    <div class="fighters">
        <div class="fighter">
            <img id="aliPhoto" class="photo winner" src="ali.jpg">
            <div>Али</div>
        </div>

        <div class="vs">VS</div>

        <div class="fighter">
            <img id="beksultanPhoto" class="photo" src="beka.jpg">
            <div>Бексултан</div>
        </div>
    </div>
    <div class="info">
        Полулегкий вес • Главный бой<br>
        <span>Судейское решение Р5 05:00</span>
    </div>
</div>

<!-- Бой 2 -->
<div class="fight">
    <div class="fighters">
        <div class="fighter">
            <img id="romanPhoto" class="photo winner" src="roma.jpg">
            <div>Роман</div>
        </div>

        <div class="vs">VS</div>

        <div class="fighter">
            <img id="alikhanPhoto" class="photo" src="alikh.jpg">
            <div>Алихан</div>
        </div>
    </div>
    <div class="info">
        Легкий вес • Со-главный бой<br>
        <span>Добровольная сдача Р2 02:34</span>
    </div>
</div>

</div>

<script>
function changePhoto(id, path){
    if(path.trim() !== ""){
        document.getElementById(id).src = path;
    }
}
</script>

</body>
</html>
