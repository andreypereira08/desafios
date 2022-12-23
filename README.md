<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- <link rel="stylesheet" href="style.css"> -->
    <!-- CSS only -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
<script src="https://unpkg.com/phosphor-icons"></script>

<style>
    *{
    margin: 0;
    padding: 0;
    border: 0;
    box-sizing: border-box;
}

body{
    background-color: #e8e8e8;
    display: flex;
    align-items: center;
    justify-content: center;

    height: 100vh;
    margin: 0;
    transition: background 0.2s linear;
}

body.dark{
    background-color: #212121;
}

body .mode{
    position: fixed;
    margin-top: -90vh;
    margin-right: -90vw;
}

.checkbox{
    opacity: 0;
    position: absolute;
    display: inline-block;
}

.label{
    background-color: rgb(89, 89, 89);
    border-radius: 50px;
    cursor: pointer;
    
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 5px;
    position: relative;
    height: 26px;
    width: 50px;
    margin-right: 10px;

    transform: scale(1.5);   
}

.label .bola{
    background-color: white;
    border-radius: 50%;
    position: absolute;
    top: 2px;
    left: 2px;

    height: 22px;
    width: 22px;

    transform: translateX(0px);
    transition: transform 0.2s linear;
}

.checkbox:checked + .label .bola{
    transform: translateX(24px);
}

.sol{
    color: #f1cf39;
}

.lua{
    color: rgb(155, 155, 155);
}
</style>

</head>
<body>
    <div class="mode">
        <input type="checkbox" id="chk" class="checkbox">
        <label for="chk" class="label">
            <i class="ph-moon lua"></i>
            <i class="ph-sun sol"></i>
                <!-- <span class="material-symbols-outlined lua">dark_mode</span> -->
                <!-- <span class="material-symbols-outlined sol">light_mode</span> -->
        <div class="bola"></div>
        </label>
    </div>
<div class="container">
    <h1><a href="https://andreypereira08.github.io/desafios/" target="_blank">Abrir Página Principal - Desefios</a></h1>
    <br>
    <h2>desafio 006, 007, 008, load</h2>
    <br/><br/>  
    <ul>
        <li><a href="https://andreypereira08.github.io/desafios/d006" target="_blank">Executar o desafio 006</a></li>
        <li><a href="https://andreypereira08.github.io/desafios/d007" target="_blank">Executar o desafio 007</a></li>
        <li><a href="https://andreypereira08.github.io/desafios/d008" target="_blank">Executar o desafio 008</a></li>
        <li><a href="https://andreypereira08.github.io/desafios/d011" target="_blank">Executar o desafio 011</a></li>
        <li><a href="https://andreypereira08.github.io/desafios/load" target="_blank">Executar o desafio load</a></li>
    </ul>
</div>
    <script>
        const chk = document.getElementById('chk')

        chk.addEventListener('change', ()=> {
            document.body.classList.toggle('dark')
        })
    </script>
</body>
</html>
