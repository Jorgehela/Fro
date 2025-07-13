<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>It’s not Froxx - Música Oficial</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap');

    /* Reset */
    *, *::before, *::after {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      font-family: 'Poppins', sans-serif;
      color: #e0f7f4;
      scroll-behavior: smooth;
      line-height: 1.5;
    }

    header {
      position: fixed;
      top: 0;
      left: 0; right: 0;
      background: rgba(15,32,39,0.95);
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.7);
    }

    header h1 {
      font-weight: 700;
      font-size: 1.5rem;
      color: #5fffdc;
      letter-spacing: 2px;
      margin: 0;
    }

    nav a {
      color: #a7fff3;
      text-decoration: none;
      font-weight: 600;
      margin-left: 25px;
      transition: color 0.3s ease;
      font-size: 1rem;
      text-transform: uppercase;
      letter-spacing: 1.2px;
    }

    nav a:hover {
      color: #00ffe7;
      text-shadow: 0 0 8px #00ffe7;
    }

    main {
      max-width: 960px;
      margin: 100px auto 60px;
      padding: 0 20px;
    }

    section {
      margin-bottom: 60px;
      opacity: 0;
      transform: translateY(40px);
      animation: fadeInUp 0.8s forwards;
    }
    section:nth-child(1) { animation-delay: 0.2s; }
    section:nth-child(2) { animation-delay: 0.4s; }
    section:nth-child(3) { animation-delay: 0.6s; }
    section:nth-child(4) { animation-delay: 0.8s; }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h2 {
      text-align: center;
      font-size: 2rem;
      font-weight: 700;
      margin-bottom: 30px;
      color: #00fff7;
      text-shadow: 0 0 10px #00fff7;
      letter-spacing: 1.5px;
    }

    /* Música */
    .canciones {
      display: grid;
      grid-template-columns: repeat(auto-fill,minmax(280px,1fr));
      gap: 28px;
    }

    .cancion {
      background: rgba(255,255,255,0.05);
      border-radius: 14px;
      padding: 20px;
      box-shadow: 0 0 18px #00fff7aa;
      display: flex;
      flex-direction: column;
      align-items: center;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
    }
    .cancion:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 30px #00fff7cc;
    }
    .cancion img {
      width: 100%;
      border-radius: 12px;
      margin-bottom: 18px;
      box-shadow: 0 0 15px #00fff7bb;
    }
    .cancion h3 {
      margin: 0 0 12px;
      font-size: 1.3rem;
      color: #7afff9;
      text-align: center;
      text-shadow: 0 0 10px #00fff7;
    }
    .cancion audio {
      width: 100%;
      border-radius: 12px;
      outline: none;
      background: #022;
      box-shadow: inset 0 0 10px #00fff7aa;
      margin-bottom: 10px;
    }
    .cancion a {
      color: #00fff7;
      font-weight: 700;
      text-decoration: none;
      text-align: center;
      font-size: 0.9rem;
      transition: text-decoration 0.3s ease;
    }
    .cancion a:hover {
      text-decoration: underline;
    }

    /* Videos */
    .videos {
      display: flex;
      flex-wrap: wrap;
      gap: 30px;
      justify-content: center;
    }
    .videos iframe {
      border-radius: 16px;
      width: 320px;
      height: 180px;
      box-shadow: 0 0 20px #00fff7bb;
      transition: transform 0.3s ease;
    }
    .videos iframe:hover {
      transform: scale(1.05);
    }

    /* Biografía */
    .bio p {
      max-width: 720px;
      margin: 0 auto;
      font-size: 1.1rem;
      line-height: 1.7;
      text-align: center;
      color: #9efaff;
      text-shadow: 0 0 8px #00fff7bb;
    }

    /* Contacto */
    .contacto {
      text-align: center;
      font-size: 1rem;
      margin-top: 10px;
      color: #8ff8ff;
      letter-spacing: 1px;
    }
    .contacto p {
      margin: 10px 0;
    }
    .contacto a {
      color: #00fff7;
      font-weight: 700;
      text-decoration: none;
      transition: color 0.3s ease;
    }
    .contacto a:hover {
      color: #33fff9;
      text-shadow: 0 0 10px #33fff9;
    }

    footer {
      text-align: center;
      margin: 40px 0 20px;
      color: #333;
      font-size: 0.9rem;
    }

    @media (max-width: 680px) {
      .videos iframe {
        width: 90vw;
        height: 50vw;
      }
    }

  </style>
