<!DOCTYPE html>
<html lang="hu">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Grotta Di Pasta - Fine Italian Dining</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&display=swap" rel="stylesheet">
  <style>
    html {
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: 'Playfair Display', serif;
      background-color: #0d0d0d;
      color: #f5f5f5;
      line-height: 1.6;
    }
    header {
      background: url('pizza-header.jpg') center/cover no-repeat;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #fff;
      border-bottom: 5px solid #e0c77e;
      animation: fadeIn 2s ease-in;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    header h1 {
      font-size: 64px;
      margin: 0;
      text-shadow: 0 2px 10px rgba(0,0,0,0.7);
      letter-spacing: 2px;
    }
    header p {
      font-size: 24px;
      font-style: italic;
      margin-top: 10px;
      color: #e0c77e;
    }
    nav {
      background: #000;
      padding: 15px;
      display: flex;
      justify-content: center;
      gap: 30px;
      font-size: 18px;
      border-top: 2px solid #e0c77e;
      border-bottom: 2px solid #e0c77e;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav a {
      text-decoration: none;
      color: #fff;
      transition: color 0.3s, transform 0.3s;
    }
    nav a:hover {
      color: #e0c77e;
      transform: scale(1.1);
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
      opacity: 0;
      transform: translateY(40px);
      transition: all 1s ease;
    }
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    h2 {
      text-align: center;
      font-size: 36px;
      color: #e0c77e;
      margin-bottom: 40px;
      border-bottom: 1px solid #e0c77e;
      display: inline-block;
    }
    .menu {
      background: #222;
      padding: 20px;
      border-radius: 8px;
      margin-bottom: 40px;
    }
    .menu h3 {
      color: #e0c77e;
      border-bottom: 1px solid #e0c77e;
      margin-top: 20px;
    }
    .menu ul {
      list-style: none;
      padding: 0;
    }
    .menu li {
      padding: 5px 0;
      border-bottom: 1px dotted #555;
      display: flex;
      justify-content: space-between;
    }
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
    }
    .gallery img {
      width: 300px;
      border-radius: 8px;
      transition: transform 0.5s, box-shadow 0.5s;
    }
    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 20px rgba(0,0,0,0.5);
    }
    footer {
      background: #000;
      color: #999;
      text-align: center;
      padding: 30px;
      font-size: 14px;
      border-top: 2px solid #e0c77e;
    }
    .contact p {
      margin: 5px 0;
    }
    @media (max-width: 600px) {
      header h1 { font-size: 32px; }
      .gallery img { width: 100%; }
      nav { flex-wrap: wrap; gap: 10px; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Grotta Di Pasta</h1>
    <p>Családias olasz étterem és pizzéria</p>
  </header>

  <nav>
    <a href="#about">Rólunk</a>
    <a href="#menu">Étlap</a>
    <a href="#drinks">Itallap</a>
    <a href="#gallery">Galéria</a>
    <a href="#contact">Kapcsolat</a>
  </nav>

  <section id="about">
    <h2>Rólunk</h2>
    <p style="text-align: center; font-size: 20px; max-width: 800px; margin: auto;">
      A <strong>Grotta Di Pasta</strong> Étterem és Pizzéria családi vállalkozásként 2023 novemberében nyitott meg. Várunk minden éhes és szomjas vendéget házias, friss tészta- és pizzakülönlegességekkel, barátságos, családias hangulatban Bocskaikert szívében.
    </p>
    <ul style="margin-top: 20px;">
      <li>22+12 férőhelyes belső tér + terasz</li>
      <li>Gyermekbarát</li>
      <li>Helyben fogyasztás és elvitel</li>
      <li>Készpénzes és kártyás fizetés</li>
      <li>Parkolás a közelben</li>
      <li>Zártkörű rendezvények megegyezés szerint</li>
    </ul>
  </section>

  <section id="menu">
    <h2>Étlap</h2>
    <div class="menu">
      <h3>Pizzák</h3>
      <ul>
        <li>Nápolyi<span>2500 Ft</span></li>
        <li>Kolbászos<span>2500 Ft</span></li>
        <li>Szalámis<span>2500 Ft</span></li>
        <li>Sonkás<span>2500 Ft</span></li>
        <li>Négy évszak<span>2700 Ft</span></li>
        <li>Tonhalas<span>2700 Ft</span></li>
        <li>Mexikói<span>2600 Ft</span></li>
        <li>Gombás<span>2600 Ft</span></li>
        <li>Hawaii<span>2600 Ft</span></li>
        <li>Magyaros<span>2800 Ft</span></li>
        <li>Plusz Feltétel<span>300 Ft</span></li>
      </ul>
      <h3>Frissensültek</h3>
      <ul>
        <li>Marha Steak<span>2000 Ft</span></li>
        <li>Sertés Steak<span>1300 Ft</span></li>
        <li>Csirkecomb egész<span>1200 Ft</span></li>
      </ul>
      <h3>Sültek</h3>
      <ul>
        <li>Rántott Sertéstarja <span>2200 Ft</span></li>
        <li>Rántott Csirkeszárnyak 3-3db <span>1400 Ft</span></li>
        <li>Rántott Csirkemellfilé <span> 1400 Ft</span></li>
      </ul>
      <h3>Tészták</h3>
      <ul>
        <li>Ravioli <span>2200 Ft</span></li>
        <li>Túrós csusza tejföllel és pirított szalonnával <span>2100 Ft</span></li>
        <li>Káposztás kocka <span>2000 Ft</span></li>
        <li>Váradi sonkás tészta <span>2500 Ft</span></li>
        <li>Carbonara <span>2000 Ft</span></li>
        <li>Bolognai <span>2000 Ft</span></li>
        <li>Milánói <span>2000 Ft</span></li>
        <li>Krumplis tészta <span>2000 Ft</span></li>
        <li>Piszkos tészta (prézli, sárgabaracklekvár) <span>2000 Ft</span></li>
        <li>Pesztós-tejszines tészta<span>2000 Ft</span></li>
        <li>Diós metélt <span> 2000 Ft</span></li>
        <li>Mákos metélt <span> 2000 Ft</span></li>
      </ul>
      <h3>Öntetek</h3>
      <ul>
        <li>Ketchup, Mustár, Majonéz <span>200 Ft</span></li>
        <li>Tartár Mártás <span>400 Ft</span></li>
        <li>Csípős szósz Gyroshoz <span>200 Ft</span></li>
      </ul>
      <h3>Street Food</h3>
      <ul>
        <li>Hamburger <span>2500 Ft</span></li>
        <li>Gyros hasábburgonyával <span>2850 Ft</span></li>
        <li>Mics <span> 550Ft/db</span></li>
        <li>Rántott sajt hasábburgonyával és tartár mártással <span>3000 Ft</span></li>
      </ul>
      <h3>Köretek</h3>
      <ul>
        <li>Hasábburgonya <span>900 Ft</span></li>
        <li>Párolt rízs <span>780 Ft</span></li>
        <li>Rizi-bizi <span>900 Ft</span></li>
        <li>Burgonyasaláta (min. 48 órás előrendeléssel) <span>1200 Ft</span></li>
      </ul>
      <h3>Saláták</h3>
      <ul>
        <li>Friss káposztasaláta <span>750 Ft</span></li>
        <li>Friss uborkasaláta <span>750 Ft</span></li>
        <li>Savanyú uborka <span>750 Ft</span></li>
      </ul>
      <h3>Csomagolás</h3>
      <ul>
        <li>Pizzás doboz <span>250 Ft</span></li>
        <li>Műanyag doboz <span>200 Ft</span></li>
        <li>Szatyor <span>50 Ft</span></li>
      </ul>
    </div>
  </section>

  <section id="drinks">
    <h2>Itallap</h2>
    <div class="menu">
      <h3>Sörök</h3>
      <ul>
        <li>Csapolt 5dl <span>1000 Ft</span></li>
        <li>Dreher citrom üveges 0,33L 0% <span>360 Ft</span></li>
        <li>Dreher meggy-szeder üveges 0,33L 0% <span>410 Ft</span></li>
        <li>Kőbányai világos üveges 0,5L 4,3% <span>570 Ft</span></li>
        <li>Peroni üveges 0,33L 5% <span>750 Ft</span></li>
        <li>Heineken dobozos 0,33L 5% <span>410 Ft</span></li>
      </ul>
      <h3>Borok</h3>
      <ul>
        <li>Fehér / Vörös / Rosé <span>690 Ft/dl</span></li>
      </ul>
      <h3>Rövid italok</h3>
      <ul>
        <li>Havanna Club Kubai rum 40% <span>1250 Ft/4cl</span></li>
        <li>Jägermeister 35% <span>1250 Ft/4cl</span></li>
        <li>Kalinka vodka 37,5% <span>980 Ft/4cl</span></li>
        <li>Martini <span>800 Ft/1dl</span></li>
        <li>Metaxa <span>1400 Ft/4cl</span></li>
        <li>Whisky <span>1100 Ft/4cl</span></li>
      </ul>
      <h3>Kávék</h3>
      <ul>
        <li>Eszpresszó <span>590 Ft</span></li>
        <li>Cappuccino <span>790 Ft</span></li>
      </ul>
      <h3>Üdítők</h3>
      <ul>
        <li>Pepsi dobozos 0,33l <span>400 Ft</span></li>
        <li>Coca-Cola, Fanta, Sprite dobozos 0,33l <span>450 Ft</span></li>
        <li>Palackos Coca-Cola, Zero, Sprite, Fanta, Ginger, Tonic 0,5l <span>800 Ft</span></li>
      </ul>
      <h3>Gyümölcslevek</h3>
      <ul>
        <li>Cappy (alma, eper, barack, multivitamin, narancs) <span>550 Ft</span></li>
      </ul>
      <h3>Ásványvíz</h3>
      <ul>
        <li>Natur Aqua (enyhe, dús, mentes) <span>350 Ft</span></li>
      </ul>
    </div>
  </section>

  <section id="gallery">
    <h2>Galéria</h2>
    <div class="gallery">
      <img src="mics.jpg" alt="Mics">
      <img src="terasz.jpg" alt="Terasz">
      <img src="saslik.jpg" alt="Saslik">
    </div>
  </section>

  <section id="contact">
    <h2>Kapcsolat</h2>
    <p style="text-align: center;">
      📞 +36 20 931 3291 <br />
      📍 4241 Bocskaikert, Debreceni út 25/A <br />
    </p>
  </section>

  <footer>
    &copy; 2025 Grotta Di Pasta | Minden jog fenntartva.
  </footer>

  <script>
    // scroll-based reveal
    const sections = document.querySelectorAll("section");
    window.addEventListener("scroll", () => {
      sections.forEach(sec => {
        const top = sec.getBoundingClientRect().top;
        if (top < window.innerHeight - 100) {
          sec.classList.add("visible");
        }
      });
    });
  </script>
</body>
</html>


