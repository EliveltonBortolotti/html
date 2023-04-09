<script> document.write("Qual número estou pensando"); </script>
<input type="text" id="numero"/>
<input type="submit" id="adivinhar"
	value="Compare"/>
<script>
var segredo = 10;
var caixaDoNumero = document.getElementById("numero");
var botaoClicado = function() {
	if(segredo == caixaDoNumero.value) {
		alert("Parabéns! Você acertou o número secreto!");
	}
	else {
		alert("Infelizmente você errou! O número era " + segredo);
	}
};
var botaoAdivinhar = document.getElementById("adivinhar");
botaoAdivinhar.onclick = botaoClicado;
</script>
