Tareas_Abraham
==============
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>manipulación de inputs</title>
	
</head>

<body>
<input type="text" name="pais" value="" id="pais"/>
<input type="button" name="boton" value="write" id="boton" onClick="escribe();">
<input type="button" name="boton" value="I'm Death" id="boton" onClick="borra();">
<input type="button" name="boton" value="País" id="boton" onClick="escribePais();">
<div id="contienePais"></div>


<script type="text/javascript" chartset="utf-8">

		/*function pierna(v1, v2){
			alert(v2 + v1);
			};*/
			
			//pierna();
			
			function escribe(){
					document.getElementById("pais").value="Feed me";
					document.getElementById("pais").focus();
				};
				function borra(){
					document.getElementById("pais").value="";
				};
				function escribePais(){
					document.getElementById("contienePais").innerHTML=document.getElementById("pais").value;
				};
				//escribe();
	</script>
		<style type="text/css" media="screen">
            #contienePais{
                font-size:100px;
                text-align:center;
            }
            
        </style>
    
    
   

</body>
</html>
