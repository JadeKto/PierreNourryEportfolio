<!-- =========================
STRUCTURE DU PROJET
=========================

/mon-site
│── index.html (Accueil)
│── sommaire.html
│── qui-je-suis.html
│── parcours.html
│── situation-apprentissage.html
│── /css
│     └── style.css
│── /js
│     └── script.js

========================= -->

<!-- =========================
STYLE GLOBAL AMÉLIORÉ (MODERNE)
========================= -->

/* css/style.css */

body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(135deg, #0f0f0f, #1c1c1c);
  color: #fff;
}

header {
  background: rgba(0,0,0,0.8);
  backdrop-filter: blur(10px);
  position: sticky;
  top: 0;
  z-index: 1000;
}

nav {
  display: flex;
  justify-content: center;
  gap: 30px;
  padding: 15px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 600;
  position: relative;
}

nav a::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  background: #00ffd5;
  left: 0;
  bottom: -5px;
  transition: 0.3s;
}

nav a:hover::after {
  width: 100%;
}

main {
  padding: 60px 20px;
  text-align: center;
}

h1 {
  font-size: 3rem;
  margin-bottom: 20px;
}

button {
  padding: 12px 25px;
  border: none;
  border-radius: 10px;
  background: #00ffd5;
  color: #000;
  font-weight: bold;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  transform: scale(1.05);
  background: #00c2a8;
}

.fade-in {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeIn 1s forwards;
}

@keyframes fadeIn {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* =========================
SCRIPT
========================= */

// js/script.js

document.addEventListener("DOMContentLoaded", () => {
  document.querySelectorAll('.fade-in').forEach((el, i) => {
    el.style.animationDelay = `${i * 0.2}s`;
  });
});

function goTo(page) {
  window.location.href = page;
}

/* =========================
PAGES HTML
========================= */

<!-- INDEX.HTML -->
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Accueil</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<header>
<nav>
<a href="index.html">Accueil</a>
<a href="sommaire.html">Sommaire</a>
<a href="qui-je-suis.html">Qui je suis</a>
<a href="parcours.html">Mon parcours</a>
<a href="situation-apprentissage.html">Situation d'apprentissage</a>
</nav>
</header>
<main>
<h1 class="fade-in">Bienvenue</h1>
<p class="fade-in">Découvre mon univers</p>
<button onclick="goTo('sommaire.html')" class="fade-in">Entrer</button>
</main>
<script src="js/script.js"></script>
</body>
</html>

<!-- SOMMAIRE.HTML -->
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sommaire</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<header>
<nav>
<a href="index.html">Accueil</a>
<a href="sommaire.html">Sommaire</a>
<a href="qui-je-suis.html">Qui je suis</a>
<a href="parcours.html">Mon parcours</a>
<a href="situation-apprentissage.html">Situation d'apprentissage</a>
</nav>
</header>
<main>
<h1 class="fade-in">Sommaire</h1>
<p class="fade-in">Navigation du site</p>
</main>
<script src="js/script.js"></script>
</body>
</html>

<!-- QUI JE SUIS -->
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Qui je suis</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<header>
<nav>
<a href="index.html">Accueil</a>
<a href="sommaire.html">Sommaire</a>
<a href="qui-je-suis.html">Qui je suis</a>
<a href="parcours.html">Mon parcours</a>
<a href="situation-apprentissage.html">Situation d'apprentissage</a>
</nav>
</header>
<main>
<h1 class="fade-in">Qui je suis</h1>
<p class="fade-in">Présentation personnelle</p>
</main>
<script src="js/script.js"></script>
</body>
</html>

<!-- PARCOURS -->
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Parcours</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<header>
<nav>
<a href="index.html">Accueil</a>
<a href="sommaire.html">Sommaire</a>
<a href="qui-je-suis.html">Qui je suis</a>
<a href="parcours.html">Mon parcours</a>
<a href="situation-apprentissage.html">Situation d'apprentissage</a>
</nav>
</header>
<main>
<h1 class="fade-in">Mon parcours</h1>
<p class="fade-in">Ton parcours ici</p>
</main>
<script src="js/script.js"></script>
</body>
</html>

<!-- SITUATION D'APPRENTISSAGE -->
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Situation d'apprentissage</title>
<link rel="stylesheet" href="css/style.css">
</head>
<body>
<header>
<nav>
<a href="index.html">Accueil</a>
<a href="sommaire.html">Sommaire</a>
<a href="qui-je-suis.html">Qui je suis</a>
<a href="parcours.html">Mon parcours</a>
<a href="situation-apprentissage.html">Situation d'apprentissage</a>
</nav>
</header>
<main>
<h1 class="fade-in">Situation d'apprentissage</h1>
<p class="fade-in">Analyse et réflexion</p>
</main>
<script src="js/script.js"></script>
</body>
</html>
