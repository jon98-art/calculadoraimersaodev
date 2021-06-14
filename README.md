# calculadoraimersaodev

<html>

<head>
    <title>
        Imersão Dev - Aula 02
    </title>
</head>

<body>
    <div class="container">
        <h1 class="page-title">
            Calculadora
        </h1>
        <img src="https://www.alura.com.br/assets/img/imersoes/dev-2021/logo-imersao-calculadora.svg" class="page-logo"
            alt="">
        <div class="calculadora">
        </div>
    </div>
    <a href="https://alura.com.br/" target="_blank">
        <img src="https://www.alura.com.br/assets/img/home/alura-logo.svg" alt="" class="alura-logo">
    </a>
</body>
  
  body {
    font-family: 'Roboto Mono',monospace;
    min-height: 854px;
    background-image: url('https://www.alura.com.br/assets/img/imersoes/dev-2021/dia-2-calculadora-certa.pn');
    background-color: #000000;
    background-size: cover;
    background-position: center top;
    background-repeat: no-repeat;
  }
  
  .container {
    text-align: center;
    padding: 30px;
    height: 100vh;
  }
  
  .page-title {
    color: #ffffff;
    margin: 0 0 5px;
  }
  
  .page-subtitle {
    color: #ffffff;
    margin-top: 5px;
  }
  
  .page-logo {
    width: 200px;
  }
  
  .calculadora {
    width: 264px;
    height:360px;
    background-image: url('https://www.alura.com.br/assets/img/imersoes/dev-2021/dia-2-calculadora-calc.png');
    margin: 0 auto;
    position: relative;
  }
  
  h2 {
    position: absolute;
    font-size:16px;
    font-weight:bold;
    top: 142px;
    left: calc(50% - 72.5px);
    width: 145px;
    text-align:center;
  }
  
  .alura-logo {
    width: 40px;
    position: absolute;
    top: 10px;
    right:10px;
  }

</html>

var primeiroValor = parseInt (prompt("Digite o primeiro valor:"))
var segundoValor = parseInt(prompt("Digite o segundo valor:"))

var operacao = prompt("Digite 1 para fazer uma divisão,Digite 2 para fazer uma multiplicação,Digite 3 para fazer uma soma,Digite 4 para fazer uma subtração" )

if (operacao == 1){
  var resultado = primeiroValor / segundoValor
  document.write("<h2>" + primeiroValor + " / " + segundoValor + " = " + resultado + "</h2>")
}
else if (operacao == 2){
  var resultado = primeiroValor * segundoValor
  document.write("<h2>" + primeiroValor + " x " + segundoValor + " = " + resultado + "</h2>")
}
 else if (operacao == 3){
  var resultado = primeiroValor + segundoValor
  document.write("<h2>" + primeiroValor + " + " + segundoValor + " = " + resultado + "</h2>") }
else if (operacao == 4){
  var resultado = primeiroValor - segundoValor
  document.write("<h2>" + primeiroValor + " - " + segundoValor + " = " + resultado + "</h2>") }

else {
  document.write("<h2>Opção Inválida</h2>")
}
