<!DOCTYPE html>
<html>
<head>
<style>
body{
  background:black;
  color:pink;
  font-size:30px;
  text-align:center;
  margin-top:120px;
  font-family:serif;
  text-shadow:0 0 10px pink, 0 0 20px hotpink;
}
</style>
</head>

<body>

<div id="type"></div>

<script>
let text = "Hello Kris, this is your first typewriter!";
let i = 0;

function typeWriter() {
  if (i < text.length) {
    document.getElementById("type").innerHTML += text.charAt(i);
    i++;
    setTimeout(typeWriter, 80);
  }
}

typeWriter();
</script>

</body>
</html>
