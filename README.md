<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Melanie Dunkel - Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://use.typekit.net/uwc8cyo.css">
  <style>
    /* Grundkonfiguration */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Poppins', sans-serif;
    min-height: 100vh;
    display: flex;
    flex-direction: column; 
    overflow: hidden;
}

.main-header {
    width: 100%;
    padding: 30px 7%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0;
    z-index: 100;
}

.nav-menu ul {
    display: flex;
    list-style: none;
    gap: 40px;
}

.nav-menu a {
    text-decoration: none;
    color: #333;
    text-transform: uppercase;
    font-size: 14px;
    letter-spacing: 2px;
    transition: color 0.3s;
}

.nav-menu a:hover {
    color: #cbd1c5;
}

/* --- Container Anpassung --- */
.container {
    position: relative;
    width: 100%;
    padding: 0 7%;
    display: flex;
    align-items: center;
}

.sidebar-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
}

.pink-line {
    width: 2px;
    height: 350px;
    background-color: #f7dcd0;
    margin: 120px 0 20px 0;
}

.sidebar-text {
    writing-mode: vertical-rl;
    transform: rotate(180deg);
    font-size: 30px;
    letter-spacing: 2px;
    text-transform: uppercase;
    font-weight: lighter;
}

/* Hauptinhalt */
.content {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    padding-left: 100px; 
    padding-top: 100px;
}

.text-group {
    z-index: 2;
    margin-right: -80px;
}

.name {
    font-size: 30px;
    font-weight: lighter;
    letter-spacing: 10px;
    margin-bottom: 30px;
}

.title {
    font-family: 'the-seasons', serif;
    font-size: 150px;
    line-height: 0.85;
    font-weight: 400;
    display: block;
}

/* Bild-Kreis */
.image-container {
    width: 500px;
    height: 500px;
    border-radius: 50%;
    overflow: hidden;
    z-index: 1;
}

.image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Farbpalette */
.color-palette {
    position: absolute;
    right: 7%;
    bottom: 1px;
    display: flex;
}

.dot {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    margin-left: -15px;
    border: 2px solid #fff;
}

.dot-1 { background-color: #cbd1c5; z-index: 1; }
.dot-2 { background-color: #e9ede4; z-index: 2; }
.dot-3 { background-color: #f7dcd0; z-index: 3; }
.dot-4 { background-color: #f2f1ed; z-index: 4; }

@media (max-width: 1024px) {
    .main-header { padding: 20px; }
    .nav-menu { display: none; } /* Menü auf Handy ausblenden oder Burger-Icon nutzen */
    .content { flex-direction: column; padding-left: 0; }
    .text-group { margin-right: 0; margin-bottom: 20px; text-align: center; }
    .title .italic { margin-left: 0; }
    .image-container { width: 300px; height: 300px; }
}
  </style>
</head>
<body>

    <header class="main-header">
        <div class="logo"><img src="logo.png" alt="Logo"></div>
        <nav class="nav-menu">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#projekte">Projekte</a></li>
                <li><a href="#ueber-mich">Über mich</a></li>
                <li><a href="#kontakt">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <div class="container">
        <aside class="sidebar-container">
            <div class="pink-line"></div>
            <div class="sidebar-text">Meine Arbeiten 2023-2026</div>
        </aside>

        <main class="content">
            <div class="text-group">
                <h2 class="name">MELANIE DUNKEL</h2>
                <h1 class="title">
                    Kreatives<br>
                    <span>Port<i>folio</i></span>
                </h1>
            </div>

            <div class="image-container">
                <img src="signatur.jpg" alt="Melanie Dunkel">
            </div>
        </main>

        <footer class="color-palette">
            <div class="dot dot-1"></div>
            <div class="dot dot-2"></div>
            <div class="dot dot-3"></div>
            <div class="dot dot-4"></div>
        </footer>
    </div>

</body>
</html>
