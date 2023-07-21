<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>

<style type="text/css">
*{
   margin: 0;
   padding: 0;
}

main{
   background-color: #c5d3f8;
   margin: 0 auto; 
   border-bottom: 1px dotted #080007;
   padding: 0 0 0 0; 
   width: 1050px;
}

main.first-main {
    height: 450px;
}

main.second-main {
    height: 250px;
}

#box1 {
    background-color: #ffffff;
    width: 495px;
    height: 400px;
    border: 2px dotted #000000;
    float: left;
    margin : 20px 17px 15px 17px;
   position : relative
}

#box1 p {
    position: absolute; 
    top: 5%; 
    left: 50%; 
   transform : translate(-50%, -50%)
}

#box2{
   background-color: #ffffff;
   width: 495px;
   height: 400px;
    border: 2px dotted #000000;
   float: right;
   margin : 20px 17px 15px 0px; /* top right bottom left 순 */
   position : relative
}

#box2 p {
    position: absolute; 
    top: 5%; 
    left: 50%; 
   transform : translate(-50%, -50%)
}

.map-image {
    width: 350px;
    height: auto;
   position: absolute;
   left : 80px;
   bottom : 10px
}

#box3{
   background-color: #ffffff;
   width: 323px;
   height: 200px;
    border: 2px dotted #000000;
   float: left;
    margin: 20px 17px 20px 17px; /* top right bottom left 순 */
   position : relative
}

<!-- #box3 p {
    position: absolute; 
    top: 10%; 
    left: 50%; 
   transform : translate(-50%, -50%)
} -->

#unit {
   margin: 80px 150px 0px 30px;
   font-size: 30px;
   color: #000000;
}

.custom-button {
    background-color: #efa0f5;
    color: #000000;
    border: 1px solid #efa0f5;
    padding: 5px 10px;
    font-size: 10px;
    cursor: pointer;
    border-radius: 10px;
   position: absolute;
   right : 20px;
   bottom : 80px
}


#box4{
   background-color: #ffffff;
   width: 323px;
   height: 200px;
    border: 2px dotted #000000;
   float: left;
    margin: 20px 17px 20px 0px;
   position : relative
}

#box4 p {
    position: absolute; 
    top: 10%; 
    left: 50%; 
   transform : translate(-50%, -50%)
}

#box5{
   background-color: #ffffff;
   width: 323px;
   height: 200px;
    border: 2px dotted #000000;
   float: right;
    margin: 20px 17px 20px 0px;
   position : relative
}

#box5 p {
    position: absolute; 
    top: 10%; 
    left: 50%; 
   transform : translate(-50%, -50%)
}

.wind-image {
    width: 80px;
    height: auto;
   position: absolute;
   right : 20px;
   bottom : 20px
}


</style>

</head>
<body>

<main class="first-main">

    <div id="box1">
        <p>카메라</p>
    </div>

    <div id="box2">
        <p>지도</p>
      <img src="https://blog.kakaocdn.net/dn/cV7bPu/btqCjdXg9XK/yBH7hBLIAm5UPwykndnQyk/img.gif" alt="지도" class="map-image">
    </div>
</main>

<main class="second-main">
   <div id="box3">
        <p id="speed">속도</p>
      <p id="unit">km/h</p>
        <button id="changeTextButton" class="custom-button">Change</button>
    </div>

    <script>
        const changeTextButton = document.getElementById('changeTextButton');
        const speedParagraph = document.getElementById('unit');

        changeTextButton.addEventListener('click', function () {
            if (speedParagraph.textContent === 'km/h') {
                speedParagraph.textContent = 'knot(kn)';
            } else {
                speedParagraph.textContent = 'km/h';
            }
        });
    </script>

    <div id="box4">
        <p>각도</p>
    </div>

    <div id="box5">
        <p>바람</p>
      <img src="https://cdn.pixabay.com/animation/2023/03/15/13/04/13-04-56-75_512.gif" alt="바람 이미지" class="wind-image">
    </div>
</main>
</body>
</html>
