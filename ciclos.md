Tareas_Abraham
==============
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Ciclos</title>

<style type="text/css" media="screen">

	.marca{
		float:left;
		width:120px;
		height: 40px;
		line-height: 40px;
		text-align: center;
		background:#F36;
		color: #000;
		margin: 5px;
	}

</style>


</head>

<body>

	<button onClick="llamar()"> Mexican Grill </button>
    
    <div id="demo"></div>
    
    
  

<script type="text/javascript" charset="utf-8">
	
	function llamar(){
		comida = ["Tacos", "Enchiladas", "Pozole", "Quesadillas", "Chilaquiles", "Guacamole"];
		
		var text = "";
		
		for (i = 0; i < comida.length; i++) { 
			text += "<div class='marca'>" + comida[i] + "</div>";
			
		}
		document.getElementById("demo").innerHTML = text;
	};
	
</script>

</body>
</html>
