<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Herbalife Bien-Être</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet" />
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f9f9f9;
      color: #333;
      scroll-behavior: smooth;
    }
    header {
      background-color: #fff;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      padding: 20px 40px;
      position: sticky;
      top: 0;
      z-index: 10;
    }
    header h1 {
      margin: 0;
      color: #58b368;
      font-weight: 600;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      margin-right: 20px;
      color: #555;
      text-decoration: none;
      font-weight: 500;
    }
    section {
      padding: 60px 20px;
      max-width: 900px;
      margin: auto;
    }
    .hero {
      text-align: center;
      animation: fadeIn 1.5s ease;
    }
    .hero h2 {
      font-size: 2.5rem;
      color: #58b368;
    }
    .hero p {
      font-size: 1.2rem;
      color: #666;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
      background: #fff;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
      animation: fadeIn 1.5s ease;
    }
    input, textarea {
      padding: 12px;
      font-size: 1rem;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
    button {
      background-color: #58b368;
      color: white;
      border: none;
      padding: 12px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s ease;
    }
    button:hover {
      background-color: #469d59;
    }
    footer {
      background-color: #e6f2ea;
      text-align: center;
      padding: 20px;
      font-size: 0.9rem;
      color: #555;
    }

    /* --- BOUTON RETOUR EN HAUT --- */
    #backToTop {
      position: fixed;
      bottom: 30px;
      right: 30px;
      background-color: #58b368;
      color: white;
      border: none;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      font-size: 20px;
      display: none;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      z-index: 1000;
      transition: opacity 0.3s ease;
    }
    #backToTop:hover {
      background-color: #469d59;
    }
  </style>
</head>
<body>

  <header>
    <h1>Herbalife Bien-Être</h1>
    <nav>
      <a href="#accueil">Accueil</a>
      <a href="#contact">Contact</a>
      <a href="#participation">Participer</a>
    </nav>
  </header>

  <section class="hero" id="accueil">
    <h2>Transforme ton mode de vie</h2>
    <p>Découvre comment Herbalife peut t'aider à atteindre tes objectifs de bien-être et de nutrition.</p>
  </section>

  <section id="apropos">
    <h2>À propos de moi</h2>
    <p>Coach bien-être certifiée, je t'accompagne avec les produits Herbalife dans ton parcours vers une meilleure forme physique, plus d'énergie et un équilibre nutritionnel optimal.</p>
  </section>

  <section id="contact">
    <h2>Contacte-moi</h2>
    <form>
      <input type="text" placeholder="Nom" required />
      <input type="email" placeholder="Email" required />
      <textarea rows="4" placeholder="Ton message" required></textarea>
      <button type="submit">Envoyer</button>
    </form>
  </section>

  <section id="participation">
    <h2>Participe à mon programme Herbalife</h2>
    <form>
      <input type="text" placeholder="Prénom" required />
      <input type="text" placeholder="Nom" required />
      <input type="email" placeholder="Email" required />
      <textarea rows="4" placeholder="Quel est ton objectif ?" required></textarea>
      <button type="submit">Je m’inscris</button>
    </form>
  </section>

  <footer>
    © 2025 Herbalife Bien-Être · Coach indépendant<br />
    Site réalisé avec ❤️
  </footer>

  <!-- Bouton retour en haut -->
  <button id="backToTop" title="Retour en haut">↑</button>

  <script>
    const backToTop = document.getElementById("backToTop");

    window.onscroll = () => {
      if (document.body.scrollTop > 300 || document.documentElement.scrollTop > 300) {
        backToTop.style.display = "flex";
      } else {
        backToTop.style.display = "none";
      }
    };

    backToTop.addEventListener("click", () => {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    });
  </script>

</body>
</html>
