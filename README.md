<!DOCTYPE html>
<html>
<head>
  <title>Game Xả Stress</title>

  <style>
    body {
      text-align: center;
      background: #e6f7ff;
      font-family: Arial;
    }

    #bubble {
      width: 100px;
      height: 100px;
      background: pink;
      border-radius: 50%;
      position: absolute;
      top: 200px;
      left: 200px;
      cursor: pointer;
    }
  </style>
</head>

<body>

<h1>🎮 Click Bong Bóng</h1>
<p>Điểm: <span id="score">0</span></p>

<div id="bubble"></div>

<script>
let score = 0;

let bubble = document.getElementById("bubble");

bubble.onclick = function() {
  score++;
  document.getElementById("score").innerText = score;

  let top = Math.random() * 400;
  let left = Math.random() * 400;

  bubble.style.top = top + "px";
  bubble.style.left = left + "px";
};
</script>

</body>
</html>
