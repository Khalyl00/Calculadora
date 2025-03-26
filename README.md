<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Calculadora</title>
</head>
<body>
    <h1>Minha Calculadora</h1>

    Primeiro numero<br />
    <input Id="n1" type=" number" /><br />
    Segundo numero <br />
    <input Id="n2" type=" number" /><br />
    <button onclick="somar()">Somar</button>
    <button onclick="subtrair()">Subtrair</button>
    <button onclick="multiplicar()">Multiplicar</button>
    <button onclick="dividir()">Dividir</button>
    <br /><br />
    o Resultado é <spam></spam>

    <script>
        var n1 = document.querySelector('#n1')
        var n2 = document.querySelector('#n2')
        var resultado = document.querySelector('spam')

        function somar() {
            resultado.innerHTML = parseInt(n1.value) + parseInt(n2.value)
        }
        function subtrair() { 
            alert('Subtraiu');
            resultado.innerHTML = parseInt(n1.value) - parseInt(n2.value)
        }
        function multiplicar() {
            resultado.innerHTML = parseInt(n1.value) * parseInt(n2.value)
        }
        function dividir() {
            console.log('Dividiu');
            resultado.innerHTML = parseInt(n1.value) / parseInt(n2.value)
        }
    </script>
</html>
