# CalcularIMC
Um Progaminha simples, para calcular o IMC do usuário
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <script>
        function pulaLinha() {
            document.write("<br><br>")
        }

        function mostra(frase) {
            document.write(frase)
            pulaLinha()
        }

        function calculaImc(altura, peso) {
            let imc = peso / (altura * altura)
            return imc
        }
        let nome = prompt("Digite o seu nome:")
        let alturaInformada = prompt(nome + ", informe a sua altura:")
        let pesoInformado = prompt(nome + ", informe o seu peso:")
        let imc = calculaImc(alturaInformada, pesoInformado)
        if (alturaInformada === "" && pesoInformado === "") {
            alert("Digite um valor!")
        } else {
            document.write(nome + ", o seu IMC é: " + imc)
        }
    </script>

</body>

</html>
