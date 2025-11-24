<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Fight Card</title>

<style>
body{
    margin:0;
    background:#111;
    color:white;
    font-family:Arial, sans-serif;
}

h1{
    text-align:center;
    color:red;
    margin-top:20px;
}

.container{
    max-width:1000px;
    margin:30px auto;
    padding:20px;
}

/* Блок боя */
.fight{
    border:2px solid red;
    border-radius:15px;
    padding:20px;
    margin-bottom:30px;
    background:#1a1a1a;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

/* Левая часть */
.fighters{
    display:flex;
    align-items:center;
    gap:20px;
}

.fighter{
    text-align:center;
}

/* Фото */
.photo{
    width:100px;
    height:100px;
    border-radius:50%;
    border:5px solid red;
    object-fit:cover;
}

/* победная рамка */
.winner{
    border-color:limegreen;
}

.vs{
    color:red;
    font-size:30px;
    font-weight:bold;
}

/* Правая часть */
.info{
    text-align:right;
}

/* Панель изменения фото */
.input-panel{
    background:#222;
    padding:15px;
    border-radius:10px;
    margin-top:30px;
}

.input-panel h3{
    margin-top:0;
    color:red;
}

label{
    font-size:14px;
}

input{
    width:100%;
    padding:8px;
    margin-top:5px;
    margin-bottom:15px;
    background:#111;
    color:white;
    border:1px solid red;
    border-radius:5px;
}

/* Адаптация под телефон */
@media(max-width:700px){
    .fight{
        flex-direction:column;
        text-align:center;
    }
    .info{
        text-align:center;
        margin-top:15px;
    }
}

.header{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:15px;
}

.ufc-link{
    background:red;
    color:white;
    text-decoration:none;
    padding:6px 12px;
    border-radius:8px;
    font-size:14px;
    font-weight:bold;
    transition:0.2s;
}

.ufc-link:hover{
    background:#ff3b3b;
}
</style>
</head>

<body>

<div class="header">
    <h1>UFC 343</h1>
    <a class="ufc-link" href="https://AlishkaNepo.github.io/UFC-S/" target="_blank">Перейти на сайт</a>
</div>

<div class="container">

<!-- ================= БОЙ 1 ================= -->
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
        Полулегкий вес • Главный бой<br><br>
        <span style="color:limegreen;font-weight:bold;">Судейское решение Р5 05:00</span>
    </div>

</div>


<!-- ================= БОЙ 2 ================= -->
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
        Легкий вес • Со-главный бой<br><br>
        <span style="color:limegreen;font-weight:bold;">Добровольная сдача Р2 02:34</span>
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
