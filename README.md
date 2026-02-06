<!DOCTYPE html>
<html>
<head>
  <title>Valentine</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background-color: #ffe6eb;
      margin-top: 100px;
    }

    h1 {
      color: #ff3366;
      font-size: 36px;
    }

    button {
      font-size: 22px;
      padding: 15px 30px;
      border-radius: 12px;
      border: none;
      cursor: pointer;
      margin: 20px;
    }

    #yes {
      background-color: #ff3366;
      color: white;
    }

    #no {
      background-color: #ddd;
      position: absolute;
    }

    #message {
      font-size: 30px;
      color: #ff3366;
      margin-top: 40px;
      display: none;
    }
  </style>
</head>

<body>

  <h1>Shantanu 💖</h1>
  <h1>Will you be my Valentine?</h1>

  <button id="yes" onclick="yesClicked()">Yes Rutuja 💕</button>
  <button id="no" onmouseover="moveNo()">No</button>

  <div id="message">YAY!!! 😍💘 Thank you!!!</div>

  <script>
    function moveNo() {
      const noBtn = document.getElementById("no");
      noBtn.style.left = Math.random() * 300 + "px";
      noBtn.style.top = Math.random() * 300 + "px";
    }

    function yesClicked() {
      document.getElementById("message").style.display = "block";
    }
  </script>

</body>
</html>
