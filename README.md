# Cricket-.com
This my cricket game play and enjoy 
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cricket Game and Name/Passion</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f2f2f2; /* Background color */
      color: #333; /* Main color */
    }
    footer {
      background-color: #333; /* Footer background color */
      color: #fff; /* Footer text color */
      padding: 10px 0;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      margin: 10px;
      background-color: #007bff; /* Button background color */
      color: #fff; /* Button text color */
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3; /* Button background color on hover */
    }
    #score {
      font-size: 24px;
      margin-top: 20px;
    }
    #container {
      margin-top: 50px;
      position: relative;
    }
    #name {
      font-size: 24px;
      margin-bottom: 10px;
    }
    #passion {
      font-size: 18px;
      margin-bottom: 20px;
    }
    .image {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
    }
    .left-image {
      left: 0;
    }
    .right-image {
      right: 0;
    }
    .cricket-equipment {
      position: absolute;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);
    }
  </style>
</head>
<body style="background-color: #ffffff;"> <!-- Main page background color -->
  <h1>GANESH CRICKET GAME</h1>
  <div id="container">
    <img src="https://r2.easyimg.io/dtdfxms19/virat-kohli-plays-a-cover-drive-1366x900-1.jpg" alt="Left Image" class="image left-image">
    <img src="https://r2.easyimg.io/dtdfxms19/img-20240319-wa0008.jpg" alt="Right Image" class="image right-image">
    <div id="name">GANESH</div>
    <div id="passion"></div>
  </div>
  <h2>Cricket Game</h2>
  <button onclick="hit()">Hit</button>
  <button onclick="reset()">Reset</button>
  <p id="score">Score: <span id="currentScore">0</span></p>

  <script>
    let score = 0;

    function hit() {
      const runs = Math.floor(Math.random() * 7); // Random runs between 0 and 6
      score += runs;
      document.getElementById("currentScore").textContent = score;
      if (runs === 0) {
        alert("Out! Your final score is " + score);
        reset();
      }
    }

    function reset() {
      score = 0;
      document.getElementById("currentScore").textContent = score;
    }
  </script>
  <footer>
    <p>Thank you for playing this game</p>
  </footer>
</body>
</html>