</head>
<body>

<header>
  <h1>It’s not Froxx</h1>
  <nav>
    <a href="#musica">Música</a>
    <a href="#videos">Videos</a>
    <a href="#bio">Bio</a>
    <a href="#contacto">Contacto</a>
  </nav>
</header>

<main>
  <section id="musica">
    <h2>Todas mis canciones</h2>
    <div class="canciones">

      <div class="cancion">
        <img src="https://i.scdn.co/image/ab67616d0000b2733d8a8c6d3f9f72aa869d8dff" alt="Sabor a Menta" />
        <h3>Sabor a Menta</h3>
        <audio controls>
          <source src="https://p.scdn.co/mp3-preview/4b937dbd2e4c7b6e4e9a6c1b0516e7aab9c6e52f?cid=YOUR_SPOTIFY_CLIENT_ID" type="audio/mpeg" />
          Tu navegador no soporta audio.
        </audio>
        <a href="https://open.spotify.com/track/2a6r9kw0SWiMEaeQjgoS3v" target="_blank" rel="noopener noreferrer">Escuchar en Spotify</a>
      </div>

      <div class="cancion">
        <img src="https://i.scdn.co/image/ab67616d0000b2736a949f7c6074b1f324476120" alt="Tu Cuerpo" />
        <h3>Tu Cuerpo (feat. Krone, Bela & Toky-0)</h3>
        <audio controls>
          <source src="https://p.scdn.co/mp3-preview/9a432b8e09c2e3e7766ef387deff742854698dd1?cid=YOUR_SPOTIFY_CLIENT_ID" type="audio/mpeg" />
          Tu navegador no soporta audio.
        </audio>
        <a href="https://open.spotify.com/track/3kJkRvzvG0ZlLypTPiqgwp" target="_blank" rel="noopener noreferrer">Escuchar en Spotify</a>
      </div>

      <div class="cancion">
        <img src="https://i.scdn.co/image/ab67616d0000b2739bd47622f50e9de3afdd3069" alt="Dónde Estás?" />
        <h3>Dónde Estás?</h3>
        <audio controls>
          <source src="https://p.scdn.co/mp3-preview/9e8f34ebf4f8fa7a0ff89c34854f2f680e00ff2b?cid=YOUR_SPOTIFY_CLIENT_ID" type="audio/mpeg" />
          Tu navegador no soporta audio.
        </audio>
        <a href="https://open.spotify.com/track/5tXnCEHCmhI9x8rH6MDP5R" target="_blank" rel="noopener noreferrer">Escuchar en Spotify</a>
      </div>

    </div>
  </section>

  <section id="videos">
    <h2>Videos</h2>
    <div class="videos">
      <iframe
        src="https://www.youtube.com/embed/dQw4w9WgXcQ"
        title="Video oficial Sabor a Menta"
        allowfullscreen
      ></iframe>
      <iframe
        src="https://www.youtube.com/embed/3JZ_D3ELwOQ"
        title="Video oficial Tu Cuerpo"
        allowfullscreen
      ></iframe>
    </div>
  </section>

  <section id="bio">
    <h2>Biografía</h2>
    <div class="bio">
      <p>
        It’s not Froxx es un artista que fusiona trap, R&B y sonidos urbanos con una vibra fresca y elegante.
        Su música explora temas de pasión, introspección y las vivencias de la vida nocturna, siempre con un estilo personal y auténtico.
        Con colaboraciones que cruzan fronteras, su proyecto sigue creciendo y ganando seguidores en el mundo del trap latino.
      </p>
    </div>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <div class="contacto">
      <p>Para booking y colaboraciones:</p>
      <p><a href="mailto:contacto@itsnotfroxx.com">contacto@itsnotfroxx.com</a></p>
      <p>Sígueme en redes:</p>
      <p>
        <a href="https://instagram.com/itsnotfroxx" target="_blank" rel="noopener noreferrer">Instagram</a> |
        <a href="https://twitter.com/itsnotfroxx" target="_blank" rel="noopener noreferrer">Twitter</a> |
        <a href="https://youtube.com/itsnotfroxx" target="_blank" rel="noopener noreferrer">YouTube</a>
      </p>
    </div>
  </section>
</main>

<footer>
  &copy; 2025 It’s not Froxx. Todos los derechos reservados.
</footer>

</body>
</html>
