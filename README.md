<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>İyi ki Doğdun Berat 🎂</title>

<style>
body {
  margin: 0;
  font-family: 'Arial', sans-serif;
  background: linear-gradient(135deg, #ffecd2, #fcb69f);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  background: #fff;
  border-radius: 20px;
  width: 90%;
  max-width: 380px;
  padding: 20px;
  text-align: center;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

img {
  width: 100%;
  border-radius: 15px;
  margin-bottom: 15px;
}

h1 {
  color: #ff6b6b;
  margin-bottom: 10px;
}

button {
  background: #ff6b6b;
  color: white;
  border: none;
  padding: 12px 20px;
  border-radius: 25px;
  font-size: 16px;
  cursor: pointer;
  margin-top: 15px;
}

button:hover {
  background: #ff4757;
}

.envelope {
  margin-top: 20px;
  perspective: 1000px;
  display: none;
}

.letter {
  width: 100%;
  background: #fffaf0;
  border-radius: 10px;
  padding: 20px;
  transform: rotateX(-90deg);
  transform-origin: top;
  transition: transform 1s;
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.letter.open {
  transform: rotateX(0deg);
}

.letter p {
  color: #444;
  font-size: 15px;
  line-height: 1.6;
}
</style>
</head>

<body>

<div class="container">
  <h1>🎉 İyi ki Doğdun!</h1>

  <img src="foto.jpg" alt="Berat">

  <button onclick="openLetter()">📜 Mektubu Aç</button>

  <div class="envelope" id="envelope">
    <div class="letter" id="letter">
      <p>
        Doğum günün kutlu olsun Beratım 🌹<br><br>
        Yeni yılda ve yaşında mutluluklar dilerim.<br>
        Pesde bu senede çakıcam 😄<br><br>
        Sevgilerle 🌹🌹🌹
      </p>
    </div>
  </div>
</div>

<script>
function openLetter() {
  document.getElementById("envelope").style.display = "block";
  setTimeout(() => {
    document.getElementById("letter").classList.add("open");
  }, 100);
}
</script>

</body>
</html>
