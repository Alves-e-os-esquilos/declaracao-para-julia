<title>Para Júlia 💖</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #fff0f5, #ffe6f0);
      color: #333;
      overflow-x: hidden;
      scroll-behavior: smooth;
    }

    header {
      background-color: #e60073;
      color: white;
      padding: 60px 20px;
      text-align: center;
      animation: fadeIn 2s ease;
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.2rem;
    }

    section {
      max-width: 900px;
      margin: 60px auto;
      padding: 0 20px;
      animation: fadeInUp 2s ease;
    }

    .intro, .motivos, .frases, .galeria, .rodape {
      text-align: center;
    }

    button {
      background-color: #e60073;
      color: white;
      padding: 12px 30px;
      font-size: 1.2rem;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      transition: background 0.3s ease;
      margin-top: 20px;
    }

    button:hover {
      background-color: #cc005f;
    }

    .declaracao {
      display: none;
      margin-top: 40px;
      font-size: 1.2rem;
      white-space: pre-line;
      animation: fadeIn 2s ease;
    }

    .motivos ul {
      list-style: none;
      padding: 0;
      font-size: 1.1rem;
      margin-top: 30px;
    }

    .motivos ul li {
      background: #ffd6e8;
      margin: 10px auto;
      max-width: 600px;
      padding: 12px 20px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      animation: fadeInUp 1s ease forwards;
    }

    .galeria img {
      width: 280px;
      height: 360px;
      object-fit: cover;
      border-radius: 18px;
      margin: 20px;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
      transition: transform 0.3s ease;
    }

    .galeria img:hover {
      transform: scale(1.05);
    }

    .frases p {
      font-style: italic;
      font-size: 1.3rem;
      color: #cc0066;
      margin: 30px 0;
      animation: pulse 4s infinite;
    }

    .rodape {
      padding: 40px 20px;
      background: #ffe6f0;
      font-size: 1rem;
    }

    .hearts {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      overflow: hidden;
      z-index: 0;
    }

    .heart {
      position: absolute;
      color: #ff69b4;
      animation: float 8s infinite ease-in;
      font-size: 24px;
      opacity: 0.6;
    }

    @keyframes float {
      0% { transform: translateY(100vh) scale(1); opacity: 0; }
      50% { opacity: 1; }
      100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes pulse {
      0%, 100% { opacity: 0.8; }
      50% { opacity: 1; }
    }

    .musica {
      text-align: center;
      margin-top: 20px;
    }

    .musica a {
      text-decoration: none;
      color: #e60073;
      font-weight: bold;
      font-size: 1rem;
    }

  </style>
</head>
<body>

  <div class="hearts" id="hearts"></div>

  <header>
    <h1>Para Júlia 💖</h1>
    <p>Uma mensagem feita com carinho, só pra você</p>
  </header>

<section class="intro">
    <p>Tem algo que eu preciso te contar, e guardei isso com muito carinho...</p>
    <button onclick="mostrarDeclaracao()">Clique para começar</button>
    <div class="declaracao" id="declaracao">
      <p>
Júlia,

A gente se aproximou, riu, trocou segredos, histórias...
E cada pedacinho seu foi ficando aqui, no meu coração.

E com o tempo, percebi que era mais do que amizade.
Eu me apaixonei por você.

Foi natural, foi sincero, foi real.
E hoje, eu só queria te contar isso, sem pressa, sem cobrança.

Só queria que você soubesse.

Com carinho,  
Gabriel Alves 💖
      </p>
    </div>
  </section>

  <section class="motivos">
    <h2>Motivos pelos quais eu gosto de você</h2>
    <ul>
      <li>Seu sorriso que ilumina qualquer lugar</li>
      <li>Seu jeito carinhoso de cuidar dos outros</li>
      <li>As conversas que me fazem esquecer do mundo</li>
      <li>O jeito como você é verdadeira, sempre</li>
      <li>Porque com você, tudo é mais leve</li>
    </ul>
  </section>

  <section class="frases">
    <p>“Com você, até o silêncio tem significado.”</p>
  </section>

  <section class="galeria">
    <img src="foto2.jpg" alt="Foto 2">
    <img src="foto5.jpg" alt="Foto 5">
    <img src="foto1.jpg" alt="Foto 1">
    <img src="foto4.jpg" alt="Foto 4">
    <img src="foto6.jpg" alt="Foto 6">
    <img src="foto3.jpg" alt="Foto 3">
  </section>

  <section class="frases">
    <p>“Você me faz querer ser alguém melhor todos os dias.”</p>
    <p>“A vida sorriu pra mim quando colocou você no meu caminho.”</p>
  </section>

  <div class="rodape">
    Feito com 💖 por Gabriel Alves — 2025
  </div>

  <script>
    function mostrarDeclaracao() {
      document.getElementById("declaracao").style.display = "block";
    }

    const hearts = document.getElementById('hearts');
    for (let i = 0; i < 40; i++) {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.innerHTML = '❤';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDelay = Math.random() * 8 + 's';
      heart.style.fontSize = (Math.random() * 20 + 20) + 'px';
      hearts.appendChild(heart);
    }
  </script>

</body>
</html>
<!-- Música: Pupila -->
  <div class="musica">
    <iframe width="0" height="0"
      src="https://www.youtube.com/embed/937mq8wUmRI?autoplay=1&loop=1&playlist=937mq8wUmRI"
      frameborder="0" allow="autoplay">
