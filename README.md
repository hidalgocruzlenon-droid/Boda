<!DOCTYPE html><html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Boda Alexander & Pierina</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">
<style>
body {
  margin: 0;
  font-family: 'Montserrat', sans-serif;
  background-color: #f9f9f7;
  color: #333;
  text-align: center;
}
.section {
  padding: 60px 20px;
  animation: fadeInUp 1.2s ease;
}
.title {
  font-family: 'Playfair Display', serif;
  font-size: 2.5em;
  color: #556b2f;
}
.subtitle {
  font-size: 1.2em;
  margin-top: 10px;
}
.divider {
  width: 60px;
  height: 2px;
  background: gold;
  margin: 20px auto;
}
.box {
  background: white;
  margin: 20px auto;
  padding: 20px;
  border-radius: 15px;
  max-width: 500px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.08);
  animation: fadeInUp 1.5s ease;
}
.countdown {
  font-size: 1.5em;
  color: #556b2f;
}
.footer {
  font-size: 0.9em;
  color: #777;
}
button, a.button {
  display:inline-block;
  margin-top:15px;
  padding:12px 22px;
  background:#556b2f;
  color:white;
  text-decoration:none;
  border-radius:10px;
  font-weight:bold;
  transition: all 0.3s ease;
}
button:hover, a.button:hover {
  background:#6b8e23;
  transform: scale(1.05);
}
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
</head>
<body><!-- Música de fondo --><audio autoplay loop>
  <source src="https://cdn.pixabay.com/audio/2023/03/14/audio_0b6e5c8c6b.mp3" type="audio/mpeg">
</audio><div class="section">
  <div class="title">Alexander & Pierina</div>
  <div class="subtitle">¡Nos casamos!</div>
  <div class="divider"></div>
  <p>Con la bendición de Dios y nuestros padres,<br>queremos invitarte a celebrar nuestro matrimonio.</p>
</div><div class="section">
  <div class="title">23 Mayo 2026</div>
  <div class="subtitle">3:00 PM</div>
  <div class="divider"></div>
  <p>San Alberto Mz A Lote 1<br>Chosica</p>
</div><div class="section">
  <div class="title">Ubicación</div>
  <div class="divider"></div>
  <a href="https://www.google.com/maps/search/?api=1&query=San+Alberto+Mz+A+Lote+1+Chosica+Peru" target="_blank" class="button">Ver ubicación en Google Maps</a>
</div><div class="section">
  <div class="title">Cuenta regresiva</div>
  <div id="countdown" class="countdown"></div>
</div><div class="section box">
  <div class="title">Código de vestimenta</div>
  <p>Elegante<br><br>
  Con todo el cariño, les pedimos evitar prendas de color blanco o beige</p>
</div><div class="section box">
  <div class="title">Confirmación</div>
  <p>Haz clic para confirmar tu asistencia:</p>
  <a href="https://wa.me/51913222203?text=Confirmo%20mi%20asistencia%20a%20su%20boda" target="_blank" class="button">Confirmar por WhatsApp</a>
</div><div class="section footer">
  <p>Acompáñanos en este día tan especial 💖</p>
</div><script>
const weddingDate = new Date("May 23, 2026 15:00:00").getTime();
const countdown = document.getElementById("countdown");

setInterval(() => {
  const now = new Date().getTime();
  const distance = weddingDate - now;

  const days = Math.floor(distance / (1000 * 60 * 60 * 24));
  const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));

  countdown.innerHTML = `${days} días ${hours} horas ${minutes} minutos`;

  if (distance < 0) {
    countdown.innerHTML = "¡Hoy es el gran día!";
  }
}, 1000);
</script></body>
</html>
