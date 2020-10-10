<!DOCTYPE html>   
<html lang="en"> 
<head>
	<meta charset="utf-8">
	<title>JavaScript: Animation</title>
	<style type="text/css">
	
		#container{
			position: absolute; 
			left: 20px; 
			top: 20px; 
			height: 500px; 
			width: 500px;
			border: 3px solid #CCC; 
			background-color: #FFF;
			text-align: center;
		}
		.king{
			float: left; 
			width: 75px; 
			height: 100px;
			margin: 10px;
			background: rgb(235, 79, 79) url('4.jpg') no-repeat;
		}
		.box{	
			float: left; 
			width: 75px; 
			height: 100px;
			margin: 10px;
			background: rgb(235, 79, 79) url('5.jpg') no-repeat;
			
			}
	</style>
</head>

<body>
	<div id="container">
		
	</div>
	<script>



		var x;
		for(x=0;x<10;x++) {

			setTimeout(function(){

				var box = document.createElement('div');
				box.className = 'box';
				document.getElementById('container').appendChild(box);

				var b = document.createElement('k');
				b.className = 'king';
				document.getElementById('container').appendChild(b);
				
			
		
			
			},500*x);

		}



	</script>
</body>
</html>
