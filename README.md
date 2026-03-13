<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      background: black;
      color: pink;
      font-size: 30px;
      text-align: center;
      margin-top: 120px;
      font-family: serif;
      text-shadow: 0 0 10px pink, 0 0 20px hotpink;
    }
  </style>
</head>
<body>

<div id="type"></div>

<script>
let text = "Hello Kris, welcome to your typewriter effect!";
let i = 0;

function typeWriter() {
  if (i < text.length) {
    document.getElementById("type").innerHTML += text.charAt(i);
    i++;
    setTimeout(typeWriter, 100); // 100ms delay between letters
  }
}

typeWriter();
</script>

</body>
</html>
