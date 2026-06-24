<!DOCTYPE html>
<html lang="my">
<head>
  <meta charset="UTF-8">
  <title>Love Question</title>
  <style>
    body {
      text-align: center;
      font-family: Arial;
      margin-top: 100px;
    }
    button {
      padding: 10px 20px;
      margin: 10px;
      font-size: 20px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <h1>မင်း ငါကို ချစ်လား? 💖</h1>

  <button id="yesBtn" onclick="answerYes()">Yes ❤️</button>
  <button onclick="answerNo()">No 💔</button>

  <h2 id="result"></h2>

  <script>
    let size = 20;

    function answerYes() {
      document.getElementById("result").innerText = "ကိုကိုလည်း အရမ်းချစ်ပါတယ် 😍";
    }

    function answerNo() {
      let yesBtn = document.getElementById("yesBtn");
      size += 10; // size တိုး
      yesBtn.style.fontSize = size + "px";
      yesBtn.style.padding = (size/2) + "px";
    }
  </script>

</body>
</html>
