<!DOCTYPE html>
<html lang="cs">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kadeřnický salon</title>
  <script src="Java.js" defer></script>
  <link rel="stylesheet" href="style.css">
  <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
</head>
<body>


    
  <header class="header">
    <nav class="navbar">
      
        <a class="logo" href="Filip.html">
            <img src="logo1.png" alt="logo" width="100" height="100">
        </a>
      

      <ul class="nav-menu">
        <li><a href="#onas">O nás</a></li>
        <li><a href="#sluzby">Služby</a></li>
        <li><a href="#ukazky">Ukázky naší práce</a></li>
        <li><a href="#kontakt">Kontakt</a></li>
        <li><a href="#recenze">Recenze</a></li>
      </ul>

    <a class="socialni-link" href="https://www.instagram.com/" target="_blank" >
  <img src="ig_logo.png" alt="logo" width="50" height="50">
    </a>
    </nav>
  </header>





  <main>
    <section class="hero" id="hero">
      <div class="overlay"></div>
      <div class="hero-content">
        <h1>Kadeřnický salon</h1>
        <p>Toto je Kadeřnický salon.</p>

        <div class="hero-buttons">
          <a href="#kontakt" class="btn btn-primarni">Objednat termín</a>
          <a href="#sluzby" class="btn btn-sekundarni">Naše služby</a>
        </div>
      </div>

  </main>



<section id="ukazky" class="section">
  <h2>Ukázky naší práce</h2>

  <div class="galerie-obrazky">
    <div class="gallery">
      <img src="pic4.png" alt="Barvení vlasů" >
      <p onclick="showImage('pic4.png', 'Barvení vlasů')">Barvení vlasů</p>
    </div>

    <div class="gallery">
      <img src="pic3.png" alt="Střih1" >
      <p onclick="showImage('pic3.png', 'Barvení vlasů')">Moderní pánský střih</p>
    </div>

    <div class="gallery">
      <img src="pic2.png" alt="Střih2" >
      <p onclick="showImage('pic2.png', 'Barvení vlasů')">Dámský střih</p>
    </div>
  </div>
</section>




<div id="galerie-modal" class="modal" onclick="this.style.display='none'">
  <span class="close" onclick="closeModal()">×</span>
  <div class="modal-content" onclick="event.stopPropagation()">
    <img id="galerie-img" alt="">
    <p id="galerie-popisek"></p>
  </div>
</div>


<section id="onas" class="section">
  <h2>O nás</h2>
</section>

<section id="sluzby" class="section">
  <h2>Služby</h2>
  <div class="sluzby">
    </div>

</section>


<section id="kontakt" class="section">
  <h2>Kontakt</h2><br>
  <div class="kontakty">
      
    <div class="obrazek">
      <img src="https://static.tildacdn.net/tild3861-3261-4665-b339-303633386164/where.svg" alt="">
      <a href="https://mapy.com/cs/turisticka?source=addr&id=12805112&ds=1&x=14.3019408&y=50.0471628&z=17" target="_blank" >
      <p>Svitákova 2818/9 Praha 15500</p>
      </a>
    </div>

    <div class="obrazek">
      <img src="https://static.tildacdn.net/tild3633-6437-4865-a565-656632366365/when.svg" alt="">
      <p>Pondělí - Sobota 9:00 - 20:00 </p>
    </div>

    <div class="obrazek">
      <img src="https://static.tildacdn.net/tild6135-6336-4636-a261-646638346261/call.svg" alt="">
      <p>+420 771 168 967</p>
    </div>

  </div>
</section>

<section id="recenze" class="section">
  <h2>Recenze</h2>

  <form method="POST" class="recenze-form">
    <input type="text" name="jmeno" placeholder="Vaše jméno" required><br><br>
    <input type="email" name="email" placeholder="Váš email" required><br><br>
    <textarea name="recenze" placeholder="Vaše recenze" required></textarea><br><br>
    <button type="submit" name="odeslat">Odeslat</button>
  </form>
  
  <div class="recenze-vypis">
    <?php include "recenze.php"; ?>
  </div>

</section>
</body>
</html>


