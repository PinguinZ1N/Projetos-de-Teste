<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora</title>
    <style>
        body {
            background-color: rgb(0, 0, 0);
        }
        section {
            margin: auto;
            text-align: center;
            font: 70px Arial;
            background-color: rgb(39, 38, 38);
            width: 400px;
            height: 500px;
            border-radius: 30px;
        }
        input {
            font: 45px Arial;
            text-align: center;
            width: 75px;
            height: 75px;
            border-radius: 12px;
            background-color: rgb(81, 80, 80);
            box-shadow: black 10px 10px 10px;
            color: rgb(41, 2, 77);
        }
        header{
            text-align: center;
            font: normal 60px ARIAL;
            color: blueviolet;
        }
        
        div {
            font: 50px normal Arial;
            color: blueviolet;
            background-color: rgb(80, 80, 80);
            border-radius: 50px;
            box-shadow: black 10px 10px 10px;
        }
    </style>
</head>
<body>
    <header>CALCULATOR 5.1</header>
    
    <section> 
        <input type="button" value="7" onclick="add('7')">   <input type="button" value="8" onclick="add('8')">   <input type="button" value="9" onclick="add('9')">   <input type="button" value="+" onclick="add('+')">  <br>
        <input type="button" value="4" onclick="add('4')">   <input type="button" value="5" onclick="add('5')">   <input type="button" value="6" onclick="add('6')">   <input type="button" value="-" onclick="add('-')">  <br>
        <input type="button" value="1" onclick="add('1')">   <input type="button" value="2" onclick="add('2')">   <input type="button" value="3" onclick="add('3')">   <input type="button" value="*" onclick="add('*')">  <br>
        <input type="button" value="0" onclick="add('0')"> <input type="button" value="CE" onclick="limpar()"> <input type="button" value="=" onclick="resultado('=')"> <input type="button" value="/" onclick="add('/')">  <br>
        <p></p>
        <div id="res">0</div>
    </section>

    <script>
        var res = window.document.getElementById("res")
        var valor = ""

        function add(conta) {   
            valor += conta
            res.innerHTML = valor
            
        }
        function limpar(clean) {
            valor = 0
            res.innerHTML = valor
            valor = ""


        }
        function resultado(igual) {
            res.innerHTML = eval(valor)



        }
    </script>
</body>
</html>

