<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Angie & Raúl 💖 Nuestra Galaxia</title>

<style>
body {
    margin: 0;
    overflow: hidden;
    background: radial-gradient(circle at center, #12001f, #000000 85%);
    font-family: 'Segoe UI', sans-serif;
    color: white;
}

.star {
    position: absolute;
    color: #ffb3ec;
    animation: flotar linear infinite;
    white-space: nowrap;
    opacity: 0.9;
    text-shadow: 0 0 10px #ff7bdc;
}

@keyframes flotar {
    from {
        transform: translateY(100vh) scale(0.6);
        opacity: 0;
    }
    to {
        transform: translateY(-10vh) scale(1.2);
        opacity: 1;
    }
}

.center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    z-index: 10;
    padding: 20px;
}

h1 {
    font-size: 3.2em;
    color: #ff8fe3;
    text-shadow: 0 0 25px #ff6bd5;
}

p {
    font-size: 1.25em;
    color: #ffe6f7;
    max-width: 650px;
    line-height: 1.6;
}
</style>
</head>

<body>

<div class="center">
    <h1>✨ Angie & Raúl ✨</h1>
    <p>
        Angie, mi amor… 💕<br><br>
        En este universo infinito, cada estrella lleva un pedacito de lo que siento por ti.  
        Eres mi paz, mi alegría, mi motivación y el sueño que quiero cuidar toda la vida.  
        <br><br>
        Te amo hoy, te amaré mañana  
        y en todas las galaxias que existan 🌌💖  
        <br><br>
        — Raúl 💞
    </p>
</div>

<script>
const palabras = [
    "Angie 💖",
    "Mi Monii 💕",
    "Mi amor 💘",
    "Mi vida 💓",
    "Mi todo 🌎",
    "Mi alegría ✨",
    "Mi felicidad 🌷",
    "Mi amor eterno ♾️",
    "Mi amor infinito 💞",
    "Mi motivación 🌟",
    "Mi paz 🕊️",
    "Mi tranquilidad 💫",
    "Mis ganas de crecer 🌱",
    "Mi reina 👑",
    "Mi esposa 💍",
    "Te amo 💖",
    "Siempre contigo 💑",
    "Raúl ama a Angie 💕"
];

function crearEstrella() {
    const star = document.createElement("div");
    star.className = "star";
    star.textContent = palabras[Math.floor(Math.random() * palabras.length)];

    star.style.left = Math.random() * window.innerWidth + "px";
    star.style.fontSize = (14 + Math.random() * 12) + "px";
    star.style.animationDuration = (6 + Math.random() * 8) + "s";

    document.body.appendChild(star);

    setTimeout(() => {
        star.remove();
    }, 15000);
}

setInterval(crearEstrella, 350);
</script>

</body>
</html>

