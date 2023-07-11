# Sailing-Boat

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>

<style type="text/css">
*{ /* 모든태그에 적용 : * (초기값 설정) */
	margin: 0;
	padding: 0;
}

header{
	background-color: #0657f8;
	margin: 10px auto;	
	border: 1px solid #000000;
	padding: 5px;
	width: 1000px;
	height: 30px;
} 

main{
	background-color: #a9c2f9;
	margin: 0 auto; /* auto 알아서 중앙으로 맞춰줌 */
	border-bottom: 1px solid #000000;
	padding: 20px 0 20px 0; 
	width: 1000px;
	height: 400px;
}

#box1{
	background-color: #ffffff;
	width: 450px;
	height: 300px;
    border: 3px dotted #000000;
	float: left;
    margin-left: 20px
}
#box2{
	background-color: #ffffff;
	width: 450px;
	height: 300px;
    border: 3px dotted #000000;
	float: right;
    margin-right: 20px
}
#box3{
	background-color: #ffffff;
	width: 300px;
	height: 300px;
    border: 3px dotted #000000;
	float: left;
    margin-left: 10px
}
#box4{
	background-color: #ffffff;
	width: 300px;
	height: 300px;
    border: 3px dotted #000000;
	float: left;
    margin-left: 30px
}
#box5{
	background-color: #ffffff;
	width: 300px;
	height: 300px;
    border: 3px dotted #000000;
	float: right;
    margin-right: 20px
}


</style>

</head>
<body>

<header>
	<p>sailing boat</p>	
</header>

<main>
	<p>main 영역</p>
	
	<div id="box1">
		<p>카메라</p>
	</div>
	
	<div id="box2">
		<p>지도</p>
	</div>
</main>

<main>
    <p>두 번째 main 영역</p>

    <div id="box3">
      <p>속도</p>
    </div>

    <div id="box4">
      <p>각도</p>
    </div>

    <div id="box5">
        <p>바람</p>
    </div>
<main>

</body>
</html>
