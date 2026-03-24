<html>
<head>
  <title>Happy Birthday</title>
  <style>
    body {
      margin: 0;
      text-align: center;
      font-family: Arial;
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      overflow: hidden;
    }
    h1 {
      margin-top: 20%;
      font-size: 50px;
      color: white;
      animation: fadeIn 2s ease-in-out;
    }
    p {
      color: white;
      font-size: 22px;
      animation: fadeIn 4s ease-in-out;
    }
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
    .flower {
      position: absolute;
      font-size: 24px;
      animation: fall linear infinite;
    }
    @keyframes fall {
      0% {top: -10%;}
      100% {top: 110%;}
    }
  </style>
</head>
<body>

<h1>🎉 Happy Birthday 🎉</h1>
<p>Wishing you success, happiness & a wonderful year ahead!</p>

<script>
for(let i=0; i<25; i++){
  let flower = document.createElement("div");
  flower.innerHTML = "🌸";
  flower.className = "flower";
  flower.style.left = Math.random()*100 + "vw";
  flower.style.animationDuration = (Math.random()*3+3)+"s";
  document.body.appendChild(flower);
}
</script>

</body>
</html>
