<!DOCTYPE html>
<html>
<head><title>Image Display Test</title>

	<style>
		
		p {
		
			text-align: center;
			color: rgb(3, 3, 3);
		}
		
		.column {
 	 		float: left;
  			width: 25%;
  			padding: 10px;
		}

		.row::after {
 			 content: "";
  			clear: both;
  			display: table;
		}

	</style>
	
    <script type="text/javascript">

    var count=0; 
    var numImg = 6; 


  
    function onClick() {

 		count+=1;

        if (count === 1){
        	document.getElementById('Image1').style.visibility="visible";
        }

        if (count === 2){
			document.getElementById('Image2').style.visibility="visible";

        }

        if (count === 3){
        	document.getElementById('Image3').style.visibility="visible";
        }

        if (count === 4){
			document.getElementById('Image4').style.visibility="visible";

        }
        if (count === 5){
        	document.getElementById('Image5').style.visibility="visible";
        }

        if (count === 6){
			document.getElementById('Image6').style.visibility="visible";

        }
    }

    </script>

</head>
<body>
	
	<p><b> Test Button </b></p>
    <input type="button" value="add" onclick="onClick();" style="height: 50px; background-color: blue;position: absolute; left: 50%; transform: translateX(-50%);"/>
	<br><br>



	<div class="row">
  		<div class="column">
    		<img id="Image1" src="56.jpg" class="position" style="visibility:hidden" width="256" height="256"/>
    	</div>
    	<div class="column">
    		<img id="Image2" src="333.jpg" class="position" style="visibility:hidden" width="256" height="256"/>
    	</div>
    	<div class="column">
    		<img id="Image3" src="41.jpg" class="position" style="visibility:hidden" width="256" height="256"/>
    	</div>
    </div>
    <div class="row">
    	<div class="column">
    		<img id="Image4" src="252.jpg" class="position" style="visibility:hidden" width="256" height="256"/>
    	</div>
    	<div class="column">
			<img id="Image5" src="63.jpg" class="position" style="visibility:hidden" width="256" height="256"/>
		</div>
		<div class="column">
			<img id="Image6" src="111.jpg" class="position" style="visibility:hidden" width="256" height="256"/>
		</div>
	</div>
	
</body>
</html
