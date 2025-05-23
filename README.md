<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>California Dream Travel</title>
  <style>
    /* Reset e básico */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      background: #f5f9fc;
      color: #333;
      line-height: 1.6;
    }
    header {
      background: linear-gradient(90deg, #0052d4, #4364f7, #6fb1fc);
      color: white;
      padding: 20px 0;
      text-align: center;
      box-shadow: 0 4px 10px rgba(0,0,0,0.15);
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 5px;
      font-weight: 700;
    }
    header p {
      font-size: 1.2rem;
      font-style: italic;
      font-weight: 300;
    }
    nav {
      margin-top: 15px;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #ff865c;
    }
    main {
      max-width: 1100px;
      margin: 30px auto;
      padding: 0 20px;
    }
    section {
      margin-bottom: 50px;
    }
    h2 {
      color: #0052d4;
      margin-bottom: 15px;
      font-size: 2rem;
      border-bottom: 3px solid #ff865c;
      display: inline-block;
      padding-bottom: 5px;
    }
    /* Home banner */
    #home-banner {
      background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1400&q=80') no-repeat center/cover;
      height: 400px;
      border-radius: 10px;
      color: white;
      display: flex;
      flex-direction: column;
      justify-content: center;
      text-align: center;
      padding: 0 20px;
      box-shadow: inset 0 0 50px rgba(0,0,0,0.5);
      margin-bottom: 40px;
    }
    #home-banner h2 {
      font-size: 3rem;
      margin-bottom: 10px;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.7);
    }
    #home-banner p {
      font-size: 1.5rem;
      font-weight: 300;
      text-shadow: 1px 1px 6px rgba(0,0,0,0.6);
    }
    /* Destinos grid */
    #destinos-list {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
      gap: 25px;
    }
    .destino-card {
      background: white;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s ease;
      cursor: pointer;
    }
    .destino-card:hover {
      transform: scale(1.05);
    }
    .destino-card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }
    .destino-card h3 {
      margin: 15px;
      color: #0052d4;
      font-size: 1.5rem;
    }
    .destino-card p {
      margin: 0 15px 15px 15px;
      color: #555;
      font-size: 1rem;
    }
    /* Sobre */
    #sobre p {
      max-width: 800px;
      margin: 0 auto;
      font-size: 1.1rem;
      color: #444;
      line-height: 1.7;
    }
    /* Contato */
    #contato {
      text-align: center;
    }
    #contato p {
      margin-bottom: 10px;
      font-size: 1.2rem;
    }
    #contato a {
      display: inline-block;
      margin: 0 10px;
      color: #0052d4;
      text-decoration: none;
      font-weight: 600;
      border-bottom: 2px solid transparent;
      transition: border-color 0.3s ease;
    }
    #contato a:hover {
      border-color: #ff865c;
    }
    /* Orçamento */
    form {
      max-width: 600px;
      margin: 0 auto;
      background: white;
      padding: 25px 30px;
      border-radius: 10px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
    }
    form label {
      display: block;
      margin-bottom: 7px;
      font-weight: 600;
      color: #0052d4;
    }
    form input, form select {
      width: 100%;
      padding: 10px;
      margin-bottom: 20px;
      border-radius: 5px;
      border: 1px solid #ccc;
      font-size: 1rem;
      transition: border-color 0.3s ease;
    }
    form input:focus, form select:focus {
      border-color: #ff865c;
      outline: none;
    }
    form button {
      background: #ff865c;
      color: white;
      border: none;
      padding: 12px 25px;
      font-size: 1.1rem;
      font-weight: 700;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    form button:hover {
      background: #e05f3c;
    }
    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background: #0052d4;
      color: white;
      margin-top: 40px;
      font-size: 1rem;
    }
    /* Responsive */
    @media (max-width: 600px) {
      header h1 {
        font-size: 1.8rem;
      }
      #home-banner h2 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>California Dream Travel</h1>
    <p>Turning your dreams into destinations</p>
    <nav>
      <a href="#home">Home</a>
      <a href="#destinos">Destinos</a>
      <a href="#sobre">Sobre Nós</a>
      <a href="#contato">Contato</a>
      <a href="#orcamento">Orçamento</a>
    </nav>
  </header>

  <main>
    <section id="home">
      <div id="home-banner">
        <h2>Explore o mundo conosco</h2>
        <p>Viagens nacionais e internacionais com conforto e segurança</p>
      </div>
    </section>

    <section id="destinos">
      <h2>Destinos em Destaque</h2>
      <div id="destinos-list">
        <div class="destino-card">
          <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=60" alt="Califórnia" />
          <h3>Califórnia</h3>
          <p>San Francisco, Los Angeles, San Diego - Cultura e praias incríveis</p>
        </div>
        <div class="destino-card">
          <img src="https://images.unsplash.com/photo-1526483360025-f4e29f5f48d0?auto=format&fit=crop&w=800&q=60" alt="Las Vegas" />
          <h3>Las Vegas</h3>
          <p>Vida noturna e entretenimento para todas as idades</p>
        </div>
        <div class="destino-card">
          <img src="https://images.unsplash.com/photo-1508898578281-774ac4893a3b?auto=format&fit=crop&w=800&q=60" alt="Orlando" />
          <h3>Orlando</h3>
          <p>Disney, Universal Studios e muita magia</p>
        </div>
        <div class="destino-card">
          <img src="https://images.unsplash.com/photo-1502602898657-3e91760cbb34?auto=format&fit=crop&w=800&q=60" alt="Paris" />
          <h3>Paris</h3>
          <p>Romance, gastronomia e cultura europeia</p>
        </div>
        <div class="destino-card">
          <img src="https://images.unsplash.com/photo-1494526585095-c41746248156?auto=format&fit=crop&w=800&q=60" alt="Tóquio" />
          <h3>Tóquio</h3>
          <p>Tecnologia avançada e tradições milenares</p>
        </div>
      </div>
    </section>

    <section id="sobre">
      <h2>Sobre Nós</h2>
      <p>
        A California Dream Travel nasceu com o sonho de levar você para os destinos mais incríveis do mundo. Com sede na Califórnia, oferecemos viagens nacionais e internacionais com atendimento personalizado, segurança e os melhores preços do mercado. Nossa missão é transformar sonhos em destinos inesquecíveis!
      </p>
    </section>

    <section id="contato">
      <h2>Contato</h2>
      <p>Fale conosco via WhatsApp: <a href="https://wa.me/15551234567" target="_blank">+1 (555) 123-4567</a></p>
      <p>Email: contato@californiadreamtravel.com</p>
      <p>Filial: 123 Sunset Blvd, Los Angeles, CA</p>
      <p>
        Siga-nos:  
        <a href="https://instagram.com/californiadreamtravel" target="_blank">Instagram</a> |  
        <a href="https://facebook.com/californiadreamtravel" target="_blank">Facebook</a> |  
        <a href="https://tiktok.com/@californiadreamtravel" target="_blank">TikTok</a>
      </p>
    </section>

    <section id="orcamento">
      <h2>Solicite seu Orçamento</h2>
      <form id="form-orcamento">
        <label for="nome">Nome Completo:</label>
        <input type="text" id="nome" name="nome" required />

        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required />

        <label for="destino">Destino:</label>
        <select id="destino" name="destino" required>
          <option value="">Selecione</option>
          <option value="california">Califórnia</option>
          <option value="lasvegas">Las Vegas</option>
          <option value="orlando">Orlando</option>
          <option value="paris">Paris</option>
          <option value="tokyo">Tóquio</option>
          <option value="maldivas">Maldivas</option>
          <option value="dubai">Dubai</option>
          <option value="nova-york">Nova York</option>
          <
