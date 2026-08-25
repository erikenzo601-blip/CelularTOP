# CelularTOP
Ranking de celulares com foco em desempenho, câmera, bateria e custo-benefício
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>CelularTOP — Ranking de Celulares</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #0b0f19;
      color: white;
    }

    header {
      background: #111827;
      padding: 18px 6%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #1f2937;
    }

    .logo {
      font-size: 24px;
      font-weight: bold;
    }

    .logo span {
      color: #4f8cff;
    }

    nav a {
      color: #aaa;
      text-decoration: none;
      margin-left: 20px;
    }

    nav a:hover {
      color: white;
    }

    .hero {
      text-align: center;
      padding: 70px 20px 50px;
    }

    .hero h1 {
      font-size: 42px;
      margin-bottom: 15px;
    }

    .hero h1 span {
      color: #4f8cff;
    }

    .hero p {
      color: #9ca3af;
      font-size: 18px;
      max-width: 650px;
      margin: auto;
    }

    .search {
      margin: 30px auto;
      max-width: 600px;
      display: flex;
    }

    .search input {
      width: 100%;
      padding: 15px;
      border: 1px solid #374151;
      border-radius: 10px;
      background: #111827;
      color: white;
      outline: none;
      font-size: 16px;
    }

    .section {
      padding: 30px 6%;
    }

    .section h2 {
      margin-bottom: 25px;
      font-size: 28px;
    }

    .phones {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
      gap: 20px;
    }

    .card {
      background: #111827;
      border: 1px solid #1f2937;
      border-radius: 16px;
      padding: 20px;
      transition: 0.2s;
    }

    .card:hover {
      transform: translateY(-5px);
      border-color: #4f8cff;
    }

    .phone-image {
      height: 180px;
      background: #1f2937;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 18px;
      color: #6b7280;
    }

    .card h3 {
      font-size: 20px;
      margin-bottom: 10px;
    }

    .score {
      font-size: 25px;
      font-weight: bold;
      color: #4f8cff;
      margin: 10px 0;
    }

    .info {
      color: #9ca3af;
      line-height: 1.8;
      font-size: 14px;
    }

    .button {
      display: block;
      text-align: center;
      background: #4f8cff;
      color: white;
      padding: 12px;
      margin-top: 15px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
    }

    .button:hover {
      background: #3978e8;
    }

    footer {
      margin-top: 50px;
      padding: 30px;
      text-align: center;
      background: #111827;
      color: #6b7280;
    }

    @media (max-width: 600px) {
      header {
        flex-direction: column;
        gap: 15px;
      }

      nav a {
        margin: 0 8px;
      }

      .hero h1 {
        font-size: 32px;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">
      Celular<span>TOP</span>
    </div>

    <nav>
      <a href="#">Início</a>
      <a href="#ranking">Ranking</a>
      <a href="#sobre">Sobre</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Encontre o celular <span>TOP</span></h1>

    <p>
      Compare celulares por desempenho, câmera, bateria e custo-benefício.
    </p>

    <div class="search">
      <input
        type="text"
        id="search"
        placeholder="Pesquisar celular..."
        onkeyup="pesquisarCelular()"
      >
    </div>
  </section>

  <section class="section" id="ranking">

    <h2>🔥 Ranking de celulares</h2>

    <div class="phones" id="listaCelulares">

      <div class="card" data-name="Galaxy A15">
        <div class="phone-image">
          📱 Galaxy A15
        </div>

        <h3>Galaxy A15</h3>

        <div class="score">8.5/10</div>

        <div class="info">
          ⚡ Desempenho: 8/10<br>
          📸 Câmera: 8/10<br>
          🔋 Bateria: 9/10<br>
          💰 Custo-benefício: 9/10
        </div>

        <a href="#" class="button">Ver detalhes</a>
      </div>


      <div class="card" data-name="Redmi Note 13">
        <div class="phone-image">
          📱 Redmi Note 13
        </div>

        <h3>Redmi Note 13</h3>

        <div class="score">8.8/10</div>

        <div class="info">
          ⚡ Desempenho: 9/10<br>
          📸 Câmera: 8/10<br>
          🔋 Bateria: 9/10<br>
          💰 Custo-benefício: 9/10
        </div>

        <a href="#" class="button">Ver detalhes</a>
      </div>


      <div class="card" data-name="Moto G54">
        <div class="phone-image">
          📱 Moto G54
        </div>

        <h3>Moto G54</h3>

        <div class="score">8.7/10</div>

        <div class="info">
          ⚡ Desempenho: 9/10<br>
          📸 Câmera: 8/10<br>
          🔋 Bateria: 9/10<br>
          💰 Custo-benefício: 9/10
        </div>

        <a href="#" class="button">Ver detalhes</a>
      </div>

    </div>

  </section>


  <section class="section" id="sobre">

    <h2>📊 Sobre o CelularTOP</h2>

    <p style="color:#9ca3af; line-height:1.8;">
      O CelularTOP é um projeto criado para facilitar a comparação
      entre celulares, mostrando desempenho, câmera, bateria e
      custo-benefício em um ranking simples.
    </p>

  </section>


  <footer>
    © 2026 CelularTOP — Todos os direitos reservados.
  </footer>


  <script>
    function pesquisarCelular() {

      const pesquisa =
        document.getElementById("search").value.toLowerCase();

      const celulares =
        document.querySelectorAll(".card");

      celulares.forEach(function(celular) {

        const nome =
          celular.dataset.name.toLowerCase();

        if (nome.includes(pesquisa)) {
          celular.style.display = "block";
        } else {
          celular.style.display = "none";
        }

      });
    }
  </script>
</body>
</html>
┌─────────────────────────────────┐
│          📱 CelularTOP           │
│                                 │
│   Encontre o melhor aparelho    │
│                                 │
│  ┌────────────┐ ┌────────────┐ │
│  │ 📱         │ │ 💻         │ │
│  │ CELULARES  │ │ PCs        │ │
│  │             │ │            │ │
│  │ Ver ranking │ │ Ver ranking│ │
│  └────────────┘ └────────────┘ │
└─────────────────────────────────┘
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>CelularTOP</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #080b12;
      color: white;
    }

    header {
      padding: 20px 6%;
      background: #101522;
      border-bottom: 1px solid #202838;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 25px;
      font-weight: bold;
    }

    .logo span {
      color: #4f8cff;
    }

    nav a {
      color: #aaa;
      text-decoration: none;
      margin-left: 20px;
    }

    nav a:hover {
      color: white;
    }

    .hero {
      text-align: center;
      padding: 70px 20px 40px;
    }

    .hero h1 {
      font-size: 42px;
      margin-bottom: 15px;
    }

    .hero h1 span {
      color: #4f8cff;
    }

    .hero p {
      color: #9ca3af;
      font-size: 17px;
    }

    .categorias {
      max-width: 900px;
      margin: 30px auto 70px;
      padding: 20px;
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 25px;
    }

    .categoria {
      background: #111827;
      border: 1px solid #273244;
      border-radius: 20px;
      padding: 40px 25px;
      text-align: center;
      cursor: pointer;
      transition: 0.25s;
    }

    .categoria:hover {
      transform: translateY(-6px);
      border-color: #4f8cff;
    }

    .categoria .icone {
      font-size: 60px;
      margin-bottom: 20px;
    }

    .categoria h2 {
      font-size: 26px;
      margin-bottom: 10px;
    }

    .categoria p {
      color: #9ca3af;
      margin-bottom: 25px;
    }

    .botao {
      display: inline-block;
      padding: 12px 25px;
      border-radius: 10px;
      background: #4f8cff;
      color: white;
      font-weight: bold;
    }

    .conteudo {
      display: none;
      padding: 30px 6% 70px;
    }

    .conteudo.ativo {
      display: block;
    }

    .titulo-secao {
      text-align: center;
      margin-bottom: 30px;
    }

    .titulo-secao h2 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    .titulo-secao p {
      color: #9ca3af;
    }

    .produtos {
      display: grid;
      grid-template-columns: repeat(
        auto-fit,
        minmax(230px, 1fr)
      );
      gap: 20px;
    }

    .produto {
      background: #111827;
      border: 1px solid #202838;
      border-radius: 16px;
      padding: 20px;
    }

    .produto-imagem {
      height: 160px;
      border-radius: 12px;
      background: #1a2231;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 55px;
      margin-bottom: 15px;
    }

    .produto h3 {
      font-size: 20px;
      margin-bottom: 10px;
    }

    .nota {
      color: #4f8cff;
      font-size: 22px;
      font-weight: bold;
      margin-bottom: 10px;
    }

    .produto p {
      color: #9ca3af;
      line-height: 1.7;
    }

    .voltar {
      display: block;
      width: fit-content;
      margin: 35px auto 0;
      padding: 12px 25px;
      background: #202838;
      border-radius: 10px;
      cursor: pointer;
    }

    footer {
      text-align: center;
      padding: 30px;
      color: #6b7280;
      background: #101522;
    }

    @media (max-width: 650px) {
      .categorias {
        grid-template-columns: 1fr;
      }

      .hero h1 {
        font-size: 32px;
      }

      header {
        flex-direction: column;
        gap: 15px;
      }
    }
  </style>
</head>

<body>

  <header>

    <div class="logo">
      Celular<span>TOP</span>
    </div>

    <nav>
      <a href="#" onclick="mostrarInicio()">Início</a>
    </nav>

  </header>


  <main>

    <!-- INÍCIO -->

    <section id="inicio">

      <div class="hero">

        <h1>
          Encontre o seu <span>TOP</span>
        </h1>

        <p>
          Compare celulares e computadores em um só lugar.
        </p>

      </div>


      <div class="categorias">

        <div
          class="categoria"
          onclick="mostrarCategoria('celulares')"
        >

          <div class="icone">📱</div>

          <h2>Celulares</h2>

          <p>
            Rankings, preços, desempenho,
            câmera e bateria.
          </p>

          <div class="botao">
            Ver celulares
          </div>

        </div>


        <div
          class="categoria"
          onclick="mostrarCategoria('pcs')"
        >

          <div class="icone">💻</div>

          <h2>PCs</h2>

          <p>
            Computadores, desempenho,
            componentes e preços.
          </p>

          <div class="botao">
            Ver PCs
          </div>

        </div>

      </div>

    </section>


    <!-- CELULARES -->

    <section
      id="celulares"
      class="conteudo"
    >

      <div class="titulo-secao">

        <h2>📱 Ranking de Celulares</h2>

        <p>
          Encontre os melhores celulares
          para cada necessidade.
        </p>

      </div>


      <div class="produtos">

        <div class="produto">

          <div class="produto-imagem">
            📱
          </div>

          <h3>Galaxy A15</h3>

          <div class="nota">
            8.5/10
          </div>

          <p>
            ⚡ Desempenho: 8/10<br>
            📸 Câmera: 8/10<br>
            🔋 Bateria: 9/10
          </p>

        </div>


        <div class="produto">

          <div class="produto-imagem">
            📱
          </div>

          <h3>Redmi Note 13</h3>

          <div class="nota">
            8.8/10
          </div>

          <p>
            ⚡ Desempenho: 9/10<br>
            📸 Câmera: 8/10<br>
            🔋 Bateria: 9/10
          </p>

        </div>

      </div>


      <div
        class="voltar"
        onclick="mostrarInicio()"
      >
        ← Voltar
      </div>

    </section>


    <!-- PCS -->

    <section
      id="pcs"
      class="conteudo"
    >

      <div class="titulo-secao">

        <h2>💻 Ranking de PCs</h2>

        <p>
          Compare computadores por desempenho
          e custo-benefício.
        </p>

      </div>


      <div class="produtos">

        <div class="produto">

          <div class="produto-imagem">
            💻
          </div>

          <h3>PC Gamer Básico</h3>

          <div class="nota">
            8.2/10
          </div>

          <p>
            ⚡ Processador: i5<br>
            🧠 RAM: 16 GB<br>
            💾 SSD: 240 GB
          </p>

        </div>


        <div class="produto">

          <div class="produto-imagem">
            🖥️
          </div>

          <h3>PC Gamer Intermediário</h3>

          <div class="nota">
            9.1/10
          </div>

          <p>
            ⚡ Processador: Ryzen 5<br>
            🧠 RAM: 16 GB<br>
            💾 SSD: 480 GB
          </p>

        </div>

      </div>


      <div
        class="voltar"
        onclick="mostrarInicio()"
      >
        ← Voltar
      </div>

    </section>

  </main>


  <footer>
    © 2026 CelularTOP
  </footer>


  <script>

    function esconderTudo() {

      document
        .getElementById("inicio")
        .style.display = "none";

      document
        .getElementById("celulares")
        .classList.remove("ativo");

      document
        .getElementById("pcs")
        .classList.remove("ativo");
    }


    function mostrarCategoria(categoria) {

      esconderTudo();

      document
        .getElementById(categoria)
        .classList.add("ativo");

      window.scrollTo(0, 0);
    }


    function mostrarInicio() {

      document
        .getElementById("inicio")
        .style.display = "block";

      document
        .getElementById("celulares")
        .classList.remove("ativo");

      document
        .getElementById("pcs")
        .classList.remove("ativo");

      window.scrollTo(0, 0);
    }

  </script>

</body>
</html>
