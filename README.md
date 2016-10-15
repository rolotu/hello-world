<!DOCTYPE HTML>
<html>
<head lang="cn">
	<meta charset="utf-8">
	<title>简易计算器</title>
	<style>
		body{
			background-color:#e2e2e2;
			font-family:arial;
			font-size:14px;
			text-align:center;
		}
		.main{
			width:300px;
			height:200px;
			border:1px solid white;
			background-color:#f2f2f2; 
			margin:10px auto; 
		}
		.main .header{
			padding-top:10px;
			width:300px;
			height:30px;
			color:#FFF;
			background-color:#069;
		}
		h5{
			margin-top:5px;
			text-align:left;
			margin-left:18px;			
		}
		.main .shuru{
			padding-top:20px;	
		}
		.main .shuru .aaa{
			text-align:right;
		}
		.main .yes{
			padding:30px 0 0 30px;
		}
	</style>
	<script type="text/javascript">
		function xiangjia(){
			var a=document.getElementById("a1").value;
			var b=document.getElementById("b1").value;
			var c=Number(a)+Number(b);
			alert(c);
		}
		function xiangjian(){
			var a=document.getElementById("a1").value;
			var b=document.getElementById("b1").value;
			var c=Number(a)-Number(b);
			alert(c);
		}
		function xiangcheng(){
			var a=document.getElementById("a1").value;
			var b=document.getElementById("b1").value;
			var c=Number(a)*Number(b);
			alert(c);
		}
		function xiangchu(){
			var a=document.getElementById("a1").value;
			var b=document.getElementById("b1").value;
			var c=Number(a)/Number(b);
			alert(c);
		}
		function quyu(){
			var a=document.getElementById("a1").value;
			var b=document.getElementById("b1").value;
			var c=Number(a)%Number(b);
			alert(c);
		}
</script>
</head>
<body>
		<div class="main">
			<div class="header"><h5>简易计算器</h5></div>
				<form name="main" action="" method="get"> 
					<div class="shuru">
						<td>
							<tr>数值A：<input type="text" id="a1" class="aaa" placeholder="0"><br /></tr>
							<tr>数值B：<input type="text" id="b1" class="aaa" placeholder="0"></tr>
						</td>
					<div class="yes">
						<td>
							<tr><input name="jia" value="+" type="button" onClick="xiangjia()" /></tr>
							<tr><input name="jian" value="-" type="button" onClick="xiangjian()"/></tr>
							<tr><input name="cheng" value="x" type="button" onClick="xiangcheng()"/></tr>
							<tr><input name="chu" value="/" type="button" onClick="xiangchu()"/></tr>
							<tr><input name="qu" value="%" type="button" onClick="quyu()"/></tr>
						</td>
					</div>
				</form>
			</div>
		</div>
</body>
</html>
