Tareas_Abraham
==============
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Operaciones Matematicas</title>

<style type="text/css" media="screen">

	.operacion{
		width:25%;
		min-height:200px;
		float: left;
	}
	#suma #multiplicacion{
		background: #bdc3c7c;
	}
	.clear{
		clear:both;
	}
	h1{
		text-align:center;
	}
	input [type=text]{
		width:
	}

</style>`

<script type="text/javascript" charset="utf-8">
	function fsuma(){
		document.getElementById("rsuma").innerHTML=parseFloat(document.getElementById("s1").value) + parseFloat(document.getElementById("s2").value);
	}
	function fborrar(x){
		if(x == 1){
			document.getElementById("s1").value = "";
			document.getElementById("s2").value = "";
		}
	}
</script>


</head>

<body>
	<h1>Operaciones Matematicas</h1>
	<div id="suma" class="operacion">
    	<input type="text" id="s1"/>
        <span class="operador">+</span>
        <input type="text" id="s2"/>
        <input type="button" value="Sumar" id="sumar" onClick="fsuma()"/>
        <div class="resultado" id="rsuma"></div>
        <input type="button" value="Borrar" id="borrar" onClick="fborrar(1)"/>
        
    </div>
    <div id="resta" class="operacion">
    	<input type="text" id="r1"/>
        <span class="operador">-</span>
        <input type="text" id="r2"/>
        <input type="button" value="Restar" id="resultado1"/>
        <div class="resultado">232</div>
    </div>
    <div id="multiplicacion" class="operacion"></div>
    <div id="divicion" class="operacion"></div>
   
</body>
</html>

