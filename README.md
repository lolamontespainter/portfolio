index.html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lola Montes - Artiste</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background-color: #fff;
      color: #333;
      scroll-behavior: smooth;
    }

    /* HEADER FIXE */
    header {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      background-color: #FF7F50;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }

    header h1 {
      margin: 0;
      color: white;
      font-size: 1.8rem;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 1rem;
      font-weight: 600;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #FFD700;
    }

    section {
      padding: 6rem 2rem 4rem 2rem; /* top padding compensé pour header fixe */
    }

    .intro {
      text-align: center;
      background: linear-gradient(135deg, #FFE4B5, #FFDEAD);
    }

    .intro img {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      margin-top: 1rem;
      transition: transform 0.5s;
    }

    .intro img:hover {
      transform: scale(1.05);
    }

    h2 {
      text-align: center;
      margin-bottom: 2rem;
      color: #FF6347;
      font-size: 2rem;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }

    .grid img {
      width: 100%;
      height: auto;
      border-radius: 8px;
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
    }

    .grid img.show {
      opacity: 1;
      transform: translateY(0);
    }

    .portfolio-item, .fresque-item, .shop-item {
      text-align: center;
    }

    .shop-item button {
      margin-top: 0.5rem;
      padding: 0.5rem 1rem;
      border: none;
      background-color: #FF7F50;
      color: white;
      font-weight: bold;
      cursor: pointer;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    .shop-item button:hover {
      background-color: #FF6347;
    }

    form {
      max-width: 500px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
    }

    form input, form textarea {
      margin-bottom: 1rem;
      padding: 0.8rem;
      border-radius: 5px;
      border: 1px solid #ccc;
      font-size: 1rem;
    }

    form button {
      padding: 0.8rem;
      border-radius: 5px;
      border: none;
      background-color: #FF7F50;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }

    form button:hover {
      background-color: #FF6347;
    }

    footer {
      background-color: #333;
      color: white;
      padding: 2rem;
      text-align: center;
    }

    footer a {
      color: #FFA07A;
      text-decoration: none;
      margin: 0 0.5rem;
    }

    /* Responsive text */
    @media (max-width: 768px) {
      header {
        flex-direction: column;
      }
      nav {
        margin-top: 0.5rem;
      }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <h1>Lola Montes</h1>
    <nav>
      <a href="#presentation">Présentation</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#fresques">Fresques participatives</a>
      <a href="#boutique">Boutique</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- PRESENTATION -->
  <section id="presentation" class="intro">
    <h2>Bienvenue dans mon univers</h2>
    <p>Je suis Lola Montes, peintre muraliste et illustratrice. Je crée des fresques murales colorées et participatives ainsi que des illustrations uniques.</p>
    <img src="https://via.placeholder.com/800x400.png?text=Fresque+principale" alt="Fresque principale">
  </section>

  <!-- PORTFOLIO -->
  <section id="portfolio">
    <h2>Portfolio</h2>
    <div class="grid">
      <div class="portfolio-item">
        <img src="https://via.placeholder.com/400x300.png?text=Fresque+1" alt="Fresque 1">
        <p>Fresque murale - Lieu / Description courte</p>
      </div>
      <div class="portfolio-item">
        <img src="https://via.placeholder.com/400x300.png?text=Fresque+2" alt="Fresque 2">
        <p>Fresque murale - Lieu / Description courte</p>
      </div>
      <div class="portfolio-item">
        <img src="https://via.placeholder.com/400x300.png?text=Illustration+1" alt="Illustration 1">
        <p>Illustration originale - Format / Description</p>
      </div>
      <div class="portfolio-item">
        <img src="https://via.placeholder.com/400x300.png?text=Illustration+2" alt="Illustration 2">
        <p>Illustration originale - Format / Description</p>
      </div>
    </div>
  </section>

  <!-- FRESQUES PARTICIPATIVES -->
  <section id="fresques">
    <h2>Fresques participatives</h2>
    <div class="grid">
      <div class="fresque-item">
        <img src="https://via.placeholder.com/400x300.png?text=Fresque+Participative+1" alt="Fresque participative 1">
        <p>Description de la fresque participative</p>
      </div>
      <div class="fresque-item">
        <img src="https://via.placeholder.com/400x300.png?text=Fresque+Participative+2" alt="Fresque participative 2">
        <p>Description de la fresque participative</p>
      </div>
    </div>
  </section>

  <!-- BOUTIQUE -->
  <section id="boutique">
    <h2>Boutique</h2>
    <div class="grid">
      <div class="shop-item">
        <img src="https://via.placeholder.com/400x300.png?text=Illustration+à+Vendre+1" alt="Illustration 1">
        <p>Illustration 1 - 20€</p>
        <button onclick="window.open('https://tonlienbigcartel.com/produit1', '_blank')">Acheter</button>
      </div>
      <div class="shop-item">
        <img src="https://via.placeholder.com/400x300.png?text=Illustration+à+Vendre+2" alt="Illustration 2">
        <p>Illustration 2 - 25€</p>
        <button onclick="window.open('https://tonlienbigcartel.com/produit2', '_blank')">Acheter</button>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Contact</h2>
    <form action="mailto:tonemail@example.com" method="post" enctype="text/plain">
      <input type="text" name="name" placeholder="Nom" required>
      <input type="email" name="email" placeholder="Email" required>
      <textarea name="message" rows="5" placeholder="Votre message" required></textarea>
      <button type="submit">Envoyer</button>
    </form>
    <p style="text-align:center; margin-top:1rem;">Suivez-moi : 
      <a href="https://instagram.com/toncompte" target="_blank">Instagram</a>
    </p>
  </section>

  <!-- FOOTER -->
  <footer>
    &copy; 2025 Lola Montes - Tous droits réservés
  </footer>

  <!-- ANIMATIONS JS -->
  <script>
    // Simple animation au scroll pour les images
    const images = document.querySelectorAll('.grid img');

    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if(entry.isIntersecting) {
          entry.target.classList.add('show');
        }
      });
    }, { threshold: 0.1 });

    images.forEach(img => observer.observe(img));
  </script>

</body>
</html>
