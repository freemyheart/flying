<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>定位和居中问题</title>
	<style>
		body{
			margin: 0;
			padding: 0;
		}
		.plan-a,.plan-b{
			width: 900px;
			height: 600px;
			border:1px solid #000000;
			position: relative;
		}
		.center{
			width: 400px;
			height: 200px;
			background: grey;
			position: absolute;
			top:50%;
			left: 50%;
			margin: -100px 0 0 -200px;
			overflow: hidden;
		}
		.round-left-top , .round-right-bottom,.round-left-top-b , .round-right-bottom-b{
			position: absolute;
			width: 100px;
			height: 100px;
			background: rgb(254,195,9);
			border-radius: 50px;
		}
		.round-left-top{
			left: -50px;
			top: -50px;
		}
		.round-right-bottom{
			right: -50px;
			bottom: -50px;
		}
		.center-b{
			width: 400px;
			height: 200px;
			background: grey;
			position: absolute;
			top:50%;
			left: 50%;
			-webkit-transform: translate(-50%,-50%);
					transform: translate(-50%,-50%);
			overflow: hidden;
		}
		.plan-c{
			width: 900px;
			height: 600px;
			border:1px solid #000000;
			justify-content:center;
			align-items:center;
			display:-webkit-flex;
		}
		.center-c{
			width: 400px;
			height: 200px;
			background: grey;
			position: relative;
			overflow: hidden;
		}
	</style>
</head>
<body>
	<div class="plan-a">
		<div class="center">
			<div class="round-left-top"></div>
			<div class="round-right-bottom"></div>
		</div>
	</div>
	<div class="plan-b">
		<div class="center-b">
			<div class="round-left-top"></div>
			<div class="round-right-bottom"></div>
		</div>
	</div>
	<div class="plan-c">
		<div class="center-c">
			<div class="round-left-top"></div>
			<div class="round-right-bottom"></div>
		</div>
	</div>
</body>
</html>
