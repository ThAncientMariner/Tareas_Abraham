Tareas_Abraham
==============
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Jquery Efectos</title>
 <script src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
  <script src="http://code.jquery.com/color/jquery.color.svg-names-2.1.2.min.js"></script>
</head>

<body>

<input type="button" value="aparece" onClick="aparece();"/>
<input type="button" value="desaparece" onClick="desaparece();"/>
<input type="button" value="fadein" onClick="fadein();"/>
<input type="button" value="fadeout" onClick="fadeout();"/>
<input type="button" value="toggle" onClick="toggle();"/>
<input type="button" value="slide" onClick="slide();"/>


<div class="clear"></div>

<style type="text/css" media="screen">
	
	.clear{
		clear:both;	
		}
	.cuadro{
		float:left;
		margin: 5px;
		width: 200px;
		height: 200px;
	}
	#rojo{
		background: red;
		display:none;
	}
	#azul{
		background: blue;
		display:none;
	}
	#verde{
		background: green;
		display:none;
	}
	#negro{
		background: black;
		display:none;
	}
	#zanahoria{
		background: #FF6600;
		display:none;
	}

</style>

<script type="text/javascript" charset="utf-8">

	function aparece(){
		$("#rojo").show();
	};
	
	
	function desaparece(){
		$("#rojo").hide();
	};
	
	function fadein(){
		$("#azul").fadeIn(1000, function(){
			$("#verde").fadeIn(1000)
			});
	};
	
	
	function fadeout(){
		$("#azul").fadeOut(1000, function(){
				$("#verde").fadeOut();
			});
	};
	function toggle(){
		$("#azul").fadeToggle();
	}
	
	function slide(){
		$("#negro").slideToggle();
	};
	
	
	$(document).ready(function() {
        $("#rojo").click(function(){
				$("#zanahoria").fadeIn();
			});
		$("#azul").mouseenter(function(){
				$("#zanahoria").fadeIn(200);
			});
			$("#azul").mouseleave(function(){
				$("#zanahoria").fadeOut(200);
			});
			
			$("#verde").mouseenter(function(){
				$("#zanahoria").css("width", "300");
			});
			$("#verde").mouseleave(function(){
				$("#zanahoria").css("width", "200");
			});
			
			$("#negro").click(function(){
				$("#zanahoria").animate({
					width: "500px",
					backgroundColor: "#2e8b57",
					}, 1000)
				});
		
    });
	

</script>

<div id="rojo" class="cuadro"></div>
<div id="azul" class="cuadro"></div>
<div id="verde" class="cuadro"></div>
<div id="negro" class="cuadro"></div>
<div id="zanahoria" class="cuadro"></div>
<div class="clear"></div>

</body>
</html>
