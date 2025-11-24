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
    margin:10px 0;
    font-size:24px;
}

.header{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:10px;
    flex-wrap:wrap;
    margin-bottom:20px;
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

.container{
    max-width:1000px;
    margin:0 auto 30px auto;
    padding:0 15px;
}

/* Блок боя */
.fight{
    border:2px solid red;
    border-radius:15px;
    padding:15px;
    margin-bottom:25px;
    background:#1a1a1a;
    display:flex;
    justify-content:space-between;
    align-items:center;
    flex-wrap:wrap;
}

/* Левая часть */
.fighters{
    display:flex;
    align-items:center;
    gap:15px;
    flex-wrap:wrap;
    justify-content:center;
    width:100%;
}

.fighter{
    text-align:center;
    flex:1 1 100px;
}

.photo{
    width:100px;
    height:100px;
    border-radius:50%;
    border:5px solid red;
    object-fit:cover;
}

.winner{
    border-color:limegreen;
}

.vs{
    color:red;
    font-size:24px;
    font-weight:bold;
    flex-shrink:0;
}

/* Правая часть */
.info{
    text-align:center;
    margin-top:10px;
    width:100%;
    font-size:14px;
}

.info span{
    font-weight:bold;
}

/* Панель изменения фото */
.input-panel{
    background:#222;
    padding:15px;
    border-radius:10px;
    margin-top:20px;
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
@media(max-width:480px){
    h1{
        font-size:20px;
    }
    .photo{
        width:80px;
        height:80px;
        border-width:4px;
    }
    .vs{
        font-size:20px;
    }
    .info{
        font-size:13px;
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
        Полулегкий вес • Главный бой<br>
        <span style="color:limegreen;">Судейское решение Р5 05:00</span>
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
        Легкий вес • Со-главный бой<br>
        <span style="color:limegreen;">Добровольная сдача Р2 02:34</span>
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
